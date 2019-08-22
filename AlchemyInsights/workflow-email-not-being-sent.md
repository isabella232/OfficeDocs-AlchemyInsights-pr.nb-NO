---
title: Arbeidsflyt for e-post blir ikke sendt
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
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530892"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Arbeidsflyt for e-post blir ikke sendt til en SharePoint-liste eller et bibliotek

1. E-post fra arbeidsflyter er ikke sendt til alle brukere eller bare bestemte brukere, eller du ser feil **i e-postmeldingen ikke kan sendes. Kontroller at e-postmeldingen har en gyldig mottaker**.

    Kontroller om brukeren finnes i **Alle** tillatelsene gruppen (Brukerinformasjonsliste) for denne områdesamlingen.  Eksempel på direkte URL-adressen: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Hvis brukeren ikke finnes, kontrollerer du at brukeren er logget inn på siden. 
    - Hvis det er en ekstern bruker, må du kontrollere at deres invitasjonen er godtatt.
    - Hvis brukeren finnes i gruppen tillatelser, må du kontrollere e-postadressen er riktig.
    - Hvis e-postadressen som brukerne ikke er angitt her, oppretter du et eksempel på varselet for brukeren som fremtvinger synkronisering av brukerkontoen fra profiler av SharePoint for denne områdesamlingen.
 
2. E-post fra arbeidsflyter er sendt til administratorene for områdesamling, men ikke til andre brukere, og se feilen **HTTP forbudt å <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Se [Tilgang når du sender en e-post til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontroller også at funksjonen **begrenset tilgang tillatelse lockdown brukermodus** samlingen ikke er aktiv.


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opprette flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flyt](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


