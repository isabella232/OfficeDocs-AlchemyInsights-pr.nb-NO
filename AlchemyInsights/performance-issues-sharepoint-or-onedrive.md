---
title: Ytelses problemer – SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771910"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive langsomt, utilgjengelig eller ikke tilgjengelig for flere brukere

SharePoint eller OneDrive kan være tregt, ikke tilgjengelig eller utilgjengelig, eller kan vise tjeneste utilgjengelig eller 503 feil, av flere årsaker:
  
- Hvis SharePoint-eller OneDrive-nettstedet er tregt eller forsinket for flere brukere, kan det oppstå et midlertidig tjeneste problem der brukere opplever periodiske forsinkelser eller navigasjons feil ved tilgang til SharePoint-nettsteder eller OneDrive-innhold. Kontroller [instrument bordet for tjeneste tilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen er berørt.
  
- Brukere kan få en *503-server er opptatt-* feil ved forsøk på å navigere til SharePoint-eller OneDrive-nettsteder. Denne feilen kan være forårsaket av begrensning i SharePoint-tjenesten. SharePoint Online bruker begrensning til å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten. Begrensning begrenser antall brukerhandlinger eller samtidige anrop (via skript eller kode) for å hindre overforbruk av ressurser. Hvis du vil ha mer informasjon om begrensning, kan du [unngå å bli begrenset eller blokkert i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Hvis du opplever lav ytelse med et **klassisk** eller **moderne** SharePoint-nettsted eller-side, bruker du [side diagnose verktøyet](https://aka.ms/perftool) til å analysere sidene.
  
- Hvis du fremdeles opplever generell dårlig ytelse, kan du se gjennom ressursene nederst i denne artikkelen: [innføring i ytelses justering for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  