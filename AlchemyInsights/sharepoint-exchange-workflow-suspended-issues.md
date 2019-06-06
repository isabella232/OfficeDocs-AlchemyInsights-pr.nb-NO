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
ms.openlocfilehash: a44b2c7b26895e09c24df772f1ada9a2e3483747
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735991"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="3300b-102">Arbeidsflyter i SharePoint</span><span class="sxs-lookup"><span data-stu-id="3300b-102">Workflows in SharePoint</span></span>

<span data-ttu-id="3300b-103">Hvis SharePoint-arbeidsflyter ikke sender e-postmeldinger, kan organisasjonen har oppdaget Exchange Online sender grensene.</span><span class="sxs-lookup"><span data-stu-id="3300b-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="3300b-104">'Arbeidsflyten er avbrutt' feilmeldingen kan oppstå hvis du har én av følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="3300b-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="3300b-105">Du har en arbeidsflyt i SharePoint Online som bruker SharePoint 2010 eller SharePoint 2013 arbeidsflyttypen plattform.</span><span class="sxs-lookup"><span data-stu-id="3300b-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="3300b-106">Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere samtidig, mer enn 10 000 mottakere per dag, eller i mer enn 30 meldinger per minutt.</span><span class="sxs-lookup"><span data-stu-id="3300b-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="3300b-107">Når du starter arbeidsflyten, i e-postmeldingen sendes ikke, og du ser feilmeldingen, interne statusen er satt til Suspended eller kan sende til en mottaker vises.</span><span class="sxs-lookup"><span data-stu-id="3300b-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="3300b-108">Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="3300b-108">For more information, please refer to the following [article](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

