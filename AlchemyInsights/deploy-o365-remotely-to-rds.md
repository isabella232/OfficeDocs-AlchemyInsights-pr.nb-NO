---
title: Distribuere Office 365 ProPlus for delt bruk på RDS, Terminal Server eller VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959468"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="121b3-102">Distribuere Office 365 ProPlus for delt bruk på RDS, Terminal Server eller VDI</span><span class="sxs-lookup"><span data-stu-id="121b3-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="121b3-103">Slik distribuerer du Office 365 ProPlus ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="121b3-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="121b3-104">Du må ha en Microsoft 365 for forretningsplan eller en Office 365-plan som inkluderer Office 365 ProPlus, for eksempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="121b3-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="121b3-105">Office 365 Business og Office 365 Business Premium-abonnementer inkluderer ikke Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="121b3-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="121b3-106">Du må aktivere [aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="121b3-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="121b3-107">Du kan også laste ned og kjøre [Microsoft Kundestøtte og gjenoppretting Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Office 365 ProPlus i aktiverings modus for delt datamaskin.</span><span class="sxs-lookup"><span data-stu-id="121b3-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="121b3-108">Hvis du vil ha mer informasjon om forutsetninger, oppsettsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av distribusjonsverktøyet for Office, kan du se [distribuere office 365 ProPlus ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="121b3-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="121b3-109">Slik retter du feil relatert til aktivering av delt datamaskin:</span><span class="sxs-lookup"><span data-stu-id="121b3-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="121b3-110">Se [Feilsøke problemer med aktivering av delt datamaskin for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="121b3-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="121b3-111">Se [tilbakestille aktiveringsstatusen for Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="121b3-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="121b3-112">Hvis du vil installere Office 365 ProPlus på RDS fra administrasjonssenteret for Microsoft 365, ***som bruker standard installasjonsinnstillinger***, bruker du følgende fremgangsmåte:</span><span class="sxs-lookup"><span data-stu-id="121b3-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="121b3-113">Sjekk hvilken Office 365 plan du har.</span><span class="sxs-lookup"><span data-stu-id="121b3-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="121b3-114">[Finn ut hvordan](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="121b3-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="121b3-115">Bytt om nødvendig til en annen plan i Office-365.</span><span class="sxs-lookup"><span data-stu-id="121b3-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="121b3-116">[Finn ut hvordan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="121b3-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="121b3-117">Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Office 365-planer, avinstallerer du det.</span><span class="sxs-lookup"><span data-stu-id="121b3-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="121b3-118">For eksempel ved å gå til **kontroll panel** > **avinstallere et program**.</span><span class="sxs-lookup"><span data-stu-id="121b3-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="121b3-119">Avinstaller ved hjelp av [Microsoft Kundestøtte og gjenoppretting Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du kjører i problemer.</span><span class="sxs-lookup"><span data-stu-id="121b3-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="121b3-120">På RDS-serveren logger du på administrasjonssenteret for Microsoft 365 med administratorkontoen og [installerer Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="121b3-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="121b3-121">Når Office er installert, må du ***ikke åpne eller logge på*** noen Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="121b3-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="121b3-122">Aktiver aktivering av delt datamaskin ved å redigere registret på RDS-serveren ved å følge disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="121b3-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="121b3-123">Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg **Kjør**.</span><span class="sxs-lookup"><span data-stu-id="121b3-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="121b3-124">I åpne-boksen skriver du inn **regedit**, og deretter velger du **OK**.</span><span class="sxs-lookup"><span data-stu-id="121b3-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="121b3-125">Velg **Yes (ja** ) når du blir spurt om du vil tillate at Registerredigering gjør endringer på enheten.</span><span class="sxs-lookup"><span data-stu-id="121b3-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="121b3-126">I Registerredigering legger du til en strengverdi på **SharedComputerLicensing** med en innstilling på 1 under HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="121b3-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="121b3-127">Logg på RDS-serveren ***som sluttbruker*** , og [Kontroller at aktivering av delt datamaskin er aktivert for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="121b3-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

