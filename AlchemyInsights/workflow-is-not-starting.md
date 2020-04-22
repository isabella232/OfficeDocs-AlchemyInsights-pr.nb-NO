---
title: Arbeidsflyten starter ikke
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
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766106"
---
# <a name="workflow-is-not-starting"></a>Arbeidsflyten starter ikke

- SharePoint 2010- og SharePoint 2013-arbeidsflyter starter ikke.

    - Hvis arbeidsflyten ikke starter, kan det være et midlertidig tjenesteproblem der brukere kan oppleve periodiske forsinkelser med arbeidsflytfremdriften. Kontroller [instrumentbordet for servicetilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen påvirkes.

    - Hvis det har gått mer enn 24 timer siden du først så dette problemet, kan du logge en støttebillett. I mange tilfeller jobber vi allerede med en løsning. Vennligst gi oss minst 24 timer for å fullføre en løsning.

- SharePoint 2010 arbeidsflyter forsinket ved start.

    - Dette skjer hvis arbeidsflyten utløses i store partier. (for eksempel når flere elementer legges til samtidig).

    - Arbeidsflyter er ikke utformet for å kjøre sanntid, så en forsinkelse er etter utformingsvirkemåte.

   -  Hvis arbeidsflyten er kompleks xmol (Extensible Object Markup Language), kan kompilering være treg. Sjekk [denne](https://support.microsoft.com//kb/3043697) artikkelen.

    - Du bør forenkle arbeidsflyten eller utforme den på nytt ved hjelp av microsoft SharePoint 2013 arbeidsflytplattformtypen.

    - Hvis arbeidsflytloggen har blitt stor, kan det være lurt å tømme elementene eller opprette en ny loggliste.

        Mer informasjon : [Tøm arbeidsflytloggen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


