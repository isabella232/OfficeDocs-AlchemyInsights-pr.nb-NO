---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704422"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

 **Sette opp DLP**

Har du problemer med **at dlp (Data Loss Prevention)** i Office 365 ikke fungerer som forventet? I så fall må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder hva **DLP-policyen** leter etter når den evalueres.
  
Med DLP-policyer kan du identifisere og beskytte sensitiv informasjon i organisasjonen. Hvis du vil konfigurere DLP-policyer, bruker du informasjonen [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Hvilke DLP-retningslinjer ser etter**
  
Når du bruker de **innebygde sensitive informasjonstypene** i sikkerhets- og samsvarssentrene, ser DLP-policyer etter bestemte mønstre og elementer når du oppdager disse sensitive typene.
  
- **Innebygde sensitive informasjonstyper**

    Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager sensitivetypen, kan du se: [Hva de sensitive informasjonstypene ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Egendefinerte sensitive informasjonstyper**

    Hvis du prøver å opprette egendefinerte sensitive informasjonstyper, bruker du følgende artikkel for informasjon om hvordan du oppretter en egendefinert sensitiv type: [Opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Teste en DLP-policy**

Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, bruker du alternativet **Testtype** under **Klassifiseringer** > **Sensitive infotyper**. Hvis du vil ha mer informasjon, kan du se [Teste egendefinerte sensitive informasjonstyper](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Få sensitiv datainnsikt med [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Se bestemte detaljer om hendelsen med en [hendelsesrapport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
