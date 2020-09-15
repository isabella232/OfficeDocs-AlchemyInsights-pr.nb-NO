---
title: DLP kan trenge en egen definert type
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
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712193"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP kan trenge en egen definert type

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP kan kreve en egen definert informasjons type**

Med en policy for hindring av tap av data (HINDRING) kan du identifisere og beskytte sensitive data i organisasjonen. I noen scenarioer kan det hende du må opprette en egen **definert** sensitiv informasjons type for å beskytte organisasjonens data.

Organisasjonen kan for eksempel identifisere og beskytte ansatt-IDer eller andre data i et bestemt format for organisasjonen. Hvis dette er tilfelle, kan du se følgende artikler for mer informasjon.
  
 **Tilpasse en innebygd sensitiv informasjons type**
  
Hvis en innebygd sensitiv informasjons type oppfyller behovene dine med bare noen få tilpasninger, kan du [tilpasse en innebygd sensitiv informasjons type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Du kan for eksempel legge til eller fjerne nøkkel ord, eller legge til eller fjerne støtte bevis som en dato eller adresse.
  
 **Opprette en egen definert sensitiv informasjons type**
  
Men hvis du trenger å identifisere og beskytte en annen type sensitiv informasjon helt, kan du [opprette en egen definert sensitiv informasjons type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i bruker grensesnittet til sikkerhets & samsvars senteret.
  
**Opprette en egen definert sensitiv informasjons type i sikkerhets & overholdelses senteret PowerShell**

Til slutt, hvis bruker grensesnittet ikke gir alle alternativene du trenger, kan du [opprette en egen definert sensitiv informasjons type i sikkerhets & Overholdelses senteret PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Når du starter med en XML-fil, kan du bruke alle alternativene som er tilgjengelige.
