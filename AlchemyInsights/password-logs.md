---
title: Passordlogger
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527176"
---
# <a name="password-logs"></a>Passordlogger

**Jeg har problemer med tilgang til overvåkingslogger for tilbakestilling av passord**

Utfør følgende trinn for å feilsøke problemer med tilgang til overvåkingslogger for tilbakestilling av passord:

Kontroller at du er autorisert til å vise overvåkingslogger. 

Bare følgende roller godkjennes:
 - Global administrator
 - Sikkerhetsadministrator
 - Sikkerhetsleser

**Jeg vil se alle overvåkingshendelser for tilbakestilling av passord fra det tidspunktet da jeg opprinnelig distribuerte**

Opptil 120 000 hendelser for tilbakestilling/registrering av passord lagres i rapportene for de siste 30 dagene. Denne maksimumsgrensen gjelder for brukergrensesnittet når du laster ned CSV-filen. 1 million hendelser er tilgjengelige via PowerShell.
Hvis du vil ha mer informasjon, kan du se koblingene nedenfor:

- [Selvbetjente hendelser for tilbakestilling av passord fra API-rapporter og -hendelser for Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Slik laster du ned registreringshendelser for tilbakestilling av passord raskt med PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Jeg ønsker å forstå mer om rapporteringsmuligheter for tilbakestilling av passord**

Kontroller hvem som registrerer seg for eller tilbakestiller passord med overvåkingslogger for tilbakestilling av passord for Azure I Azure-portalen under **Brukere og grupper.**
Hvis du vil ha mer informasjon, kan du se følgende koblinger:

- [Oversikt over rapporter om tilbakestilling av passord](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Slik viser du rapporter for tilbakestilling av passord i Azure Portal](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Selvbetjente hendelser for tilbakestilling av passord fra API-rapporter og -hendelser for Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Slik laster du ned registreringshendelser for tilbakestilling av passord raskt med PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


