---
title: DLP trenger kanskje en egendefinert type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030803"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP trenger kanskje en egendefinert type

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP kan kreve en egendefinert informasjonstype**

Med en policy for hindring av datatap (DLP) kan du identifisere og beskytte sensitive data i organisasjonen. I noen scenarioer må du kanskje opprette din egen egendefinerte **sensitive** informasjonstype for å beskytte organisasjonens data.

Organisasjonen må for eksempel kanskje identifisere og beskytte ansatt-ID-er eller andre data i et format som er spesifikk for organisasjonen. Hvis dette er det, kan du se følgende artikler for mer informasjon.
  
 **Tilpasse en innebygd sensitiv informasjonstype**
  
Hvis en innebygd sensitiv informasjonstype oppfyller behovene dine med bare noen få tilpasninger, kan du tilpasse en innebygd [sensitiv informasjonstype.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Du kan for eksempel legge til eller fjerne nøkkelord, eller legge til eller fjerne støttebevis, for eksempel en dato eller adresse.
  
 **Opprette en egendefinert sensitiv informasjonstype**
  
Men hvis du trenger å identifisere og beskytte en annen type sensitiv informasjon, kan du opprette en egendefinert [sensitiv](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) informasjonstype i brukergrensesnittet i sikkerhetssenteret & samsvarssenteret.
  
**Opprette en egendefinert sensitiv informasjonstype i Sikkerhets- & PowerShell**

Hvis brukergrensesnittet ikke har alle alternativene du trenger, kan du opprette en egendefinert sensitiv informasjonstype i [PowerShell & Security & Compliance Center.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Ved å begynne med en XML-fil kan du bruke alle tilgjengelige alternativer.
