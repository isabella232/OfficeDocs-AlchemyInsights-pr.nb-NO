---
title: Aktiver tilbakeskriving av passord i Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 607e27c883f83b4b29347e764b8f2273cf0f117e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325396"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktiver tilbakeskriving av passord i Azure AD Connect

Hvis du vil aktivere selvbetjent tilbakeskriving av passordtilbakestilling, må du først aktivere alternativet for tilbakeskriving i Azure AD Connect. Følg fremgangsmåten nedenfor fra Azure AD Connect-serveren din:

1. Logg på Azure AD Connect-påloggingsserveren, og start konfigurasjonsveiviseren for **Azure AD Connect**.
2. På **Velkommen**-siden klikker du på **Konfigurer**.
3. Velg **Tilpass synkroniseringsalternativer** på siden **Flere oppgaver**, og klikk deretter på **Neste**.
4. Skriv inn global administratorlegitimasjon for Azure-leieren på siden **Koble til Azure AD**, og klikk deretter på **Neste**.
5. Klikk på **Neste** på **Koble til kataloger** og **domene/OU**-filtreringssider.
6. På siden **Valgfrie funksjoner** merker du av i boksen ved siden av **Tilbakeskriving av passord** og klikker på **Neste**.
7. På siden **Klar for konfigurasjon** klikker du på **Konfigurer** og venter til prosessen er ferdig.
8. Når du ser konfigurasjonen er ferdig, klikker du på **Avslutt**.

Med tilbakeskriving av passord aktivert i Azure AD Connect konfigurerer du Azure AD SSPR for tilbakeskriving.  Hvis du vil aktivere tilbakeskriving av passord i SSPR, kan du fullføre følgende trinn:

1. Logg deg på Azure-portalen ved hjelp av en global administratorkonto.
2. Søk etter og velg **Azure Active Directory**, klikk på **Tilbakestilling av passord**, og klikk deretter på **Lokal integrering**.
3. Angi alternativet for **Tilbakeskrive passord til den lokale katalogen?** til **Ja**.
4. Angi alternativet for **Tillat brukere å låse opp kontoene uten å tilbakestille passordet?** til **Ja**.
5. Når du er klar, klikker du på **Lagre**.

Hvis du vil ha mer informasjon, kan du se [Aktivere tilbakeskriving for selvbetjent passordtilbakestilling i Azure Active Directory til et lokalt miljø](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

**Obs!** Når en administrator tilbakestiller en brukers passord i Azure Portal, skrives passordet tilbake til lokalt hvis brukeren er synkronisert med forbund eller hash for passord. Denne funksjonaliteten krever Azure Premium-lisens (P1 eller P2) og støttes for øyeblikket ikke i administrasjonsportalen for Office.
