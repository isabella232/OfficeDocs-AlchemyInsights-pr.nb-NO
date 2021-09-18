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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446700"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP trenger kanskje en egendefinert type

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

**DLP kan kreve en egendefinert informasjonstype**

Med en policy for hindring av datatap (DLP) kan du identifisere og beskytte sensitive data i organisasjonen. I noen scenarioer må du kanskje opprette din egen egendefinerte sensitive informasjonstype for å beskytte organisasjonens data. Hvis du vil ha mer informasjon, kan du se Lære om [sensitive informasjonstyper](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) og enhetsdefinisjoner for Sensitiv [informasjonstype](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

Hvis du vil ha mer informasjon om hvordan du oppretter egendefinerte sensitive informasjonstyper og policyer, kan du se: 

**Tilpasse en innebygd sensitiv informasjonstype**

Hvis en innebygd sensitiv informasjonstype oppfyller behovene dine med bare noen få tilpasninger, kan du se Tilpasse en innebygd [sensitiv informasjonstype](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Du kan for eksempel legge til eller fjerne nøkkelord, eller legge til eller fjerne støttebevis, for eksempel en dato eller adresse.

**Opprette en egendefinert sensitiv informasjonstype**

Men hvis du trenger å identifisere og beskytte en annen type sensitiv informasjon helt, kan du opprette en egendefinert sensitiv informasjonstype i Samsvarssenter for Microsoft 365. Hvis du vil ha mer informasjon, [kan du se Komme i gang med egendefinerte sensitive informasjonstyper](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).

**Opprette en egendefinert sensitiv informasjonstype i Sikkerhets- &-samsvarssenteret PowerShell**

Hvis brukergrensesnittet ikke gir alle alternativene du trenger, kan du opprette en egendefinert sensitiv informasjonstype i PowerShell & Security & Compliance Center. Ved å begynne med en XML-fil kan du bruke alle tilgjengelige alternativer. Hvis du vil ha mer informasjon, [kan du se Opprette en egendefinert sensitiv informasjonstype ved hjelp av PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).

Hvis du vil teste policyen i testmodus først, kan du se Implementere policy i [testmodus](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) og Opprette, teste og justere [en DLP-policy](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy). 