---
title: Mottok brukerne skadelig e-post
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291801"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="3bcf0-102">Mottok brukerne skadelig e-post?</span><span class="sxs-lookup"><span data-stu-id="3bcf0-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="3bcf0-103">Nå kan du rapportere skadelig e-post til Microsoft ved hjelp av [Administrasjonsinnsendinger i Sikkerhets- og samsvarssenteret](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="3bcf0-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="3bcf0-104">Meldinger som sendes i [administrasjonsinnsendinger](https://sip.protection.office.com/reportsubmission) blir skannet, og følgende resultater vises i **detalj** -undermenyen:</span><span class="sxs-lookup"><span data-stu-id="3bcf0-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="3bcf0-105">Hvis det oppstod en feil i avsenderens e-postgodkjenning på leveringstidspunktet.</span><span class="sxs-lookup"><span data-stu-id="3bcf0-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="3bcf0-106">Informasjon om eventuelle policy-treff som kan ha påvirket eller overstyrt avgjørelsen til en melding.</span><span class="sxs-lookup"><span data-stu-id="3bcf0-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="3bcf0-107">Gjeldende detonasjonsresultater viser om nettadressene eller filene i meldingen var skadelige eller ikke.</span><span class="sxs-lookup"><span data-stu-id="3bcf0-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="3bcf0-108">Tilbakemelding fra gradering</span><span class="sxs-lookup"><span data-stu-id="3bcf0-108">Feedback from graders</span></span>

<span data-ttu-id="3bcf0-109">Hvis det ble funnet en overstyring, skal den nye skanningen fullføres på noen minutter.</span><span class="sxs-lookup"><span data-stu-id="3bcf0-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="3bcf0-110">Hvis det ikke var et problem med e-postgodkjenning eller hvis leveringen ikke ble påvirket av en overstyring, kan tilbakemeldingen fra gradering ta opptil en dag.</span><span class="sxs-lookup"><span data-stu-id="3bcf0-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="3bcf0-111">Hvis du er uenig i den endelige avgjørelsen om en melding, nettadresse eller fil (blokkert i stedet for ikke blokkert), send meldingen på nytt etter en dag for ny skanning.</span><span class="sxs-lookup"><span data-stu-id="3bcf0-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="3bcf0-112">Det er store sjanser for at avgjørelsen endres når meldingen sendes på nytt.</span><span class="sxs-lookup"><span data-stu-id="3bcf0-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="3bcf0-113">I mellomtiden kan du fjerne skadelig e-post fra brukernes innbokser ved å følge instruksjonene i [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="3bcf0-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="3bcf0-114">Kunder med Microsoft Defender for Office 365 kan:</span><span class="sxs-lookup"><span data-stu-id="3bcf0-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="3bcf0-115">bruke [Trusselutforsker til å finne og slette mistenkelig e-post](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="3bcf0-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="3bcf0-116">[bruke klarerte lenker til å blokkere tilgang ](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) til en skadelig nettadresse</span><span class="sxs-lookup"><span data-stu-id="3bcf0-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="3bcf0-117">spore brukere som klikket og fikk tilgang til skadelige nettadresser: [Vise nettadresse for phishing og klikke avgjørelsesdata](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="3bcf0-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="3bcf0-118">manuelt [starte en automatisert undersøkelse](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="3bcf0-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="3bcf0-119">Du kan også beskytte deg mot skadelige filer og nettadresser ved å følge instruksjonene i [Beskyttelse mot skadelige nettadresser og filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="3bcf0-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>