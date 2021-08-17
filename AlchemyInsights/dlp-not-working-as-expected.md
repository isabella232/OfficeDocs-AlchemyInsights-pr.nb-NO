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
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079711"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

 **Konfigurere DLP**

Har du problemer med **datatapsforhindring (DLP)** i Office 365 fungerer ikke som forventet? Hvis dette er det, må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder det **DLP-policyen** ser etter når den evalueres.
  
Med DLP-policyer kan du identifisere og beskytte sensitiv informasjon i organisasjonen. Hvis du vil konfigurere DLP-policyer, bruker du informasjonen [her](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Hvilke DLP-policyer ser etter**
  
Når du bruker de **innebygde** sensitive informasjonstypene i sentre for sikkerhet og samsvar, ser DLP-policyer etter bestemte mønstre og elementer når du oppdager disse sensitive typene.
  
- **Innebygde typer sensitiv informasjon**

    Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager den sensitive typen, kan du se: Hvilke sensitive [informasjonstyper ser etter](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Egendefinerte sensitive informasjonstyper**

    Hvis du prøver å opprette egendefinerte sensitive informasjonstyper, kan du bruke følgende artikkel for informasjon om hvordan du oppretter en egendefinert sensitiv type: Opprette en egendefinert [sensitiv informasjonstype](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Teste en DLP-policy**

Hvis du vil teste dataene med en innebygd eller egendefinert sensitiv informasjonstype, bruker du alternativet **Testtype** under **Klassifiseringer**  >  **Sensitive informasjonstyper**. Hvis du vil ha mer informasjon, [kan du se Teste egendefinerte sensitive informasjonstyper](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Få sensitive datainnsikter med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Se spesifikke detaljer om hendelsen med en [hendelsesrapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
