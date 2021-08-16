---
title: E-post for arbeidsflyt sendes ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072529"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbeidsflyt-e-post sendes ikke for en SharePoint liste eller bibliotek

1. E-post fra arbeidsflyter sendes ikke til alle brukere eller bare bestemte brukere, eller du ser feilen E-postmeldingen kan ikke sendes. Kontroller at **e-postmeldingen** har en gyldig mottaker .

    Kontroller om brukeren finnes i gruppen **Alle personer-tillatelser** (brukerinformasjonsliste) for denne nettstedssamlingen.  Eksempel på direkte nettadresse: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Hvis brukeren ikke finnes, må du kontrollere at brukeren er logget på siden. 
    - Hvis det er en ekstern bruker, må du kontrollere at invitasjonen er godtatt.
    - Hvis brukeren finnes i tillatelsesgruppen, må du kontrollere at e-postadressen er riktig.
    - Hvis brukernes e-postadresse ikke er angitt her, oppretter du et eksempelvarsel for denne brukeren som tvinger synkroniseringen av denne brukerkontoen fra brukerprofiler for SharePoint til denne nettstedssamlingen.
 
2. E-post fra arbeidsflyter sendes til administratorene for områdesamlingen, men ikke til andre brukere og ser feilen **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Se [Ingen tilgang når du sender en e-postmelding til en SharePoint gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontroller også at funksjonen **Låsingsmodus for brukertillatelser med** begrenset tilgang ikke er aktiv.


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opprette Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


