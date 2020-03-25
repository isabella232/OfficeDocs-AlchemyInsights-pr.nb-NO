---
title: SharePoint Online regulering
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931235"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online regulering

**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen. Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger. I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.

Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene. Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider. I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.

**503-serveren er opptatt feil**

Brukere kan få en 503-server er opptatt feil når du prøver å navigere til SharePoint eller OneDrive-områder. 

Denne feilen kan skyldes regulering i SharePoint-tjenesten. SharePoint Online bruker regulering for å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten. Regulering begrenser antall brukerhandlinger eller samtidige anrop (etter skript eller kode) for å forhindre overforbruk av ressurser. 

Hvis du vil ha mer informasjon om regulering, [se, Unngå å bli strupet eller blokkert i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Hvis du mener at denne feilen ikke er relatert til regulering, kan du kontrollere om det oppstår aktivt vedlikehold på leieren ved å navigere til [meldingssenteret](https://portal.office.com/adminportal/home#/MessageCenter).

 Til slutt må du sørge for at du besøker [Siden Servicehelse](https://portal.office.com/adminportal/home#/servicehealth) for å se etter eventuelle råd/hendelser som kan forekomme.

