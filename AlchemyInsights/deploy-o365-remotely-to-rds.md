---
title: Distribuere Microsoft 365-apper for bedrifter for delt bruk på RDS, Terminal Server eller VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200682"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="811d0-102">Distribuere Microsoft 365-apper for bedrifter for delt bruk på RDS, Terminal Server eller VDI</span><span class="sxs-lookup"><span data-stu-id="811d0-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="811d0-103">Slik distribuerer du Microsoft 365-apper for bedrifter ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="811d0-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="811d0-104">Du må ha et Microsoft 365 For Business-abonnement eller et Office 365-abonnement som inneholder Microsoft 365-apper for bedrifter, for eksempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="811d0-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="811d0-105">Microsoft 365-appene for bedrifter og Microsoft 365 Business Standard-abonnementer inkluderer ikke Microsoft 365-apper for bedrifter.</span><span class="sxs-lookup"><span data-stu-id="811d0-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="811d0-106">Du må aktivere [aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="811d0-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="811d0-107">Du kan også laste ned og kjøre [Microsofts assistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) for støtte og gjenoppretting for å installere Microsoft 365-apper for bedrifter i modus for aktivering av delt datamaskin.</span><span class="sxs-lookup"><span data-stu-id="811d0-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="811d0-108">Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av distribusjonsverktøyet for Office, kan du se Distribuere [Microsoft 365-apper for bedrifter](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)ved hjelp av Eksterne skrivebordstjenester .</span><span class="sxs-lookup"><span data-stu-id="811d0-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="811d0-109">Slik løser du feil relatert til aktivering av delt datamaskin:</span><span class="sxs-lookup"><span data-stu-id="811d0-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="811d0-110">Se [Feilsøke problemer med aktivering av delt datamaskin for Microsoft 365-apper for bedrifter.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="811d0-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="811d0-111">Se [Tilbakestille Microsoft 365 Apps for enterprise for tilstand for organisasjonsaktivering](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="811d0-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="811d0-112">Hvis du vil installere Microsoft 365-apper for bedrifter på RDS fra administrasjonssenteret for Microsoft 365, som bruker standard installasjonsinnstillinger, bruker du følgende fremgangsmåte:</span><span class="sxs-lookup"><span data-stu-id="811d0-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="811d0-113">Kontroller hvilket abonnement du har.</span><span class="sxs-lookup"><span data-stu-id="811d0-113">Check what subscription you have.</span></span> <span data-ttu-id="811d0-114">[Finn ut hvordan](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="811d0-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="811d0-115">Bytt om nødvendig til et annet abonnement.</span><span class="sxs-lookup"><span data-stu-id="811d0-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="811d0-116">[Finn ut hvordan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="811d0-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="811d0-117">Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft-abonnementer, må du avinstallere det.</span><span class="sxs-lookup"><span data-stu-id="811d0-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="811d0-118">Du kan for eksempel gå til **Avinstallere** et program i  >  **kontrollpanelet.**</span><span class="sxs-lookup"><span data-stu-id="811d0-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="811d0-119">Avinstaller ved hjelp [av Microsofts assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) for støtte og gjenoppretting hvis det er problemer.</span><span class="sxs-lookup"><span data-stu-id="811d0-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="811d0-120">Logg på administrasjonssenteret for Microsoft 365 med administratorkontoen på RDS-serveren, og installer [Microsoft 365-apper for bedrifter.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="811d0-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="811d0-121">Når Office er installert, ***må du ikke åpne eller logge på*** noen Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="811d0-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="811d0-122">Aktiver aktivering av delt datamaskin på RDS-serveren ved å redigere registeret ved å følge disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="811d0-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="811d0-123">Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg **Kjør**.</span><span class="sxs-lookup"><span data-stu-id="811d0-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="811d0-124">Skriv regedit i **Åpne**-boksen, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="811d0-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="811d0-125">Velg **Ja** når du blir bedt om å tillate at Registerredigering gjør endringer på enheten.</span><span class="sxs-lookup"><span data-stu-id="811d0-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="811d0-126">Legg til en strengverdi for **SharedComputerLicensing** i Registerredigering med innstillingen 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="811d0-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="811d0-127">Logg på som sluttbruker  på RDS-serveren, og kontroller at aktivering av delt datamaskin er aktivert [for Microsoft 365-apper for bedrifter.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="811d0-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
