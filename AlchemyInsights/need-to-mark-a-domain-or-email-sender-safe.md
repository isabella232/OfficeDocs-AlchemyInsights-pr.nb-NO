---
title: Trenger du å merke et domene eller en e-post avsender trygt?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281180"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="3d6c3-102">Trenger du å merke et domene eller en e-post avsender trygt?</span><span class="sxs-lookup"><span data-stu-id="3d6c3-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="3d6c3-103">Bruk av **sikre avsenderlister anbefales ikke** siden den åpner opp organisasjonen for spam-, phish- og spoofing-angrep.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="3d6c3-104">Hvis det imidlertid er et forretningskrav, anbefaler vi **at** du bruker regler for **[e-postflyt](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for dette.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="3d6c3-105">Vår veiledning sikrer avsenderautentisering (bekrefter at sending av domene ikke blir forfalsket).</span><span class="sxs-lookup"><span data-stu-id="3d6c3-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="3d6c3-106">**Merk:** Vi anbefaler ikke å administrere falske positiver ved hjelp av sikre avsenderlister, fordi unntak fra spamfiltrering kan åpne organisasjonen for sikkerhetsangrep.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="3d6c3-107">Hvis brukeren(e) mottar meldinger som er feilaktig merket som søppelpost eller søppelpost, må du **[rapportere meldinger og filer til Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="3d6c3-108">Klarerte avsendere i Outlook, Tillatt avsenderliste eller tillatt domeneliste i policyer for anti-spam **bør unngås** fordi avsendere omgår all spam- og forfalskningsbeskyttelse og avsendergodkjenning (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="3d6c3-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="3d6c3-109">Denne metoden brukes best for midlertidig testing.</span><span class="sxs-lookup"><span data-stu-id="3d6c3-109">This method is best used for temporary testing only.</span></span>
