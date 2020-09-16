---
title: E-post for arbeids flyt sendes ikke
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748998"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-post for arbeids flyt sendes ikke for en SharePoint-liste eller et bibliotek

1. E-post fra arbeids flyter sendes ikke til alle brukere eller bare bestemte brukere, eller du får feil **meldingen kan ikke sendes. Kontroller at e-posten har en gyldig mottaker**.

    Kontroller om brukeren er i gruppen **alle personer** tillatelser (bruker informasjons liste) for denne nettsteds samlingen.  Eksempel på direkte URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Hvis brukeren ikke finnes, må du kontrollere at brukeren er logget på siden. 
    - Hvis det er en ekstern bruker, må du kontrollere at invitasjonen er godtatt.
    - Hvis brukeren finnes i tillatelses gruppen, må du kontrollere at e-postadressen er riktig.
    - Hvis e-postadressen for brukere ikke er angitt her, oppretter du et eksempel varsel for brukeren som tvinger synkroniseringen av den bruker kontoen fra bruker profiler for SharePoint til denne nettsteds samlingen.
 
2. E-post fra arbeids flyter sendes til administratorer for område samlinger, men ikke til andre brukere og ser feil **http forbudt til <span>https:</span>//URL/_vti_bin/Client.xvc.sp.Utilities.Utility.SendEmail**.
 

    Se ingen [tilgang når du sender en e-post til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Kontroller også at funksjonen for **låsing av bruker tillatelse for begrenset tilgang** ikke er aktiv i nettsteds samlings modus.


## <a name="related-topics"></a>Beslektede emner
Vil du prøve Microsoft flyt inn i SharePoint Online?
- [Opprett flyt](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint og flyt](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


