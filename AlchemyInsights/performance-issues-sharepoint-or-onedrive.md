---
title: Ytelsesproblemer-SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068420"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive treg, utilgjengelig eller utilgjengelig for flere brukere

SharePoint eller OneDrive kan være treg, utilgjengelig eller utilgjengelig, eller kan vise tjenesten utilgjengelig eller 503 feil, av flere grunner:
  
- Hvis SharePoint-eller OneDrive-området er tregt eller forsinket for flere brukere, kan det være et midlertidig tjeneste problem der brukere opplever uregelmessige forsinkelser eller navigasjonsfeil ved tilgang til SharePoint-områder eller OneDrive-innhold. Kontroller [instrumentbordet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen er berørt.
  
- Brukere kan få en *503-server er opptatt* feil når du prøver å navigere til SharePoint eller OneDrive-områder. Denne feilen kan forårsakes av regulering i SharePoint-tjenesten. SharePoint Online bruker regulering for å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten. Regulering begrenser antall brukerhandlinger eller samtidige anrop (etter skript eller kode) for å hindre overforbruk av ressurser. Hvis du vil ha mer informasjon om regulering, kan du [unngå å få begrenset eller blokkert i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Hvis du opplever treg ytelse med et **klassisk** eller **moderne** SharePoint-område eller-side, bruker du [side diagnoseverktøyet](https://aka.ms/perftool) til å analysere sidene.
  
- Hvis du fremdeles opplever generell treg ytelse, kan du se gjennom ressursene nederst i denne artikkelen: [innføring i ytelsesjustering for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  