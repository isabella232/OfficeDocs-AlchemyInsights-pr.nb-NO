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
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679702"
---
# <a name="dlp-not-working-as-expected"></a>DLP fungerer ikke som forventet

**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.

 **Konfigurere DLP**

Har du problemer med hindring av datatap **(DLP)** i Office 365 fungerer ikke som forventet? Hvis det er tilfelle, må du kontrollere at **DLP-policyen** er riktig konfigurert, og at dataene inneholder hva **DLP-policyen** ser ut når det evalueres.
  
Policyer for DLP lar deg identifisere og beskytte sensitiv informasjon i organisasjonen. Hvis du vil konfigurere policyer for hindring av tap, kan du bruke informasjonen [her](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Hvilke DLP-policyer ser etter**
  
Når du bruker de **innebygde sensitive informasjons typene** i sikkerhets-og samsvars senteret, ser DLP-policyer for bestemte mønstre og elementer når de oppdager disse sensitive typene.
  
- **Innebygde sensitive informasjons typer**

    Hvis du vil ha informasjon om de innebygde sensitive typene og hva en DLP-policy ser etter når du oppdager den sensitive typen, kan du se: [hva de sensitive informasjons typene ser ut for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Egen definerte sensitive informasjons typer**

    Hvis du prøver å opprette egen definerte sensitive informasjons typer, bruker du følgende artikkel for å få informasjon om hvordan du oppretter en egen definert sensitiv type: [opprette en egen definert sensitiv informasjons type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Teste en DLP-policy**

Hvis du vil teste dataene med en innebygd eller egen definert, sensitiv informasjons type, bruker du **test type** alternativet under **klassifiseringer**av  >  **sensitive informasjons typer**. Hvis du vil ha mer informasjon, kan du se [teste egen definerte sensitive informasjons typer](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapporter**
  
- Få sensitive data innsikt med [DLP-rapporter.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Se bestemte detaljer om hendelsen med en [hendelses rapport](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
