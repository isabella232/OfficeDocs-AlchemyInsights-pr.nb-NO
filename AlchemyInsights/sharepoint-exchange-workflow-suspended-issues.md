---
title: Komme i gang med SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700716"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="1899c-102">Arbeids flyter i SharePoint</span><span class="sxs-lookup"><span data-stu-id="1899c-102">Workflows in SharePoint</span></span>

<span data-ttu-id="1899c-103">Hvis SharePoint-arbeidsflyter ikke sender e-postmeldinger, kan det hende at organisasjonen har funnet grensen for Exchange Online-avsenderen.</span><span class="sxs-lookup"><span data-stu-id="1899c-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="1899c-104">Feil meldingen «arbeids flyten er ute stengt» kan oppstå hvis du har ett av følgende elementer:</span><span class="sxs-lookup"><span data-stu-id="1899c-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="1899c-105">Du har en arbeids flyt i SharePoint Online som bruker arbeids flyt plattform typen for SharePoint 2010 eller SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="1899c-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="1899c-106">Arbeids flyten er konfigurert til å sende en egen definert e-postmelding til flere enn 200 brukere om gangen, mer enn 10 000 mottakere per dag eller mer enn 30 meldinger per minutt.</span><span class="sxs-lookup"><span data-stu-id="1899c-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="1899c-107">Når du kjører arbeids flyten, sendes ikke e-postmeldingen, og du ser feil meldingen, den interne statusen er satt til suspendert eller kan ikke sendes til en mottaker.</span><span class="sxs-lookup"><span data-stu-id="1899c-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="1899c-108">Hvis du vil ha mer informasjon, kan du se [artikkelen](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)nedenfor.</span><span class="sxs-lookup"><span data-stu-id="1899c-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

