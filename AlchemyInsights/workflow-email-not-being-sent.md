---
title: E-post for arbeidsflyt sendes ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049382"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-post for arbeidsflyt sendes ikke for SharePoint-lister eller-biblioteker

1. E-post fra arbeidsflyter sendes ikke til alle brukere eller bare bestemte brukere, eller du ser feilen **e-postmeldingen ikke kan sendes. Kontroller at e-postmeldingen har en gyldig mottaker**.

    Kontroller om brukeren finnes i gruppen **alle personer** tillatelser (Brukerinformasjonsliste) for denne områdesamlingen.  Eksempel på direkte URL-<tenant>adresse:<sitename>https://. SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0

    - Hvis brukeren ikke finnes, må du kontrollere at brukeren er logget på siden. 
    - Hvis det er en ekstern bruker, må du kontrollere at invitasjonen er godtatt.
    - Hvis brukeren finnes i tillatelsesgruppen, må du kontrollere at e-postadressen er riktig.
    - Hvis brukerens e-postadresse ikke er angitt her, kan du opprette et eksempel varsel for den brukeren som tvinger synkroniseringen av denne brukerkontoen fra brukerprofiler for SharePoint til områdesamlingen.
 
2. E-post fra arbeidsflyter sendes til administratorer for områdesamling, men ikke til andre brukere, og se feilen **http forbudt til <span>https:</span>//URL/_vti_bin/Client.xvc.sp.Utilities.Utility.SendEmail**.
 

    Se [Ingen tilgang når du sender en e-post til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontroller også at funksjonen områdesamling for **låsing av bruker tillatelse begrenset tilgang** ikke er aktiv.


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


