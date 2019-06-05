---
title: Komme i gang med SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 9a8d72a01ed35794fcab370b48bbb189663d3396
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2019
ms.locfileid: "34718755"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="6c56d-102">Arbeidsflyter i SharePoint</span><span class="sxs-lookup"><span data-stu-id="6c56d-102">Workflows in SharePoint</span></span>

<p><span data-ttu-id="6c56d-103">Hvis SharePoint-arbeidsflyter ikke sender e-postmeldinger, kan organisasjonen har oppdaget Exchange Online sender grensene.&nbsp;</span><span class="sxs-lookup"><span data-stu-id="6c56d-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.&nbsp;</span></span></p> <p><span data-ttu-id="6c56d-104">'Arbeidsflyten er avbrutt' feilmeldingen kan oppstå hvis du har én av følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="6c56d-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span></p> <ul> <li><span data-ttu-id="6c56d-105">Du har en arbeidsflyt i SharePoint Online som bruker SharePoint 2010 eller SharePoint 2013 arbeidsflyttypen plattform.</span><span class="sxs-lookup"><span data-stu-id="6c56d-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span></li> <li><span data-ttu-id="6c56d-106">Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere samtidig, mer enn 10 000 mottakere per dag, eller i mer enn 30 meldinger per minutt.</span><span class="sxs-lookup"><span data-stu-id="6c56d-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span></li> <li><span data-ttu-id="6c56d-107">Når du starter arbeidsflyten, i e-postmeldingen sendes ikke, og du ser feilmeldingen, vises <strong>interne statusen er satt til Suspended</strong> eller <strong>kan ikke sende til en mottaker</strong> .</span><span class="sxs-lookup"><span data-stu-id="6c56d-107">When you run the workflow, the email message isn't sent, and you notice the error message, <strong>Internal Status is set to Suspended</strong> or <strong>Unable to send to a recipient</strong> is displayed.</span></span></li> </ul> <p><span data-ttu-id="6c56d-108">Hvis du vil ha mer informasjon, kan du se følgende <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">artikkel</a>.</span><span class="sxs-lookup"><span data-stu-id="6c56d-108">For more information, please refer to the following <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">article</a>.</span></span></p>

