---
title: Komme i gang med SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051650"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="ec3c4-102">Arbeidsflyter i SharePoint</span><span class="sxs-lookup"><span data-stu-id="ec3c4-102">Workflows in SharePoint</span></span>

<span data-ttu-id="ec3c4-103">Hvis SharePoint-arbeidsflyter ikke sender e-post, kan organisasjonen har oppdaget grensene for Exchange Online avsender.</span><span class="sxs-lookup"><span data-stu-id="ec3c4-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="ec3c4-104">Feilmeldingen "arbeidsflyten er suspendert" kan oppstå hvis du har ett av følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="ec3c4-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="ec3c4-105">Du har en arbeidsflyt i SharePoint Online som bruker SharePoint 2010 eller SharePoint 2013 arbeidsflyt plattformtype.</span><span class="sxs-lookup"><span data-stu-id="ec3c4-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="ec3c4-106">Arbeidsflyten er konfigurert til å sende en egendefinert e-postmelding til mer enn 200 brukere om gangen, mer enn 10 000 mottakere per dag, eller mer enn 30 meldinger per minutt.</span><span class="sxs-lookup"><span data-stu-id="ec3c4-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="ec3c4-107">Når du kjører arbeidsflyten, e-postmeldingen er ikke sendt, og du legger merke til feilmeldingen, intern status er satt til suspendert eller kan ikke sende til en mottaker vises.</span><span class="sxs-lookup"><span data-stu-id="ec3c4-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="ec3c4-108">Hvis du vil ha mer informasjon, kan du se følgende [artikkel](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="ec3c4-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

