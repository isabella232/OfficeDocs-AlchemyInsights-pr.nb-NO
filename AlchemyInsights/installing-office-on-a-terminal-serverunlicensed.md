---
title: Installere Office på en Terminal Server – ulisensiert
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663126"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="5269c-102">Installere Office på en terminalserver</span><span class="sxs-lookup"><span data-stu-id="5269c-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="5269c-103">For distribusjon av Microsoft 365-apper for bedrifter på en Windows-Server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="5269c-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="5269c-104">Du må ha et Microsoft 365-abonnement som inkluderer Microsoft 365-apper for Enterprise, for eksempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="5269c-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="5269c-105">Microsoft 365-appene for Business-og Microsoft 365-apper for Business Premium-planer inkluderer ikke Microsoft 365-apper for Enterprise.</span><span class="sxs-lookup"><span data-stu-id="5269c-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="5269c-106">Du må aktivere [aktivering av delt data maskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="5269c-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="5269c-107">Hvis du vil installere Microsoft 365-apper for Enterprise på RDS fra administrasjons senteret for Microsoft 365, ***som bruker standard installasjons innstillinger***, følger du Fremgangs måten nedenfor.</span><span class="sxs-lookup"><span data-stu-id="5269c-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="5269c-108">Du kan også laste ned og kjøre [Microsoft-assistenten for støtte og gjenoppretting](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Microsoft 365-apper for Enterprise i den delte data maskinens aktiverings modus.</span><span class="sxs-lookup"><span data-stu-id="5269c-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="5269c-109">Kontroller hvilket Microsoft 365-abonnement du har.</span><span class="sxs-lookup"><span data-stu-id="5269c-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="5269c-110">Finn ut hvordan</span><span class="sxs-lookup"><span data-stu-id="5269c-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="5269c-111">Bytt om nødvendig til et annet Microsoft 365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="5269c-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="5269c-112">Finn ut hvordan</span><span class="sxs-lookup"><span data-stu-id="5269c-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="5269c-113">Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft 365-abonnementer, må du avinstallere det.</span><span class="sxs-lookup"><span data-stu-id="5269c-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="5269c-114">Ved å gå til kontroll panel, må du for eksempel \> avinstallere et program.</span><span class="sxs-lookup"><span data-stu-id="5269c-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="5269c-115">Avinstaller ved hjelp av [Microsoft kunde støtte og gjenopprettings assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du har problemer.</span><span class="sxs-lookup"><span data-stu-id="5269c-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="5269c-116">På RDS-serveren logger du deg på administrasjons senteret for Microsoft 365 med administrator kontoen din og [installerer Microsoft 365-apper for Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="5269c-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="5269c-117">Når Office er installert, kan du ***ikke åpne eller logge på*** noen Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="5269c-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="5269c-118">Aktiver en delt data maskin aktivering på RDS-serveren ved å redigere registret ved å følge disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="5269c-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="5269c-119">Høyre klikk Windows-knappen i nedre venstre hjørne av skjermen, og velg Kjør.</span><span class="sxs-lookup"><span data-stu-id="5269c-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="5269c-120">Skriv inn **regedit**i åpne-boksen, og velg deretter OK.</span><span class="sxs-lookup"><span data-stu-id="5269c-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="5269c-121">Velg Ja når du blir bedt om å tillate register redigering for å gjøre endringer på enheten.</span><span class="sxs-lookup"><span data-stu-id="5269c-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="5269c-122">I register redigering legger du til en streng verdi på **SharedComputerLicensing** med en innstilling på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="5269c-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="5269c-123">***Logg på som en slutt bruker*** på RDS-serveren, og [Kontroller at den delte data maskin aktiveringen er aktivert for Microsoft 365-apper for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="5269c-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="5269c-124">Hvis du vil ha mer informasjon om forutsetninger, konfigurasjons instruksjoner og veiledning om tilpassede installasjoner ved hjelp av Office Deployment Tool, kan du se [distribuere Microsoft 365-apper for Enterprise ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="5269c-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="5269c-125">Hvis du vil løse feil relatert til aktivering av delt data maskin, kan du se [Feilsøke problemer med aktivering av delt data maskin for Microsoft 365-apper for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="5269c-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  