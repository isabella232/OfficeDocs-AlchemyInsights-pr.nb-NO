---
title: Feilsøke problemer med Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758074"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="5bc0f-102">Feilsøke problemer med Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="5bc0f-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="5bc0f-103">Vil du **merke forsinkelser med levering av e-postmeldinger**?</span><span class="sxs-lookup"><span data-stu-id="5bc0f-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="5bc0f-104">Prøv å bruke alternativet dynamisk levering for ATP-sikre Vedleggs policyer.</span><span class="sxs-lookup"><span data-stu-id="5bc0f-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="5bc0f-105">Dette vil unngå forsinkelser ved levering av e-postmeldinger mens du beskytter mottakere mot skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="5bc0f-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="5bc0f-106">**Vil du rapportere falske positiver eller falske negativer**?</span><span class="sxs-lookup"><span data-stu-id="5bc0f-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="5bc0f-107">Bruk denne koblingen til å sende inn filen for analyse: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="5bc0f-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="5bc0f-108">**Visste du at du kan aktivere ATP sikker koblings beskyttelse for e-post sendt mellom personer i organisasjonen**?</span><span class="sxs-lookup"><span data-stu-id="5bc0f-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="5bc0f-109">Følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="5bc0f-109">Follow these steps:</span></span>
    1. <span data-ttu-id="5bc0f-110">Gå til https://protection.office.com , og Logg deg på.</span><span class="sxs-lookup"><span data-stu-id="5bc0f-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="5bc0f-111">Gå til sikkerhets koblinger for **trussel administrasjons**  >  **policy**  >  **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="5bc0f-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="5bc0f-112">Rediger (eller Legg til) en policy under **policyer som gjelder for bestemte mottakere**.</span><span class="sxs-lookup"><span data-stu-id="5bc0f-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="5bc0f-113">Velg **Bruk sikre koblinger på meldinger som er sendt i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="5bc0f-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="5bc0f-114">Lagre policyen, og Tillat omtrent 30 minutter før endringene fungerer på sin måte gjennom data senteret.</span><span class="sxs-lookup"><span data-stu-id="5bc0f-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="5bc0f-115">Hvis du vil ha mer hjelp med ATP, kan du se [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="5bc0f-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>