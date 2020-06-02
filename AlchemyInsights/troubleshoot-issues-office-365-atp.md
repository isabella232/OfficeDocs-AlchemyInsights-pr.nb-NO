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
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511121"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="c9338-102">Feilsøke problemer med Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="c9338-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="c9338-103">**Varselforsinkelser med levering av e-postmelding?**</span><span class="sxs-lookup"><span data-stu-id="c9338-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="c9338-104">Prøv å bruke alternativet Dynamisk levering for policyene for ATP-sikre vedlegg.</span><span class="sxs-lookup"><span data-stu-id="c9338-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="c9338-105">Dette vil unngå leveringsforsinkelser for e-postmeldinger samtidig som mottakerne beskyttes mot skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="c9338-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="c9338-106">**Vil du rapportere falske positive eller falske negativer?**</span><span class="sxs-lookup"><span data-stu-id="c9338-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="c9338-107">Bruk denne koblingen til å sende inn filen din for analyse:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="c9338-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="c9338-108">**Visste du at du kan aktivere ATP Safe Links beskyttelse for e-post sendt mellom personer i organisasjonen?**</span><span class="sxs-lookup"><span data-stu-id="c9338-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="c9338-109">Følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="c9338-109">Follow these steps:</span></span>
    1. <span data-ttu-id="c9338-110">Gå til https://protection.office.com , og logg på.</span><span class="sxs-lookup"><span data-stu-id="c9338-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="c9338-111">Gå **Threat management**til  >  **Sikker**  >  **koblinger**for trusselbehandling .</span><span class="sxs-lookup"><span data-stu-id="c9338-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="c9338-112">Under **Policyer som gjelder for bestemte mottakere**, rediger (eller legg til) en policy.</span><span class="sxs-lookup"><span data-stu-id="c9338-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="c9338-113">Velg **Bruk sikre koblinger på meldinger som sendes i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="c9338-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="c9338-114">Lagre retningslinjene dine, og la det gå omtrent 30 minutter før endringene fungerer seg gjennom datasenteret.</span><span class="sxs-lookup"><span data-stu-id="c9338-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="c9338-115">Hvis du vil ha mer hjelp med ATP, kan du se [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="c9338-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>