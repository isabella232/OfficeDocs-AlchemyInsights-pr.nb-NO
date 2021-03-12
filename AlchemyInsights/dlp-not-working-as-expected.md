---
title: DLP fungerer ikke som forventet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707819"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

 **Konfigurere DLP**

Har du problemer med hindring av **tap av data (DLP)** i Office 365, fungerer ikke som forventet? Hvis det er det, må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder det **DLP-policyen** ser etter når den evalueres.
  
Med DLP-policyer kan du identifisere og beskytte sensitiv informasjon i organisasjonen. Bruk informasjonen her for å [](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)konfigurere DLP-policyer.
  
 **Hvilke DLP-policyer ser etter**
  
Når du bruker de **innebygde sensitive** informasjonstypene i sikkerhets- og samsvarssentrene, ser DLP-policyer etter bestemte mønstre og elementer når disse sensitive typene oppdages.
  
- **Innebygde typer sensitiv informasjon**

    Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager sensitive typer, kan du se: Hva de [sensitive informasjonstypene ser etter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Egendefinerte sensitive informasjonstyper**

    Hvis du prøver å opprette egendefinerte sensitive informasjonstyper, kan du bruke følgende artikkel for informasjon om hvordan du oppretter en egendefinert sensitiv type: Opprette en egendefinert [sensitiv informasjonstype.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Teste en DLP-policy**

Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, kan du bruke **alternativet Testtype** under **Klassifiseringer,** sensitive  >  **informasjonstyper.** Hvis du vil ha mer informasjon, [kan du se Teste egendefinerte sensitive informasjonstyper.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Rapporter**
  
- Få sensitiv datainnsikt med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Se spesifikke detaljer om hendelsen med en [hendelsesrapport.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
