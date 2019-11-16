---
title: Arbeidsflyten starter ikke
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "36738098"
---
# <a name="workflow-is-not-starting"></a>Arbeidsflyten starter ikke

- SharePoint 2010-og SharePoint 2013-arbeidsflyter starter ikke.

    - Hvis arbeidsflyten ikke starter, kan det være et midlertidig problem med tjenesten der brukere kan oppleve uregelmessige forsinkelser med fremdrift for arbeidsflyten. Kontroller [helse instrumentbordet for tjenesten](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen er berørt.

    - Hvis det har gått mer enn 24 timer siden du først så dette problemet, kan du logge en support billett. I mange tilfeller er vi allerede jobber med en løsning. Vennligst gi oss minst 24 timer for å fullføre en løsning.

- Arbeidsflyter for SharePoint 2010 forsinket ved oppstart.

    - Dette skjer hvis arbeidsflyten utløses i store partier. (for eksempel når flere elementer er lagt til samtidig).

    - Arbeidsflyter er ikke laget for å kjøre i sanntid, slik at en forsinkelse er etter utformings virkemåte.

   -  Hvis arbeidsflyten er kompleks Extensible Object Markup Language (XMOL), kan kompilering være treg. Sjekk [denne](https://support.microsoft.com//kb/3043697) artikkelen.

    - Du bør forenkle arbeidsflyten eller utforme den på ny ved hjelp av typen Microsoft SharePoint 2013 arbeidsflyt plattform.

    - Hvis arbeidsflytloggen er blitt stor, kan det hende du vil tømme elementene eller opprette en ny loggliste.

        Mer informasjon: [tømme Arbeidsflytlogg](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


