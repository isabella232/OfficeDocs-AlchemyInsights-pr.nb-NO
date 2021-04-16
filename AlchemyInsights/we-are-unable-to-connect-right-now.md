---
title: Aktiveringsproblem – Vi kan ikke koble til akkurat nå
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806451"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="05d2f-102">Retting av Microsoft 365-appene Meldingen «Vi kan ikke koble til akkurat nå»</span><span class="sxs-lookup"><span data-stu-id="05d2f-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="05d2f-103">Hvis du mottar denne meldingen, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="05d2f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="05d2f-104">Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper.</span><span class="sxs-lookup"><span data-stu-id="05d2f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="05d2f-105">Se [Microsofts nettadresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="05d2f-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="05d2f-106">Gå til **Start**  >  **Kjør**, og skriv deretter **inn services.msc**.</span><span class="sxs-lookup"><span data-stu-id="05d2f-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="05d2f-107">Kontroller at følgende tjenester kjører:</span><span class="sxs-lookup"><span data-stu-id="05d2f-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="05d2f-108">Automatisk konfigurasjon av nettverkstilkoblingsenheter</span><span class="sxs-lookup"><span data-stu-id="05d2f-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="05d2f-109">Nettverkslistetjeneste</span><span class="sxs-lookup"><span data-stu-id="05d2f-109">Network List Service</span></span>
    - <span data-ttu-id="05d2f-110">Nettverksplasseringsbevissthet</span><span class="sxs-lookup"><span data-stu-id="05d2f-110">Network Location Awareness</span></span>
    - <span data-ttu-id="05d2f-111">Windows-hendelseslogg</span><span class="sxs-lookup"><span data-stu-id="05d2f-111">Windows Event Log</span></span>

<span data-ttu-id="05d2f-112">Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den.</span><span class="sxs-lookup"><span data-stu-id="05d2f-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="05d2f-113">Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med utvidede tillatelser:</span><span class="sxs-lookup"><span data-stu-id="05d2f-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="05d2f-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="05d2f-114">**sfc /scannow**</span></span>

<span data-ttu-id="05d2f-115">Når denne kommandoen er ferdig, starter du datamaskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="05d2f-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="05d2f-116">Hvis du vil ha detaljert informasjon, kan du se [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere» når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="05d2f-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>