---
title: Ytelsesproblemer– SharePoint eller OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911851"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive treg, utilgjengelig eller utilgjengelig for flere brukere

SharePoint eller OneDrive kan være trege, utilgjengelige eller utilgjengelige, eller vise tjenesten utilgjengelig eller 503-feil, av flere årsaker:
  
- Hvis SharePoint- eller OneDrive-nettstedet er tregt eller forsinket for flere brukere, kan det være et midlertidig tjenesteproblem der brukere opplever uregelmessig forsinkelser eller navigasjonsfeil når de får tilgang til SharePoint nettsteder eller OneDrive innhold. Kontroller [instrumentbordet for tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for å se om organisasjonen påvirkes.
  
- Brukere kan få en *feilmelding om at 503-serveren* er opptatt når de prøver å navigere til SharePoint eller OneDrive nettsteder. Denne feilen kan være forårsaket av begrensning i SharePoint tjenesten. SharePoint Online bruker begrensning til å opprettholde optimal ytelse og pålitelighet for SharePoint Online-tjenesten. Begrensning begrenser antall brukerhandlinger eller samtidige anrop (via skript eller kode) for å hindre overforbruk av ressurser. Hvis du vil ha mer informasjon om begrensning, kan du se Unngå å bli begrensning eller blokkert [i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Hvis du opplever dårlig  ytelse  med en klassisk eller moderne SharePoint nettsted eller side, kan du bruke verktøyet [Sidediagnose](https://aka.ms/perftool) til å analysere sidene.
  
- Hvis du fremdeles opplever generell dårlig ytelse, kan du se gjennom ressursene nederst i denne artikkelen: Innføring i [ytelsesjustering for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  