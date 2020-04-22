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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716181"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="f5e2b-102">Fikse Office-appene «Vi kan ikke koble til akkurat nå»-meldingen</span><span class="sxs-lookup"><span data-stu-id="f5e2b-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="f5e2b-103">Hvis du mottar denne meldingen, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="f5e2b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f5e2b-104">Kontroller brannmur-, antivirusprogramvaren- og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Office-apper.</span><span class="sxs-lookup"><span data-stu-id="f5e2b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="f5e2b-105">Se [Microsoft-URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f5e2b-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f5e2b-106">Gå til **Start** > **Kjør**, og skriv deretter inn **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="f5e2b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f5e2b-107">Kontroller at følgende tjenester kjører:</span><span class="sxs-lookup"><span data-stu-id="f5e2b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f5e2b-108">Automatisk oppsett av nettverkstilkoblede enheter</span><span class="sxs-lookup"><span data-stu-id="f5e2b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f5e2b-109">Nettverkslistetjeneste</span><span class="sxs-lookup"><span data-stu-id="f5e2b-109">Network List Service</span></span>
    - <span data-ttu-id="f5e2b-110">Bevissthet om nettverksplassering</span><span class="sxs-lookup"><span data-stu-id="f5e2b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f5e2b-111">Hendelseslogg for Windows</span><span class="sxs-lookup"><span data-stu-id="f5e2b-111">Windows Event Log</span></span>

<span data-ttu-id="f5e2b-112">Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den.</span><span class="sxs-lookup"><span data-stu-id="f5e2b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f5e2b-113">Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekst med forhøyede tillatelser:</span><span class="sxs-lookup"><span data-stu-id="f5e2b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f5e2b-114">**sfc / scannow**</span><span class="sxs-lookup"><span data-stu-id="f5e2b-114">**sfc /scannow**</span></span>

<span data-ttu-id="f5e2b-115">Når denne kommandoen er fullført, starter du datamaskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="f5e2b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f5e2b-116">Hvis du vil ha detaljert informasjon, kan du se ["Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere" feil når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="f5e2b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>