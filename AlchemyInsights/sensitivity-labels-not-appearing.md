---
title: Følsomhet-etiketter vises ikke
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801193"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="83212-102">Følsomhet-etiketter vises ikke</span><span class="sxs-lookup"><span data-stu-id="83212-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="83212-103">Med følsomhet-etiketter kan du klassifisere og bidra til å beskytte sensitivt innhold.</span><span class="sxs-lookup"><span data-stu-id="83212-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="83212-104">De kan opprettes i samsvars senteret for Microsoft 365, Microsoft 365 Security Center eller Microsoft 365-sikkerhets & Samsvars senteret under klassifisering > følsomhet-etiketter.</span><span class="sxs-lookup"><span data-stu-id="83212-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="83212-105">Hvis du vil lære mer om denne funksjonen, kan du se [Oversikt over følsomhet-etiketter](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="83212-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="83212-106">Hvis du har konfigurert følsomhet-etikettene, men de ikke vises i Microsoft 365-appene, kan du kontrollere følgende:</span><span class="sxs-lookup"><span data-stu-id="83212-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="83212-107">Kontroller at følsomhet-etiketten er [publisert](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) til brukerne og gruppene du vil bruke.</span><span class="sxs-lookup"><span data-stu-id="83212-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="83212-108">Kontroller at brukeren bruker en app som støtter følsomhet-etiketter – se [følsomhet-etiketter i dokumentet](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="83212-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="83212-109">Hvis du [overfører Azure Information Protection-etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), må du være oppmerksom på hvilke vurderinger som er oppført [her](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="83212-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="83212-110">Støtte for hindring av tap av data (DLP): nå kan bare oppbevarings etiketter brukes som en betingelse i policyer for DLP.</span><span class="sxs-lookup"><span data-stu-id="83212-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="83212-111">Støtte for følsomme etiketter i en DLP-policy er ikke tilgjengelig ennå, men vi jobber med den.</span><span class="sxs-lookup"><span data-stu-id="83212-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="83212-112">Når kryptering er aktivert på en følsomhet-etikett, kan du velge begge til:</span><span class="sxs-lookup"><span data-stu-id="83212-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="83212-113">Tilordne tillatelser nå</span><span class="sxs-lookup"><span data-stu-id="83212-113">Assign permissions now</span></span>
    - <span data-ttu-id="83212-114">La brukere tilordne tillatelser</span><span class="sxs-lookup"><span data-stu-id="83212-114">Let users assign permissions</span></span>


<span data-ttu-id="83212-115">Hvis du vil ha mer informasjon om mulige problemer, kan du se [kjente problemer med følsomhet-etiketter](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="83212-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>