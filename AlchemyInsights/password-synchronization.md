---
title: Synkronisering av passord
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482040"
---
# <a name="password-synchronization"></a>Synkronisering av passord

**Synkronisering av hash for passord fungerer ikke i det hele tatt**

Her er noen vanlige problemer kundene støter på når synkronisering av hash for passord ikke fungerer:

- Active Directory-kontoen som brukes av Azure AD Connect til  å kommunisere med  lokal Active Directory, får ikke replikat katalogendringer og replikeringskatalogen endrer alle tillatelser, som er nødvendige for passordsynkronisering – du må løse dette ved å gi disse tillatelsene til Active Directory-kontoen.
- Synkronisering av hash for passord deaktiveres når en  administrator har endret Bruker-Sign-In-metoden fra passordsynkronisering til et annet alternativ, for eksempel forbund med **AD FS** i veiviseren for Azure AD Connect . Du kan løse dette ved å aktivere funksjonen for synkronisering av **hash** for passord på nytt i veiviseren azure AD Connect.
- Tilkoblingsproblem med lokal Active Directory. Enkelte domenekontrollere er for eksempel ikke tilgjengelige med Azure AD Connect, eller portene som kreves, [blokkeres](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) av brannmuren . Du må løse dette ved å sikre at tilkoblingen mellom Azure AD Connect-serveren og den lokale Active Directory fungerer på riktig måte.
- Azure AD Connect-serveren er for øyeblikket i feilsøkingsmodus, noe som fører til at serveren ikke får tilgang til hash-passordene . Hvis du vil feilsøke problemet, følger du fremgangsmåten i delen Feilsøke passordsynkronisering med Azure AD Connect-synkronisering – ingen passord [synkroniseres.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

**Synkronisering av hash for passord fungerer ikke for noen av brukerne mine**

1. Hvis du oppdaget at hash for passord ikke  synkroniseres for en bruker, kan du bruke feilsøkingsoppgaven i Azure AD Connect til å undersøke og løse problemet. Utfør følgende oppgaver:

    a. [Kjør feilsøkingsoppgaven i veiviseren](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Bruke cmdleten for feilsøking til å undersøke problemet med hashsynkronisering av passord for en bestemt bruk](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Det lokale Active Directory User-objektet er aktivert for **brukeren, og brukeren må endre passord ved neste påloggingsalternativ.** Når dette alternativet er aktivert, tilordnes brukeren et midlertidig passord, og brukeren blir bedt om å endre passordet ved neste pålogging. Azure AD Connect synkroniserer ikke midlertidige passord til Azure AD.

Du kan løse problemet ovenfor ved å utføre en av følgende oppgaver:

- Be brukeren om å logge på det lokale programmet (for eksempel Windows-skrivebord) og endre passordet. Det nye passordet synkroniseres til Azure AD.
- Be en administrator oppdatere brukerens passord uten å aktivere alternativet Brukeren må endre passordet ved neste pålogging **og** dele det nye passordet med brukeren.

3. Det lokale Active Directory User-objektet **er ikke riktig** konfigurert for objektsynkronisering eller passordsynkronisering. Følg fremgangsmåten i feilsøking av hash-synkronisering av passord med [Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)for å feilsøke dette problemet.







