---
title: Daglig e-postgrense overskredet. Arbeids flyten er suspendert.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731572"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="e4a7c-103">Daglig e-postgrense overskredet.</span><span class="sxs-lookup"><span data-stu-id="e4a7c-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="e4a7c-104">Arbeids flyten er suspendert.</span><span class="sxs-lookup"><span data-stu-id="e4a7c-104">Workflow is suspended.</span></span>

<span data-ttu-id="e4a7c-105">Denne feilen kan bli mottatt i følgende scenarioer:</span><span class="sxs-lookup"><span data-stu-id="e4a7c-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="e4a7c-106">Du har en arbeids flyt i SharePoint Online som bruker arbeids flyt plattform typen for SharePoint 2010 eller SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="e4a7c-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="e4a7c-107">Arbeids flyten er konfigurert til å sende en egen definert e-postmelding til flere enn 200 brukere om gangen, mer enn 10 000 mottakere per dag eller mer enn 30 meldinger per minutt.</span><span class="sxs-lookup"><span data-stu-id="e4a7c-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="e4a7c-108">Når du kjører arbeids flyten, sendes ikke e-postmeldingen, og du ser følgende virke måte:</span><span class="sxs-lookup"><span data-stu-id="e4a7c-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="e4a7c-109">For en arbeids flyt som bruker plattform typen for SharePoint 2013, går du til status siden for **arbeids flyten** .</span><span class="sxs-lookup"><span data-stu-id="e4a7c-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="e4a7c-110">På status siden for arbeids flyten er den **interne statusen** satt til **startet**, og informasjons boblen **kan ikke sendes til en mottaker**.</span><span class="sxs-lookup"><span data-stu-id="e4a7c-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="e4a7c-111">Du kan omgå dette problemet ved å konfigurere arbeids flyten til å sende e-postmeldinger uten å overskride [grensen for Exchange Online-avsenderen](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="e4a7c-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="e4a7c-112">Bruk for eksempel en pause i arbeids flyten, Send e-post til en Microsoft 365-gruppe, en distribusjons gruppe eller e-postaktivert sikkerhets gruppe, eller send meldingen til færre enn 200 mottakere om gangen.</span><span class="sxs-lookup"><span data-stu-id="e4a7c-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="e4a7c-113">Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="e4a7c-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="e4a7c-114">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="e4a7c-114">Related topics</span></span>
- [<span data-ttu-id="e4a7c-115">Opprett flyt</span><span class="sxs-lookup"><span data-stu-id="e4a7c-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e4a7c-116">SharePoint og flyt</span><span class="sxs-lookup"><span data-stu-id="e4a7c-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 