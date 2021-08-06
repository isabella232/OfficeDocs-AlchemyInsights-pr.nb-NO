---
title: Tilbakeskriving av passord fungerer ikke
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999753"
---
# <a name="password-writeback-is-not-working"></a>Tilbakeskriving av passord fungerer ikke

**Jeg har problemer med å konfigurere tilbakeskriving av passord**

- Tilbakeskriving av passord er en premium-funksjon.
- Kontroller at du forstår lisenskravene:
  - Du må ha minst én lisens tilordnet i organisasjonen
  - **Skybrukere –** alle Office 365 (O365) betalt SKU eller Azure AD Basic
  - **Sky- og/eller lokale** brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Hvis du vil lære mer om lisensieringskrav, kan du se [Lisenskrav for selvbetjent tilbakestilling av azure AD-passord](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Du har minst én administratorkonto og én test brukerkonto med en av de riktige lisensene.
- Du må koble Azure AD Koble til til den primære domenekontrolleren Emulator for at tilbakeskriving av passord skal fungere. Du kan konfigurere Azure AD Koble til til å bruke en primær  domenekontroller ved å høyreklikke på egenskapene for Active Directory-synkroniseringskoblingen og deretter **velge Konfigurer katalogpartisjoner**. Derfra ser du  etter delen for tilkoblingsinnstillinger for domenekontrolleren, og merker av for Bruk bare foretrukne **domenekontrollere**.
  > [!NOTE]
  > Hvis den foretrukne DC ikke er en PDC-emulator, vil Azure AD Koble til fortsatt ta kontakt med PDC for tilbakeskriving av passord.
- Tilbakestilling av passord er konfigurert og aktivert i leieren. Hvis du vil ha mer informasjon, kan du se Aktivere brukere [til å tilbakestille Azure AD-passordene sine.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Kontroller at administratorkontoen som brukes til å aktivere passordskriving, er en administratorkonto i skyen (opprettet i Azure AD ikke lokal AD)
- Du har en lokal ad-distribusjon med én eller flere skoger som kjører Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2 med de nyeste oppdateringspakkene installert
- Du har Azure AD Koble til-verktøyet installert, og du har klargjort AD-miljøet for synkronisering til skyen. Før du tester tilbakeskriving av passord, må du først fullføre en fullstendig import og fullstendig synkronisering fra både AD og Azure AD i Azure AD Koble til.
- Hvis du vil ha mer informasjon, kan du se hvordan du gjør en [fullstendig synkronisering og full import i Azure AD Koble til](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Jeg har et problem med tilbakeskriving av passordtilkobling**

1. Last ned og aktiver den nyeste versjonen av [Azure AD Koble til](https://www.microsoft.com/download/details.aspx?id=47594)
2. Brannmurkonfigurasjon: Azure AD Koble til-verktøyet (1.1.443 og nyere) trenger **utgående HTTPS-tilgang** til:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Tillat at inaktive tilkoblinger vedvarer i minst 2–3 minutter

**Jeg har fortsatt problemer med tilbakeskriving av passord**

- Hvis du fremdeles har problemer, kan du prøve å deaktivere og aktivere tilbakeskrivingstjenesten for passord på nytt i Azure AD Koble til-verktøyet
- Hvis du vil ha mer informasjon, kan du se hvordan [du deaktiverer](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) og aktiverer tilbakeskriving av passord på nytt
