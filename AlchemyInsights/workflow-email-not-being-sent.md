---
title: E-post for arbeidsflyt sendes ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766142"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbeidsflyt-e-post sendes ikke for en SharePoint-liste eller et bibliotek

1. E-post fra arbeidsflyter sendes ikke til alle brukere eller bare bestemte brukere, eller du ser feilen **E-postmeldingen kan ikke sendes. Kontroller at e-posten har en gyldig mottaker**.

    Kontroller om brukeren finnes i gruppen **Alle personertillatelser** (brukerinformasjonsliste) for denne områdesamlingen.  Eksempel på direkte<tenant>URL-adresse: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MedlemskapGruppeId=0

    - Hvis brukeren ikke finnes, må du kontrollere at brukeren er logget på siden. 
    - Hvis det er en ekstern bruker, må du kontrollere at invitasjonen er godtatt.
    - Hvis brukeren finnes i tillatelsesgruppen, må du kontrollere at e-postadressen er riktig.
    - Hvis brukernes e-postadresse ikke er angitt her, oppretter du et eksempelvarsel for brukeren som tvinger synkroniseringen av denne brukerkontoen fra brukerprofiler i SharePoint til denne områdesamlingen.
 
2. E-post fra arbeidsflyter sendes til administratorer for områdesamling, men ikke til andre brukere og se feilen **HTTP forbudt å <span>https:</span>//URL/_vti_bin/client.xvc.sp.ilities.utility.SendEmail**.
 

    Se [Ingen tilgang når du sender en e-post til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontroller også at funksjonen for **begrenset tilgang til brukertillatelse lockdown modus** områdesamling ikke er aktiv.


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


