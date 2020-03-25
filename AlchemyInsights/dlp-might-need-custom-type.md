---
title: DLP trenger kanskje en egendefinert type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932667"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP trenger kanskje en egendefinert type

**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen. Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger. I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.

Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene. Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider. I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.

**DLP kan kreve en egendefinert informasjonstype**

Med en policy for hindring av tap av data (DLP) kan du identifisere og beskytte sensitive data i organisasjonen. I noen scenarier må du kanskje opprette din egen **egendefinerte** sensitive informasjonstype for å beskytte organisasjonens data.

Organisasjonen må for eksempel kanskje identifisere og beskytte ansatt-IDer eller andre data i et format som er spesifikt for organisasjonen. I så fall kan du se følgende artikler for mer informasjon.
  
 **Tilpasse en innebygd sensitiv informasjonstype**
  
Hvis en innebygd sensitiv informasjonstype vil møte dine behov med bare noen få tweaks, kan du [tilpasse en innebygd sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Du kan for eksempel legge til eller fjerne søkeord, eller legge til eller fjerne støttebevis, for eksempel en dato eller adresse.
  
 **Opprette en egendefinert sensitiv informasjonstype**
  
Men hvis du trenger å identifisere og beskytte en annen type sensitiv informasjon helt, kan du [opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) i brukergrensesnittet i Security & Compliance Center.
  
**Opprette en egendefinert sensitiv informasjonstype i Security & Compliance Center PowerShell**

Til slutt, hvis brukergrensesnittet ikke inneholder alle alternativene du trenger, kan du [opprette en egendefinert sensitiv informasjonstype i Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Ved å starte med en XML-fil kan du bruke alle tilgjengelige alternativer.
