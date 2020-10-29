---
title: Feilsøke problemer med Microsoft Defender for Office 365 (ATP)
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801416"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="cbac5-102">Feilsøke problemer med Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="cbac5-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="cbac5-103">Vil du **merke forsinkelser med levering av e-postmeldinger** ?</span><span class="sxs-lookup"><span data-stu-id="cbac5-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="cbac5-104">Prøv å bruke alternativet dynamisk levering for ATP-sikre Vedleggs policyer.</span><span class="sxs-lookup"><span data-stu-id="cbac5-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="cbac5-105">Dette vil unngå forsinkelser ved levering av e-postmeldinger mens du beskytter mottakere mot skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="cbac5-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="cbac5-106">**Vil du rapportere falske positiver eller falske negativer** ?</span><span class="sxs-lookup"><span data-stu-id="cbac5-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="cbac5-107">Bruk denne koblingen til å sende inn filen for analyse: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="cbac5-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="cbac5-108">**Visste du at du kan aktivere ATP sikker koblings beskyttelse for e-post sendt mellom personer i organisasjonen** ?</span><span class="sxs-lookup"><span data-stu-id="cbac5-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="cbac5-109">Følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="cbac5-109">Follow these steps:</span></span>
    1. <span data-ttu-id="cbac5-110">Gå til https://protection.office.com , og Logg deg på.</span><span class="sxs-lookup"><span data-stu-id="cbac5-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="cbac5-111">Gå til sikkerhets koblinger for **trussel administrasjons**  >  **policy**  >  **Safe Links** .</span><span class="sxs-lookup"><span data-stu-id="cbac5-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="cbac5-112">Rediger (eller Legg til) en policy under **policyer som gjelder for bestemte mottakere** .</span><span class="sxs-lookup"><span data-stu-id="cbac5-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="cbac5-113">Velg **Bruk sikre koblinger på meldinger som er sendt i organisasjonen** .</span><span class="sxs-lookup"><span data-stu-id="cbac5-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="cbac5-114">Lagre policyen, og Tillat omtrent 30 minutter før endringene fungerer på sin måte gjennom data senteret.</span><span class="sxs-lookup"><span data-stu-id="cbac5-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="cbac5-115">Hvis du vil ha mer hjelp med ATP, kan du se [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="cbac5-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>