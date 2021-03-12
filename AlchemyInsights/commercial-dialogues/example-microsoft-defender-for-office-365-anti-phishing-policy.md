---
title: Eksempel på Microsoft Defender for office 365-policy mot phishing
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750791"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Eksempel på Microsoft Defender for office 365-policy mot phishing

Disse innstillingene aktiverer en policy kalt *Domene og ADMINISTRERENDE DIREKTØR.* Denne policyen gir både bruker- og domenebeskyttelse mot representasjon og bruker deretter policyen på all e-post som mottas av brukere i domenet. Først legger du til følgende informasjon for å opprette policyen:

- **Navn:** Beskrivelse av domene **og administrerende direktør**: Sikrer at administrerende direktør og domenet ikke representeres.
  **Brukes på:** Velg **Mottakerdomenet er**. Velg **Velg under Hvilken som** helst av disse , og velg deretter et domene.  Velg **+ Legg til**. Merk av for navnet på domenet i listen (for eksempel contoso.com *),* og velg deretter **Legg til**. Velg **Ferdig**.
- Når policyen er opprettet, kan du finjustere policyen ved hjelp av følgende alternativer:
  - **Legg til brukere for å beskytte:** I dette eksemplet kan du legge til konsernsjefens e-postadresse, som et minimum.
  - **Legg til domener for å beskytte**: Legg til organisasjonsdomenet som inkluderer kontoret til administrerende direktør.
  - **Velg handlinger:** **Hvis** e-post sendes av en representasjonsbruker , velger du Omadresser melding til en annen e-postadresse **,** og deretter skriver du inn e-postadressen til sikkerhetsadministratoren (for eksempel *securityadmin@contoso.com*). For **Hvis e-post sendes av et etterlignet domene**, velger du **Karantene meldingen**.
  - **Postboksintelligens:** Dette alternativet velges som standard når du oppretter en ny phishing-policy. La denne innstillingen **være På** for å få best resultat.
  - **Legg til klarerte avsendere og domener:** I dette eksemplet må du ikke definere noen overstyringer.
- Når du har gått gjennom innstillingene, velger du **Opprett denne policyen** eller **Lagre** etter behov.

Hvis du vil ha mer informasjon, kan du se [Phishing-policyer i Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
