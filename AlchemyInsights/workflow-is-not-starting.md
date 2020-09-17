---
title: Arbeids flyten starter ikke
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794776"
---
# <a name="workflow-is-not-starting"></a>Arbeids flyten starter ikke

- Arbeids flyter i SharePoint 2010 og SharePoint 2013 starter ikke.

    - Hvis arbeids flyten ikke starter, kan det være et midlertidig tjeneste problem der brukere kan oppleve uregelmessige forsinkelser med arbeids flyt frem drift. Kontroller [instrument bordet for tjeneste tilstand](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen er berørt.

    - Hvis det har gått mer enn 24 timer siden du så dette problemet, kan du logge en støtte forespørsel. I mange tilfeller arbeider vi allerede med en løsning. Gi oss minst 24 timer til å fullføre en løsning.

- Arbeids flyter i SharePoint 2010 forsinket ved start.

    - Dette skjer hvis arbeids flyten utløses i store grupper. (for eksempel når flere elementer legges til samtidig).

    - Arbeids flyter er ikke utformet for å kjøre i sanntid, så en forsinkelse er ved å utforme virke måte.

   -  Hvis arbeids flyten er omfattende språk for Extensible Object Markup (XMOL), kan kompileringen ta lang tid. Se [denne](https://support.microsoft.com//kb/3043697) artikkelen.

    - Du bør forenkle arbeids flyten eller utforme den på nytt ved hjelp av arbeids flyt plattform typen Microsoft SharePoint 2013.

    - Hvis arbeids flyt loggen er blitt stor, kan det være lurt å tømme elementene eller opprette en ny logg liste.

        Mer informasjon: [Tøm arbeids flyt Logg](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft flyt inn i SharePoint Online?
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flyt](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


