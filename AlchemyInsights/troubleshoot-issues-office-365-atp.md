---
title: Feilsøke problemer med Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766754"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="b1df7-102">Feilsøke problemer med Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="b1df7-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="b1df7-103">**Legg merke til forsinkelser med levering av e-postmelding?**</span><span class="sxs-lookup"><span data-stu-id="b1df7-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="b1df7-104">Prøv å bruke alternativet Dynamisk levering for atp-retningslinjene for sikre vedlegg.</span><span class="sxs-lookup"><span data-stu-id="b1df7-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="b1df7-105">Dette vil unngå forsinkelser i levering av e-postmeldinger samtidig som mottakerne beskytter mot skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="b1df7-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="b1df7-106">**Vil du rapportere falske positiver eller falske negativer?**</span><span class="sxs-lookup"><span data-stu-id="b1df7-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="b1df7-107">Bruk denne koblingen til å sende inn filen din for analyse:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="b1df7-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="b1df7-108">**Visste du at du kan aktivere ATP Safe Links beskyttelse for e-post sendt mellom personer i organisasjonen?**</span><span class="sxs-lookup"><span data-stu-id="b1df7-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="b1df7-109">Følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="b1df7-109">Follow these steps:</span></span>
    1. <span data-ttu-id="b1df7-110">Gå https://protection.office.comtil , og logg på.</span><span class="sxs-lookup"><span data-stu-id="b1df7-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="b1df7-111">Gå til Safe Links for**Safe Links** **trusselstyring.** > **Policy** > </span><span class="sxs-lookup"><span data-stu-id="b1df7-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="b1df7-112">Under **Policyer som gjelder for bestemte mottakere**, redigerer (eller legger til) en policy.</span><span class="sxs-lookup"><span data-stu-id="b1df7-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="b1df7-113">Velg **Bruk sikre koblinger til meldinger som sendes i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="b1df7-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="b1df7-114">Lagre retningslinjene dine, og la endringene arbeide seg gjennom datasenteret.</span><span class="sxs-lookup"><span data-stu-id="b1df7-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="b1df7-115">Hvis du vil ha mer hjelp med ATP, kan du se [Avansert trusselbeskyttelse for Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="b1df7-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>