---
title: Feilsøke PRT-problem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573721"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="f489e-102">Feilsøke PRT-problem</span><span class="sxs-lookup"><span data-stu-id="f489e-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="f489e-103">For at alle enheter skal kunne bli godkjent, må den være fullstendig registrert og i god tilstand og ha mulighet til å skaffe seg et primært PRT (Primary Fresh token).</span><span class="sxs-lookup"><span data-stu-id="f489e-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="f489e-104">Hybrid registrerings prosessen for Azure AD JOIN krever at enheter er på et bedrifts nettverk.</span><span class="sxs-lookup"><span data-stu-id="f489e-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="f489e-105">Det fungerer også over VPN, men det er noen advarsler til dette.</span><span class="sxs-lookup"><span data-stu-id="f489e-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="f489e-106">Vi har hørt kunder som trenger hjelp med å feilsøke hybrid registrerings prosessen for Azure AD JOIN under eksterne arbeids omstendigheter.</span><span class="sxs-lookup"><span data-stu-id="f489e-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="f489e-107">Her er en analyse av hva som skjer under Vis avanserte innstillinger i løpet av registrerings prosessen.</span><span class="sxs-lookup"><span data-stu-id="f489e-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="f489e-108">**Sky godkjennings miljø (ved hjelp av hash-synkronisering eller direkte godkjenning av Azure AD Password)**</span><span class="sxs-lookup"><span data-stu-id="f489e-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="f489e-109">Denne registrerings flyten er også kjent som "Synkroniser join".</span><span class="sxs-lookup"><span data-stu-id="f489e-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="f489e-110">Windows 10 oppdager en SCP-post når brukeren logger seg på enheten.</span><span class="sxs-lookup"><span data-stu-id="f489e-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="f489e-111">Enheten prøver først å hente leier informasjon fra klient-IDen i registeret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="f489e-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="f489e-112">Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="f489e-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="f489e-113">Hvis den mislykkes, kommuniserer enheten med lokal Active Directory (AD) for å få leier informasjon fra tjeneste tilkoblings punkt (SCP).</span><span class="sxs-lookup"><span data-stu-id="f489e-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="f489e-114">Hvis du vil kontrollere SCP, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="f489e-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="f489e-115">Vi anbefaler å aktivere SCP i AD og bare bruke SCP for første Valide ring av klient-IDen.</span><span class="sxs-lookup"><span data-stu-id="f489e-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="f489e-116">Windows 10 prøver å kommunisere med Azure AD under system konteksten for å godkjenne seg selv mot Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f489e-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="f489e-117">Du kan kontrollere om enheten har tilgang til Microsoft-ressurser under system kontoen ved å bruke tilkoblings skriptet test enhets registrering.</span><span class="sxs-lookup"><span data-stu-id="f489e-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="f489e-118">Windows 10 genererer et selv signert sertifikat og lagrer det under data maskin objektet i lokal AD.</span><span class="sxs-lookup"><span data-stu-id="f489e-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="f489e-119">Dette krever linje med syns vidden til domene kontrolleren.</span><span class="sxs-lookup"><span data-stu-id="f489e-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="f489e-120">Et enhets objekt som har et sertifikat, blir synkronisert til Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f489e-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="f489e-121">Synkroniserings syklusen er hvert 30 minutt som standard, men den avhenger av konfigurasjon av Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="f489e-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="f489e-122">Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="f489e-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="f489e-123">På dette trinnet skal du kunne se emne enheten i tilstanden venter under enhets blad for Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="f489e-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="f489e-124">Registreringen blir fullført på den neste bruker påloggingen til Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f489e-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="f489e-125">Hvis du er på VPN og en avloggings prosess avslutter domene tilkoblingen, kan du utløse registreringen manuelt:</span><span class="sxs-lookup"><span data-stu-id="f489e-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="f489e-126">Utsted en dsregcmd/JOIN lokalt på administrator lede tekst eller eksternt via PSExec til PC-en.</span><span class="sxs-lookup"><span data-stu-id="f489e-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="f489e-127">For eksempel PsExec-s \\ win10client01 cmd, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="f489e-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="f489e-128">Hvis du vil ha mer informasjon om hybrid Sammenføynings problemer, kan du se [Feilsøke enheter-problem](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="f489e-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
