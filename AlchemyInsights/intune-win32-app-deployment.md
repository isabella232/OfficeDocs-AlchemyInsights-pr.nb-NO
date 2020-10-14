---
title: Distribusjon av Intune Win32-apper
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461874"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="2c1ca-102">Distribusjon av Intune Win32-apper</span><span class="sxs-lookup"><span data-stu-id="2c1ca-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="2c1ca-103">Microsoft Intune tillater Win32-programmer, inkludert, men ikke begrenset til MSI og. EXE skal distribueres til Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="2c1ca-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="2c1ca-104">Den brukte distribusjons mekanismen krever at Intune Management Extension (IME) er tilgjengelig på målenheten.</span><span class="sxs-lookup"><span data-stu-id="2c1ca-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="2c1ca-105">IME vil bli installert automatisk som et resultat av å identifisere et PowerShell-skript eller en Win32-program distribusjon til en bruker/enhet.</span><span class="sxs-lookup"><span data-stu-id="2c1ca-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="2c1ca-106">Det finnes også et sett med forhånds krav som må oppfylles for å kunne distribuere Win32-apper som omfatter:</span><span class="sxs-lookup"><span data-stu-id="2c1ca-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="2c1ca-107">Støttede plattformer: Windows 10 versjon 1607 eller nyere (Enterprise-, Pro-og Education-versjoner).</span><span class="sxs-lookup"><span data-stu-id="2c1ca-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="2c1ca-108">Arkitektur som støttes: x86 og x64.</span><span class="sxs-lookup"><span data-stu-id="2c1ca-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="2c1ca-109">Enhets behandling: AAD-koblet og automatisk registrert (inkludert hybrid domene som er sammenføyd og automatisk registrert for gruppe policy).</span><span class="sxs-lookup"><span data-stu-id="2c1ca-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="2c1ca-110">Format for program pakke:. **intunewin**  -fil som er klargjort av [verktøyet Microsoft Win32 Content forberedelser](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="2c1ca-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="2c1ca-111">Sine</span><span class="sxs-lookup"><span data-stu-id="2c1ca-111">Limitations:</span></span>
    - <span data-ttu-id="2c1ca-112">Maksimums størrelse: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="2c1ca-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="2c1ca-113">Arkitektur som ikke støttes: armer.</span><span class="sxs-lookup"><span data-stu-id="2c1ca-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="2c1ca-114">Se gjennom dokumentet «[Legg til, tilordne og Overvåk en Win32-app i Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)» for informasjon som er relatert til disse trinnene.</span><span class="sxs-lookup"><span data-stu-id="2c1ca-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="2c1ca-115">Detaljer om feil søking av program distribusjon på Windows, inkludert Win32-apper kan gjennomgås i følgende dokumenter</span><span class="sxs-lookup"><span data-stu-id="2c1ca-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="2c1ca-116">Feilsøke problemer med installasjon av apper</span><span class="sxs-lookup"><span data-stu-id="2c1ca-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="2c1ca-117">Feilsøke Win32-apper</span><span class="sxs-lookup"><span data-stu-id="2c1ca-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)