---
title: Trenger du å merke et domene eller en e-postavsender sikkert?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803254"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="3102f-102">Trenger du å merke et domene eller en e-postavsender sikkert?</span><span class="sxs-lookup"><span data-stu-id="3102f-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="3102f-103">Bruk av **klarerte avsender lister anbefales ikke** siden den åpner organisasjonen til søppel post, phish-og forfalsknings angrep.</span><span class="sxs-lookup"><span data-stu-id="3102f-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="3102f-104">Hvis det imidlertid finnes et bedrifts krav, **anbefaler vi at** du bruker **[regler for e-postflyt](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for dette.</span><span class="sxs-lookup"><span data-stu-id="3102f-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="3102f-105">Veiledningen vår sikrer at avsender godkjenning (bekrefter at du ikke forfalsker sending av domenet).</span><span class="sxs-lookup"><span data-stu-id="3102f-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="3102f-106">**Obs**! vi anbefaler ikke administrering av falske positiver ved hjelp av lister over klarerte avsendere, fordi unntak til søppel post filtrering kan åpne organisasjonen din for å sikre sikkerhets angrep.</span><span class="sxs-lookup"><span data-stu-id="3102f-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="3102f-107">Hvis brukeren (e) mottar meldinger som er feilaktig merket som søppel post eller søppel post, kan **[du rapportere meldinger og filer til Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="3102f-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="3102f-108">Klarerte avsendere i Outlook, listen over tillatte avsender, eller listen over tillatte søppel post, **må unngås** fordi avsendere hopper over all søppel post, forfalsking og phish beskyttelse og avsender godkjenning (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="3102f-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="3102f-109">Denne metoden brukes best bare for midlertidig testing.</span><span class="sxs-lookup"><span data-stu-id="3102f-109">This method is best used for temporary testing only.</span></span>
