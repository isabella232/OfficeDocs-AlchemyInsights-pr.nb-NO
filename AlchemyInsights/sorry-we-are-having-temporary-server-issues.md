---
title: Løse Microsoft 365-apper beklager, men vi har en melding om midlertidige serverproblemer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758254"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="a45c6-102">Løse Microsoft 365-appene «beklager, vi har midlertidige serverproblemer»-meldingen</span><span class="sxs-lookup"><span data-stu-id="a45c6-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="a45c6-103">Hvis du får denne meldingen, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="a45c6-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a45c6-104">Kontroller brann muren, antivirus program varen og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper.</span><span class="sxs-lookup"><span data-stu-id="a45c6-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="a45c6-105">Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="a45c6-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a45c6-106">Gå til **Start**  >  -**kjøring**, og skriv deretter inn **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="a45c6-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a45c6-107">Kontroller at følgende tjenester kjører:</span><span class="sxs-lookup"><span data-stu-id="a45c6-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a45c6-108">Automatisk konfigurasjon av Network tilkoblede enheter</span><span class="sxs-lookup"><span data-stu-id="a45c6-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a45c6-109">Nettverks liste tjeneste</span><span class="sxs-lookup"><span data-stu-id="a45c6-109">Network List Service</span></span>
    - <span data-ttu-id="a45c6-110">Nettverks plasserings forståelse</span><span class="sxs-lookup"><span data-stu-id="a45c6-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a45c6-111">Hendelses Logg for Windows</span><span class="sxs-lookup"><span data-stu-id="a45c6-111">Windows Event Log</span></span>

<span data-ttu-id="a45c6-112">Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den.</span><span class="sxs-lookup"><span data-stu-id="a45c6-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a45c6-113">Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en lede tekst med utvidede tillatelser:</span><span class="sxs-lookup"><span data-stu-id="a45c6-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a45c6-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="a45c6-114">**sfc /scannow**</span></span>

<span data-ttu-id="a45c6-115">Når denne kommandoen er ferdig, starter du data maskinen på nytt.</span><span class="sxs-lookup"><span data-stu-id="a45c6-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a45c6-116">Hvis du vil ha mer informasjon, kan du se [«beklager, vi har ikke koblet deg til kontoen din. Prøv på nytt senere-feil når du aktiverer](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="a45c6-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>