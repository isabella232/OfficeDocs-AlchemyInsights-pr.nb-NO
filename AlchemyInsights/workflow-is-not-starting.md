---
title: Arbeidsflyten starter ikke
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
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403752"
---
# <a name="workflow-is-not-starting"></a>Arbeidsflyten starter ikke

- SharePoint 2010- og SharePoint 2013-arbeidsflyter starter ikke.

    - Hvis arbeidsflyten ikke starter, kan det være et midlertidig tjenesteproblem der brukere kan oppleve uregelmessig forsinkelser med arbeidsflytfremdriften. Kontroller [instrumentbordet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home/servicehealth) for å se om organisasjonen påvirkes.

    - Hvis det har gått mer enn 24 timer siden du så dette problemet, logger du en støtteforespørsel. I mange tilfeller arbeider vi allerede med en løsning. Gi oss minst 24 timer for å fullføre en løsning.

- SharePoint 2010-arbeidsflyter forsinket ved start.

    - Dette skjer hvis arbeidsflyten utløses i store grupper. (for eksempel når flere elementer legges til samtidig).

    - Arbeidsflyter er ikke utformet for å kjøre i sanntid, så en forsinkelse er virkemåten til utformingen.

   -  Hvis arbeidsflyten er kompleks extensible Object Markup Language (XMOL), kan kompileringen gå tregt. Se [denne](https://support.microsoft.com//kb/3043697) artikkelen.

    - Du bør forenkle arbeidsflyten eller utforme den på nytt ved hjelp av plattformtypen Microsoft SharePoint 2013-arbeidsflyt.

    - Hvis arbeidsflytloggen har blitt stor, vil du kanskje fjerne elementene eller opprette en ny loggliste.

        Mer informasjon: [Tømme arbeidsflytloggen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opprette flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
