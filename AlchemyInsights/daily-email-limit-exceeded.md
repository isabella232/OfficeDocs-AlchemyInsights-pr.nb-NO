---
title: Daglig e-post er oversteget. Arbeidsflyten er avbrutt.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514472"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="f1118-103">Daglig e-post grensen overskredet.</span><span class="sxs-lookup"><span data-stu-id="f1118-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="f1118-104">Arbeidsflyten er avbrutt.</span><span class="sxs-lookup"><span data-stu-id="f1118-104">Workflow is suspended.</span></span>

<span data-ttu-id="f1118-105">Denne feilen kan mottas i følgende scenarier:</span><span class="sxs-lookup"><span data-stu-id="f1118-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="f1118-106">Du har en arbeidsflyt i SharePoint Online som bruker SharePoint 2010 eller SharePoint 2013 arbeidsflyttypen plattform.</span><span class="sxs-lookup"><span data-stu-id="f1118-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="f1118-107">Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere samtidig, mer enn 10 000 mottakere per dag, eller i mer enn 30 meldinger per minutt.</span><span class="sxs-lookup"><span data-stu-id="f1118-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="f1118-108">Når du starter arbeidsflyten, i e-postmeldingen sendes ikke, og du legge merke til følgende virkemåte:</span><span class="sxs-lookup"><span data-stu-id="f1118-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="f1118-109">For en arbeidsflyt ved hjelp av SharePoint 2013-plattformtype, bla til siden **Status for arbeidsflyt** .</span><span class="sxs-lookup"><span data-stu-id="f1118-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="f1118-110">Den **Interne statusen** er satt til **startet**på siden Status for arbeidsflyt, og boblen informasjon viser **kan ikke sende til en mottaker**.</span><span class="sxs-lookup"><span data-stu-id="f1118-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="f1118-111">Du kan omgå dette problemet ved å konfigurere arbeidsflyten for å sende e-postmeldinger uten å overskride [grensene for Exchange Online avsender](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="f1118-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="f1118-112">Hvis du for eksempel bruke en pause i arbeidsflyten, sende e-postmeldingen til en Office 365-gruppen, en distribusjonsgruppe eller sikkerhetsgruppe for e-post er aktivert eller sende meldingen til færre enn 200 mottakere om gangen.</span><span class="sxs-lookup"><span data-stu-id="f1118-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="f1118-113">Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="f1118-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="f1118-114">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="f1118-114">Related topics</span></span>
- [<span data-ttu-id="f1118-115">Opprette flyt</span><span class="sxs-lookup"><span data-stu-id="f1118-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="f1118-116">SharePoint og flyt</span><span class="sxs-lookup"><span data-stu-id="f1118-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 