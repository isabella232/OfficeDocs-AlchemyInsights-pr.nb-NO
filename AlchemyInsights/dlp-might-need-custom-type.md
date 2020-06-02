---
title: DLP trenger kanskje en egendefinert type
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507523"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP trenger kanskje en egendefinert type

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP kan kreve en egendefinert informasjonstype**

Med en DLP-policy (Data Loss Prevention) kan du identifisere og beskytte sensitive data i organisasjonen. I noen scenarier må du kanskje opprette din egen **egendefinerte** sensitive informasjonstype for å beskytte organisasjonens data.

Organisasjonen må for eksempel kanskje identifisere og beskytte ansatt-ID-er eller andre data i et format som er spesifikt for organisasjonen. I så fall kan du se følgende artikler for mer informasjon.
  
 **Tilpasse en innebygd sensitiv informasjonstype**
  
Hvis en innebygd sensitiv informasjonstype vil møte dine behov med bare noen få tilpasninger, kan du [tilpasse en innebygd sensitiv informasjonstype](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Du kan for eksempel legge til eller fjerne søkeord, eller legge til eller fjerne støttebevis, for eksempel en dato eller adresse.
  
 **Opprette en egendefinert sensitiv informasjonstype**
  
Men hvis du må identifisere og beskytte en annen type sensitiv informasjon helt, kan du [opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) i brukergrensesnittet i Sikkerhets- & Compliance Center.
  
**Opprette en egendefinert sensitiv informasjonstype i Sikkerhet & Compliance Center PowerShell**

Til slutt, hvis brukergrensesnittet ikke gir alle alternativene du trenger, kan du [opprette en egendefinert sensitiv informasjonstype i Sikkerhet & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Ved å starte med en XML-fil kan du bruke alle tilgjengelige alternativer.
