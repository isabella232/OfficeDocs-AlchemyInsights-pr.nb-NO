---
title: Daglig e-postgrense overskredet. Arbeidsflyten er suspendert.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580342"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="2c7aa-103">Daglig e-postgrense overskredet.</span><span class="sxs-lookup"><span data-stu-id="2c7aa-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="2c7aa-104">Arbeidsflyten er suspendert.</span><span class="sxs-lookup"><span data-stu-id="2c7aa-104">Workflow is suspended.</span></span>

<span data-ttu-id="2c7aa-105">Denne feilen kan mottas i følgende scenarier:</span><span class="sxs-lookup"><span data-stu-id="2c7aa-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="2c7aa-106">Du har en arbeidsflyt i SharePoint Online som bruker sharepoint 2010- eller SharePoint 2013 arbeidsflytplattformtypen.</span><span class="sxs-lookup"><span data-stu-id="2c7aa-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="2c7aa-107">Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere om gangen, mer enn 10 000 mottakere per dag eller mer enn 30 meldinger per minutt.</span><span class="sxs-lookup"><span data-stu-id="2c7aa-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="2c7aa-108">Når du kjører arbeidsflyten, sendes ikke e-postmeldingen, og du legger merke til følgende virkemåte:</span><span class="sxs-lookup"><span data-stu-id="2c7aa-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="2c7aa-109">For en arbeidsflyt som bruker sharepoint 2013-plattformtypen, går du til siden **Arbeidsflytstatus.**</span><span class="sxs-lookup"><span data-stu-id="2c7aa-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="2c7aa-110">På siden Arbeidsflytstatus er **intern status** satt til **Startet**, og informasjonsboblen viser **Kan ikke sende til en mottaker**.</span><span class="sxs-lookup"><span data-stu-id="2c7aa-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="2c7aa-111">Du kan omgå dette problemet ved å konfigurere arbeidsflyten til å sende e-postmeldinger uten å overskride [Exchange Online-avsendergrensene](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="2c7aa-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="2c7aa-112">Bruk for eksempel en pause i arbeidsflyten, send e-posten til en Microsoft 365-gruppe, en distribusjonsgruppe eller en sikkerhetsgruppe som er aktivert for e-post, eller send meldingen til færre enn 200 mottakere om gangen.</span><span class="sxs-lookup"><span data-stu-id="2c7aa-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="2c7aa-113">Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="2c7aa-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="2c7aa-114">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="2c7aa-114">Related topics</span></span>
- [<span data-ttu-id="2c7aa-115">Opprett flyt</span><span class="sxs-lookup"><span data-stu-id="2c7aa-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="2c7aa-116">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="2c7aa-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 