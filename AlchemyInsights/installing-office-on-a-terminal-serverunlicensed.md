---
title: Installere kontoret på en Terminal Server - Ulisensiert
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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010623"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="3d790-102">Installere Office på en Terminal Server</span><span class="sxs-lookup"><span data-stu-id="3d790-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="3d790-103">For distribusjon av Microsoft 365 Apps for enterprise på en Windows Server ved hjelp av Remote Desktop Services (RDS), tidligere kalt Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="3d790-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="3d790-104">Du må ha et Microsoft 365-abonnement som inkluderer Microsoft 365 Apps for enterprise, for eksempel Office 365 Enterprise E3 eller Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="3d790-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="3d790-105">Microsoft 365 Apps for bedrifter og Microsoft 365 Apps for business Premium-planer inkluderer ikke Microsoft 365 Apps for enterprise.</span><span class="sxs-lookup"><span data-stu-id="3d790-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="3d790-106">Du må aktivere [aktivisering av delt datamaskin](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="3d790-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="3d790-107">Hvis du vil installere Microsoft 365 Apps for enterprise på RDS fra administrasjonssenteret for Microsoft 365, ***som bruker standard installasjonsinnstillinger***, bruker du følgende trinn.</span><span class="sxs-lookup"><span data-stu-id="3d790-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="3d790-108">Du kan også laste ned og kjøre [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) for å installere Microsoft 365 Apps for enterprise i delt datamaskinaktiveringsmodus.</span><span class="sxs-lookup"><span data-stu-id="3d790-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="3d790-109">Sjekk hva Microsoft 365-abonnementet du har.</span><span class="sxs-lookup"><span data-stu-id="3d790-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="3d790-110">Finn ut hvordan</span><span class="sxs-lookup"><span data-stu-id="3d790-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="3d790-111">Bytt om nødvendig til et annet Microsoft 365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="3d790-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="3d790-112">Finn ut hvordan</span><span class="sxs-lookup"><span data-stu-id="3d790-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="3d790-113">Hvis Office allerede er installert på RDS-serveren ved hjelp av andre Microsoft 365-abonnementer, må du avinstallere det.</span><span class="sxs-lookup"><span data-stu-id="3d790-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="3d790-114">Hvis du for eksempel \> går til Kontrollpanel Avinstaller et program.</span><span class="sxs-lookup"><span data-stu-id="3d790-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="3d790-115">Avinstaller ved hjelp av [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) hvis du støter på problemer.</span><span class="sxs-lookup"><span data-stu-id="3d790-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="3d790-116">Logg på administrasjonssenteret for Microsoft 365 med administratorkontoen, og [installer Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx)på RDS-serveren.</span><span class="sxs-lookup"><span data-stu-id="3d790-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="3d790-117">Når Office er installert, ***må du ikke åpne eller logge på*** noen Office-programmer.</span><span class="sxs-lookup"><span data-stu-id="3d790-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="3d790-118">Aktiver aktivisering av delt datamaskin på RDS-serveren ved å redigere registret ved å følge disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="3d790-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="3d790-119">Høyreklikk Windows-knappen nederst til venstre på skjermen, og velg Kjør.</span><span class="sxs-lookup"><span data-stu-id="3d790-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="3d790-120">Skriv inn **regedit**i Åpne-boksen, og velg deretter OK.</span><span class="sxs-lookup"><span data-stu-id="3d790-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="3d790-121">Velg Ja når du blir bedt om å tillate Registerredigering å gjøre endringer på enheten.</span><span class="sxs-lookup"><span data-stu-id="3d790-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="3d790-122">Legg til en strengverdi for **SharedComputerLicensing** i Registerredigering med en innstilling på 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="3d790-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="3d790-123">Logg på som ***sluttbruker på*** RDS-serveren, og kontroller at delt [datamaskinaktivering er aktivert for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="3d790-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="3d790-124">Hvis du vil ha mer informasjon om forutsetninger, installasjonsinstruksjoner og veiledning om tilpassede installasjoner ved hjelp av Office Deployment Tool, kan du se [Distribuere Microsoft 365 Apps for enterprise ved hjelp av Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="3d790-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="3d790-125">Hvis du vil løse feil relatert til delt datamaskinaktivering, kan du se [Feilsøke problemer med delt datamaskinaktivering for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="3d790-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  