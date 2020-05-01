---
title: MC210173 – utforming av nytt egendefinert skjema for SharePoint Designer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928536"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="1cf22-102">MC210173 – utforming av nytt egendefinert skjema for SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="1cf22-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="1cf22-103">Vi har identifisert et problem som berører SharePoint Designer-funksjonalitet for [oppretting av egendefinerte skjemaer](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1cf22-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="1cf22-104">Etter nøye gjennomgang har vi kommet frem til at det ikke finnes noen kjent løsning for dette problemet og har valgt å deaktivere funksjonen for tilpasset skjema-opprettelse fra og med kl. 03.00 UTC på lørdag 25. april 2020.</span><span class="sxs-lookup"><span data-stu-id="1cf22-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="1cf22-105">Denne endringen påvirker ikke muligheten til å redigere tidligere opprettede skjemaer eller andre eksisterende funksjoner i SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="1cf22-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="1cf22-106">Etter denne endringen var utført kan brukere ha mottatt feilen: «Kunne ikke lagre listeendringene på serveren», ved oppretting av nye skjemaer.</span><span class="sxs-lookup"><span data-stu-id="1cf22-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="1cf22-107">Brukere som tidligere har brukt SharePoint Designer til å opprette egendefinerte skjemaer, kan i stedet bruke [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) til dette formålet.</span><span class="sxs-lookup"><span data-stu-id="1cf22-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="1cf22-108">PowerApps er et enkelt og kraftig verktøy som gjør det mulig for brukere som bruker SharePoint Online Modern-opplevelsen, å opprette og redigere tilpassede skjemaer for SharePoint-lister og dokumentbiblioteker rett fra et nettleservindu.</span><span class="sxs-lookup"><span data-stu-id="1cf22-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="1cf22-109">PowerApps krever ikke kunnskap om tradisjonell koding eller andre appnedlastinger som for eksempel InfoPath.</span><span class="sxs-lookup"><span data-stu-id="1cf22-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="1cf22-110">**Obs**: Brukere av SharePoint Online Classic må midlertidig bytte til den moderne opplevelsen for tilgang til og for å bruke PowerApps, men alle tilpassede skjemaer opprettet i PowerApps, er tilgjengelige for brukere av SharePoint Online Class-opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="1cf22-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
