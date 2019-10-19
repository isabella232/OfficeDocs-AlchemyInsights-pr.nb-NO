---
title: Installere Office på en Terminal Server-ulisensiert
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205418"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="15774-102">Installere Office på en terminalserver</span><span class="sxs-lookup"><span data-stu-id="15774-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="15774-103">For distribusjon av Office 365 ProPlus på en Windows Server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="15774-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="15774-104">Du må ha en plan for Office 365 som inkluderer Office 365 ProPlus, for eksempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="15774-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="15774-105">Office 365 Business og Office 365 Business Premium-abonnementer inkluderer ikke Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="15774-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="15774-106">Du må aktivere [aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="15774-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="15774-107">Hvis du vil installere Office 365 ProPlus på RDS fra administrasjonssenteret for Microsoft 365, ***som bruker standard installasjonsinnstillinger***, bruker du følgende fremgangsmåte.</span><span class="sxs-lookup"><span data-stu-id="15774-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="15774-108">Du kan også laste ned og kjøre [Microsoft Kundestøtte og gjenoppretting Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Office 365 ProPlus i aktiverings modus for delt datamaskin.</span><span class="sxs-lookup"><span data-stu-id="15774-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="15774-109">Sjekk hvilken Office 365 plan du har.</span><span class="sxs-lookup"><span data-stu-id="15774-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="15774-110">Finn ut hvordan</span><span class="sxs-lookup"><span data-stu-id="15774-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="15774-111">Bytt om nødvendig til en annen plan i Office-365.</span><span class="sxs-lookup"><span data-stu-id="15774-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="15774-112">Finn ut hvordan</span><span class="sxs-lookup"><span data-stu-id="15774-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="15774-113">Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Office 365-planer, avinstallerer du det.</span><span class="sxs-lookup"><span data-stu-id="15774-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="15774-114">For eksempel ved å gå til kontroll panel \> Avinstaller et program.</span><span class="sxs-lookup"><span data-stu-id="15774-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="15774-115">Avinstaller ved hjelp av [Microsoft Kundestøtte og gjenoppretting Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du kjører i problemer.</span><span class="sxs-lookup"><span data-stu-id="15774-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="15774-116">På RDS-serveren logger du på administrasjonssenteret for Microsoft 365 med administratorkontoen og [installerer Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="15774-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="15774-117">Når Office er installert, må du ***ikke åpne eller logge på*** noen Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="15774-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="15774-118">Aktiver aktivering av delt datamaskin ved å redigere registret på RDS-serveren ved å følge disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="15774-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="15774-119">Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg Kjør.</span><span class="sxs-lookup"><span data-stu-id="15774-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="15774-120">I åpne-boksen skriver du inn **regedit**, og deretter velger du OK.</span><span class="sxs-lookup"><span data-stu-id="15774-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="15774-121">Velg Ja når du blir bedt om å tillate Registerredigering å gjøre endringer på enheten.</span><span class="sxs-lookup"><span data-stu-id="15774-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="15774-122">I Registerredigering legger du til en strengverdi på **SharedComputerLicensing** med en innstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="15774-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="15774-123">Logg på RDS-serveren ***som sluttbruker*** , og [Kontroller at aktivering av delt datamaskin er aktivert for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="15774-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="15774-124">Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av Office Deployment Tool, kan du se [distribuere Office 365 ProPlus ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="15774-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="15774-125">Hvis du vil rette feil relatert til aktivering av delt datamaskin, kan du se [Feilsøke problemer med delt datamaskinaktivering for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="15774-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  