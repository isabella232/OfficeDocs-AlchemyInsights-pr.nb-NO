---
title: Trenger du å merke et domene eller en e-post avsender som sikker?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792141"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="e7804-102">Trenger du å merke et domene eller en e-post avsender som sikker?</span><span class="sxs-lookup"><span data-stu-id="e7804-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="e7804-103">Bruk av **lister over klarerte avsendere** anbefales ikke siden det åpner opp organisasjonen for søppelpost, phish og forfalskende angrep.</span><span class="sxs-lookup"><span data-stu-id="e7804-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="e7804-104">Hvis det er et forretningskrav, anbefaler vi imidlertid **at** du bruker regler **[for](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** e-postflyt for dette.</span><span class="sxs-lookup"><span data-stu-id="e7804-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="e7804-105">Veiledningen vår sikrer at avsendergodkjenning (bekrefter at sending av domene ikke forfalskes).</span><span class="sxs-lookup"><span data-stu-id="e7804-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="e7804-106">**Obs!** Vi anbefaler ikke å behandle falske positiver ved å bruke lister over klarerte avsendere, fordi unntak fra søppelpostfiltrering kan åpne organisasjonen for sikkerhetsangrep.</span><span class="sxs-lookup"><span data-stu-id="e7804-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="e7804-107">Hvis brukeren(e) mottar meldinger som er feil merket som søppelpost, kan du **[rapportere meldinger og filer til Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="e7804-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="e7804-108">Klarerte avsendere i Outlook, listen over tillatte avsendere eller tillatte domener i søppelpostpolicyer bør unngås fordi avsendere omgår all søppelpost, forfalsket og phish-beskyttelse og avsendergodkjenning (SPF, DKIM, DMARC). </span><span class="sxs-lookup"><span data-stu-id="e7804-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="e7804-109">Denne metoden brukes best bare til midlertidig testing.</span><span class="sxs-lookup"><span data-stu-id="e7804-109">This method is best used for temporary testing only.</span></span>
