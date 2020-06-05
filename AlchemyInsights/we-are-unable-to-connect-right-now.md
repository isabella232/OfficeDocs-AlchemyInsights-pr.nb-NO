---
title: Aktiveringsproblem - Vi kan ikke koble til akkurat nå
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581884"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="fe618-102">Fikse Microsoft 365-appene "Vi kan ikke koble til akkurat nå"</span><span class="sxs-lookup"><span data-stu-id="fe618-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="fe618-103">Hvis du får denne meldingen, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="fe618-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fe618-104">Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper.</span><span class="sxs-lookup"><span data-stu-id="fe618-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="fe618-105">Se [Microsofts URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="fe618-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="fe618-106">Gå til **Start**  >  **Kjør**, og skriv deretter inn **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="fe618-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="fe618-107">Kontroller at følgende tjenester kjører:</span><span class="sxs-lookup"><span data-stu-id="fe618-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="fe618-108">Automatisk oppsett av nettverkstilkoblede enheter</span><span class="sxs-lookup"><span data-stu-id="fe618-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="fe618-109">Tjeneste for nettverksliste</span><span class="sxs-lookup"><span data-stu-id="fe618-109">Network List Service</span></span>
    - <span data-ttu-id="fe618-110">Bevissthet om nettverksplassering</span><span class="sxs-lookup"><span data-stu-id="fe618-110">Network Location Awareness</span></span>
    - <span data-ttu-id="fe618-111">Hendelseslogg for Windows</span><span class="sxs-lookup"><span data-stu-id="fe618-111">Windows Event Log</span></span>

<span data-ttu-id="fe618-112">Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den.</span><span class="sxs-lookup"><span data-stu-id="fe618-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="fe618-113">Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med forhøyede tillatelser:</span><span class="sxs-lookup"><span data-stu-id="fe618-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="fe618-114">**sfc /scannow (SFC/scannow)**</span><span class="sxs-lookup"><span data-stu-id="fe618-114">**sfc /scannow**</span></span>

<span data-ttu-id="fe618-115">Når denne kommandoen er fullført, starter du datamaskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="fe618-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="fe618-116">Hvis du vil ha detaljert informasjon, kan du se [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere" feil når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="fe618-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>