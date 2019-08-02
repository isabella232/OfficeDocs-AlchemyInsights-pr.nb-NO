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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059612"
---
# <a name="workflow-email-is-not-being-sent"></a>Arbeidsflyt for e-post blir ikke sendt

1. E-post fra arbeidsflyter er ikke sendt til alle brukere eller bare bestemte brukere, eller du ser feil **i e-postmeldingen ikke kan sendes. Kontroller at e-postmeldingen har en gyldig mottaker**.

Kontroller om brukeren finnes i **Alle** tillatelsene gruppen (Brukerinformasjonsliste) for denne områdesamlingen.  Eksempel på direkte URL-adressen: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

- Hvis brukeren ikke finnes, kontrollerer du at brukeren er logget inn på siden. 
- Hvis det er en ekstern bruker, må du kontrollere at deres invitasjonen er godtatt.
- Hvis brukeren finnes i gruppen tillatelser, må du kontrollere e-postadressen er riktig.
- Hvis e-postadressen som brukerne ikke er angitt her, oppretter du et eksempel på varselet for brukeren som fremtvinger synkronisering av brukerkontoen fra profiler av SharePoint for denne områdesamlingen.
 
2. E-post fra arbeidsflyter er sendt til administratorene for områdesamling, men ikke til andre brukere, og se feilen **HTTP forbudt å <spam> <spam> ** <spam> <spam>.
 

Se [Tilgang når sendt e-post til grupper](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

Kontroller også at funksjonen **begrenset tilgang tillatelse lockdown brukermodus** samlingen ikke er aktiv.

## <a name="related-topics"></a>Beslektede emner
- [Opprette flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flyt](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


