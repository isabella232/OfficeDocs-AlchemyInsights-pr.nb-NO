---
title: Eksempel på Microsoft Defender for anti-phishing-policy for Office 365
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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695647"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Eksempel på Microsoft Defender for anti-phishing-policy for Office 365

Disse innstillingene aktiverer en policy kalt *Domene og administrerende direktør.* Denne policyen gir både bruker- og domenebeskyttelse fra representasjon og bruker deretter policyen på alle e-postmeldinger som mottas av brukere i domenet. Legg først til følgende informasjon for å opprette policyen:

- **Navn:** Domene og administrerende **direktør Beskrivelse:** Sikrer at administrerende direktør og domenet ikke representeres.
  **Brukt på:** Velg **mottakerdomene er.** Velg **Velg under Hvilken som helst** av disse, og velg deretter et domene.  Velg **+ Legg til.** Merk av for navnet på domenet i listen (for eksempel contoso.com *),* og velg deretter **Legg til.** Velg **Ferdig.**
- Når policyen er opprettet, kan du finjustere policyen ved å bruke følgende alternativer:
  - **Legg til brukere for å beskytte:** I dette eksemplet legger du til administrerende direktørs e-postadresse, som et minimum.
  - **Legg til domener for å** beskytte: Legg til organisasjonsdomenet som omfatter kontoret til administrerende direktør.
  - **Velg handlinger:** **Hvis** e-post sendes av en representasjonsbruker, velger du Omdiriger melding til en annen e-postadresse, og skriver deretter inn e-postadressen til sikkerhetsadministratoren (for eksempel *securityadmin@contoso.com).* Velg Karantene for Hvis **e-post sendes av et** domene som er representasjon, **i karantene.**
  - **Postboksintelligens:** Dette alternativet velges som standard når du oppretter en ny anti-phishing-policy. La denne innstillingen **være På** for best resultat.
  - **Legge til klarerte avsendere og domener:** I dette eksemplet må du ikke definere noen overstyringer.
- Når du har gjennomgått innstillingene, velger du **Opprett denne policyen eller** **Lagre** etter behov.

Hvis du vil ha mer informasjon, kan du [se anti-phishing-policyer i Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
