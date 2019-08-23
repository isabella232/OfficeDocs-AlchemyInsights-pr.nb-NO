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
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557988"
---
# <a name="workflow-is-not-starting"></a>Arbeidsflyten starter ikke

- Arbeidsflyter for SharePoint 2010 og SharePoint 2013 starter ikke.

    - Hvis arbeidsflyten ikke starter, kan det være et problem med midlertidig tjeneste der brukere kan oppleve periodiske forsinkelser med arbeidsflyten pågår. Kontroller [Service helse instrumentbord](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se Hvis din organisasjon er påvirket.

    - Hvis det har gått mer enn 24 timer etter at du først så dette problemet, logger du deg en support billett. I mange tilfeller kan arbeider vi allerede med en løsning. Gi oss minst 24 timer å fullføre en løsning.

- SharePoint 2010-arbeidsflyter forsinket på start.

    - Dette skjer hvis arbeidsflyten utløses i store grupper. (for eksempel når flere elementer er lagt til på en gang).

    - Arbeidsflyter er ikke utformet for å kjøre i sanntid, slik at en forsinkelse er standard virkemåte.

   -  Hvis arbeidsflyten er komplekse Extensible Object Markup Language (XMOL), kan det ta lang tid kompilering. Merk av i [denne](https://support.microsoft.com/en-us/kb/3043697) artikkelen.

    - Du må forenkle arbeidsflyten diagramstørrelsen eller ved hjelp av Microsoft SharePoint 2013 plattform arbeidsflyttypen.

    - Hvis din Arbeidsflytlogg er blitt stor, kanskje du vil tømme varene eller opprette en ny loggliste.

        Mer informasjon: [Tøm Arbeidsflytlogg](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft Flow i SharePoint Online?
- [Opprette flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flyt](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


