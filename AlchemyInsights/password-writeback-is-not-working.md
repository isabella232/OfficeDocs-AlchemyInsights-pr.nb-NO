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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243517"
---
# <a name="password-writeback-is-not-working"></a>Tilbakeskriving av passord fungerer ikke

**Jeg har problemer med å konfigurere tilbakeskriving av passord**

- Tilbakeskriving av passord er en premiumfunksjon.
- Kontroller at du forstår lisensieringskravene:
  - Du må ha minst én lisens tilordnet i organisasjonen
  - **Bare skybrukere** – alle Office 365 (O365) betalte SKU-er, eller Azure AD Basic
  - **Skybrukere og/eller** lokale brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)
    - Hvis du vil finne ut mer om lisensieringskrav, kan du se Lisensieringskrav [for selvbetjent tilbakestilling av passord for Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Du har minst én administratorkonto og én test brukerkonto med en av de riktige lisensene.
- Du må koble Azure AD Connect til den primære domenekontroller-emulatoren for at tilbakeskriving av passord skal fungere. Du kan konfigurere Azure AD Connect til å bruke  en primær domenekontroller ved å høyreklikke på egenskapene for Active Directory-synkroniseringskontakten og deretter velge **Konfigurer katalogpartisjoner.** Derfra kan du se etter **delen** for tilkoblingsinnstillinger for domenekontrolleren, og merke av i boksen med tittelen Bare **bruke foretrukne domenekontrollere.**
  > [!NOTE]
  > Hvis den foretrukne DC ikke er en PDC-emulator, vil Azure AD Connect fortsatt ta kontakt med PDC for tilbakeskriving av passord.
- Tilbakestilling av passord er konfigurert og aktivert i tenanten din. Hvis du vil ha mer informasjon, kan du [se Aktivere brukere til å tilbakestille Azure AD-passordene sine.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Kontroller at administratorkontoen som brukes til å aktivere passordskriving, er en administratorkonto i skyen (opprettet i Azure AD, ikke lokalt AD)
- Du har en AD-distribusjon med én eller flere skoger lokalt som kjører Windows Server 2008 R2, Windows Server 2012 eller Windows Server 2012 R2 med de nyeste oppdateringspakkene installert
- Du har Azure AD Connect-verktøyet installert, og du har klargjort AD-miljøet for synkronisering til skyen. Før du tester tilbakeskriving av passord, må du først fullføre en fullstendig import og full synkronisering fra både AD og Azure AD i Azure AD Connect.
- Hvis du vil ha mer informasjon, kan du se hvordan du gjør en fullstendig synkronisering [og full import i Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Jeg har et problem med tilkobling med tilbakeskriving av passord**

1. Laste ned og aktivere den nyeste versjonen av [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Brannmurkonfigurasjon: Azure AD Connect-verktøyet (1.1.443 og nyere) trenger **utgående HTTPS-tilgang** til:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Tillat inaktive tilkoblinger å beholde i minst 2–3 minutter

**Jeg har fortsatt problemer med tilbakeskriving av passord**

- Hvis du fremdeles har problemer, kan du prøve å deaktivere og aktivere tilbakeskrivingstjenesten for passord på nytt i Azure AD Connect-verktøyet
- Hvis du vil ha mer informasjon, kan du se hvordan [du deaktiverer og aktiverer tilbakeskriving](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) av passord på nytt
