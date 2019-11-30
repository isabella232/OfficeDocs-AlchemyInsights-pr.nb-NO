---
title: Reparere Office-apper beklager, vi har midlertidig server problemer melding
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627999"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="92574-102">Fikse Office-programmer "Beklager, vi har midlertidige Server problemer"-melding</span><span class="sxs-lookup"><span data-stu-id="92574-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="92574-103">Hvis du får denne meldingen, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="92574-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="92574-104">Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Office-apper.</span><span class="sxs-lookup"><span data-stu-id="92574-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="92574-105">Se [URL-adresser for Office 365 og IP-adresser](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="92574-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="92574-106">Gå til **Start** > **Kjør**, og skriv deretter inn **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="92574-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="92574-107">Kontroller at følgende tjenester kjører:</span><span class="sxs-lookup"><span data-stu-id="92574-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="92574-108">Automatisk installasjon av nettverkstilkoblede enheter</span><span class="sxs-lookup"><span data-stu-id="92574-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="92574-109">Tjeneste for nettverksliste</span><span class="sxs-lookup"><span data-stu-id="92574-109">Network List Service</span></span>
    - <span data-ttu-id="92574-110">Kunnskap om nettverksplassering</span><span class="sxs-lookup"><span data-stu-id="92574-110">Network Location Awareness</span></span>
    - <span data-ttu-id="92574-111">Hendelseslogg for Windows</span><span class="sxs-lookup"><span data-stu-id="92574-111">Windows Event Log</span></span>

<span data-ttu-id="92574-112">Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den.</span><span class="sxs-lookup"><span data-stu-id="92574-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="92574-113">Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en ledetekstmed forhøyede tillatelser:</span><span class="sxs-lookup"><span data-stu-id="92574-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="92574-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="92574-114">**sfc /scannow**</span></span>

<span data-ttu-id="92574-115">Når denne kommandoen er ferdig, starter du datamaskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="92574-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="92574-116">Hvis du vil ha mer informasjon, se ["Beklager, vi kan ikke koble til kontoen din. Vennligst prøv igjen senere "feil når du aktiverer Office fra Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="92574-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>