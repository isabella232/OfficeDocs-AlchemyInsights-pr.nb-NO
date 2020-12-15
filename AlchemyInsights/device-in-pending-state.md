---
title: Enhet i ventende tilstand
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679998"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="2b794-102">Enhet i ventende tilstand</span><span class="sxs-lookup"><span data-stu-id="2b794-102">Device in pending state</span></span>

<span data-ttu-id="2b794-103">**Forhånds kravene forbindelse**</span><span class="sxs-lookup"><span data-stu-id="2b794-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="2b794-104">Hvis du setter opp enhets registreringer for første gang, må du sørge for at du har gjennomgått [innføring i enhets behandling i Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) som hjelper deg med å få tak i enheter under kontrollen av Azure ad.</span><span class="sxs-lookup"><span data-stu-id="2b794-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="2b794-105">Hvis du registrerer enheter i Azure AD direkte og registrerer dem i Intune, må du forsikre deg om at du har [konfigurert Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) og at [lisensen](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) er på plass først.</span><span class="sxs-lookup"><span data-stu-id="2b794-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="2b794-106">Sørg for at du er autorisert til å utføre operasjoner i Azure AD og lokalt AD.</span><span class="sxs-lookup"><span data-stu-id="2b794-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="2b794-107">Bare en global administrator i Azure AD kan administrere innstillinger for enhets registrering.</span><span class="sxs-lookup"><span data-stu-id="2b794-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="2b794-108">Hvis du i tillegg konfigurerer automatiske registreringer i den lokale Active Directory-katalogen, må du være administrator for Active Directory og AD FS (hvis aktuelt).</span><span class="sxs-lookup"><span data-stu-id="2b794-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="2b794-109">Hybrid registrerings prosessen for Azure AD JOIN krever at enheter er på bedrifts nettverk.</span><span class="sxs-lookup"><span data-stu-id="2b794-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="2b794-110">Det fungerer også over VPN, men det er noen advarsler til dette.</span><span class="sxs-lookup"><span data-stu-id="2b794-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="2b794-111">Vi har hørt kunder som trenger hjelp med å feilsøke hybrid registrerings prosessen for Azure AD JOIN under eksterne arbeids omstendigheter.</span><span class="sxs-lookup"><span data-stu-id="2b794-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="2b794-112">**Sky godkjennings miljø (ved hjelp av hash-synkronisering eller direkte godkjenning av Azure AD Password)**</span><span class="sxs-lookup"><span data-stu-id="2b794-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="2b794-113">Denne registrerings flyten er også kjent som "Synkroniser join".</span><span class="sxs-lookup"><span data-stu-id="2b794-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="2b794-114">Her er en analyse av hva som skjer under registrerings prosessen:</span><span class="sxs-lookup"><span data-stu-id="2b794-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="2b794-115">Windows 10 oppdager en post for tjeneste tilkoblings punkt (SCP) når brukeren logger seg på enheten.</span><span class="sxs-lookup"><span data-stu-id="2b794-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="2b794-116">Enheten prøver først å hente leier informasjon fra klient-IDen i registeret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="2b794-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="2b794-117">Hvis du vil ha mer informasjon, kan du se [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="2b794-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="2b794-118">Hvis den mislykkes, kommuniserer enheten med lokal Active Directory for å få leier informasjon fra SCP.</span><span class="sxs-lookup"><span data-stu-id="2b794-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="2b794-119">Hvis du vil kontrollere SCP, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="2b794-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="2b794-120">Vi anbefaler å aktivere SCP i Active Directory og bare bruke SCP-IDen for den første Valide ringen.</span><span class="sxs-lookup"><span data-stu-id="2b794-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="2b794-121">Windows 10 prøver å kommunisere med Azure AD under system konteksten for å godkjenne seg selv mot Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2b794-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="2b794-122">Du kan kontrollere om enheten har tilgang til Microsoft-ressurser under system kontoen ved å bruke [tilkoblings skriptet test enhets registrering](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="2b794-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="2b794-123">Windows 10 genererer selv signert sertifikat og lagrer det under data maskin objektet i lokal Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2b794-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="2b794-124">Dette krever linje med syns vidden til domene kontrolleren.</span><span class="sxs-lookup"><span data-stu-id="2b794-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="2b794-125">Enhets objekt som har sertifikat, synkroniseres til Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2b794-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="2b794-126">Synkroniserings syklusen er hvert 30 minutt som standard, men den avhenger av konfigurasjonen av Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="2b794-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="2b794-127">Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="2b794-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="2b794-128">På dette trinnet skal du kunne se emne enheten i tilstanden **venter** under enhets blad for Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="2b794-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="2b794-129">Registreringen blir fullført på den neste bruker påloggingen til Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2b794-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="2b794-130">Hvis du er på VPN og avlogging/pålogging avslutter domene tilkoblingen, kan du utløse registreringen manuelt.</span><span class="sxs-lookup"><span data-stu-id="2b794-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="2b794-131">Slik gjør du det:</span><span class="sxs-lookup"><span data-stu-id="2b794-131">To do that:</span></span>
    >
    > <span data-ttu-id="2b794-132">Utsted et `dsregcmd /join` lokalt på administrator lede tekst eller eksternt via PSExec til PC-en.</span><span class="sxs-lookup"><span data-stu-id="2b794-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="2b794-133">For eksempel: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="2b794-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="2b794-134">For vanlige problemer med registrering av Azure Active Directory-enhet, kan du se [vanlige spørsmål om enheter](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="2b794-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
