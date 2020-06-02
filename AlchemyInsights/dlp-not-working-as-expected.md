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
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507487"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

 **Sette opp DLP**

Har du problemer med **datatapsforhindring (DLP)** i Office 365 fungerer ikke som forventet? I så fall må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder det **DLP-policyen** ser etter når den evalueres.
  
DLP-policyer lar deg identifisere og beskytte sensitiv informasjon i organisasjonen. Hvis du vil konfigurere DLP-policyer, kan du bruke informasjonen [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Hva DLP-policyer ser etter**
  
Når du bruker de **innebygde sensitive informasjonstypene** i sikkerhets- og samsvarssentrene, ser DLP-policyer etter bestemte mønstre og elementer når du oppdager disse sensitive typene.
  
- **Innebygde sensitive informasjonstyper**

    Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager sensitiv type, kan du se: [Hva de sensitive informasjonstypene ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Egendefinerte sensitive informasjonstyper**

    Hvis du prøver å opprette egendefinerte sensitive informasjonstyper, kan du bruke følgende artikkel for informasjon om hvordan du oppretter en egendefinert sensitiv type: [Opprette en egendefinert sensitiv informasjonstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Teste en DLP-policy**

Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, bruker du alternativet **Testtype** under **Klassifiseringer**Sensitive  >  **informasjonstyper**. Hvis du vil ha mer informasjon, kan du se [Teste egendefinerte sensitive informasjonstyper](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Få sensitiv datainnsikt med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Se spesifikke detaljer om hendelsen med en [hendelsesrapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
