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
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960844"
---
# <a name="password-synchronization"></a>Synkronisering av passord

**Synkronisering av hash for passord fungerer ikke i det hele tatt**

Noen vanlige problemer kunder støter på når synkronisering av hash for passord ikke fungerer:

- Active Directory-kontoen som brukes av Azure AD Koble til til å kommunisere  med lokal  Active Directory, får ikke replikere katalogendringer og replikerer katalogendringer Alle tillatelser, som kreves for passordsynkronisering – Du må løse dette ved å gi disse tillatelsene til Active Directory-kontoen.
- Synkronisering av hash for passord deaktiveres etter at  en administrator har endret User Sign-In-metoden fra Passordsynkronisering til et annet alternativ, for eksempel Forbund med **AD FS** i azure AD Koble til-veiviseren – Du kan løse dette ved å aktivere funksjonen for **hash-synkronisering** av passord på nytt i azure AD Koble til-veiviseren.
- Tilkoblingsproblem med lokal Active Directory. Noen domenekontrollere er for eksempel ikke tilgjengelige for Azure AD Koble til, eller [portene](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) som kreves, er blokkert av brannmuren – Du må løse dette ved å sikre at tilkoblingen mellom Azure AD Koble til-serveren og den lokale Active Directory fungerer på riktig måte.
- Azure AD Koble til-serveren er for øyeblikket i oppsamlingsmodus, noe som fører til at serveren ikke får tilgang til hash-ene for passord . Hvis du vil feilsøke problemet, følger du fremgangsmåten som er beskrevet i delen Feilsøke passordsynkronisering med [Azure AD Koble til-synkronisering –](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Ingen passord synkroniseres .

**Synkronisering av hash for passord fungerer ikke for noen av brukerne mine**

1. Hvis du har lagt merke til at hash  for passord ikke synkroniseres for en bruker, kan du bruke feilsøkingsoppgaven i Azure AD-Koble til å undersøke og løse problemet. Utføre følgende oppgaver:

    a. [Kjøre feilsøkingsoppgaven i veiviseren](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Bruk cmdleten for feilsøking til å undersøke problemet med hashsynkronisering av passord for en bestemt bruk](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Det lokale Active Directory User-objektet er aktivert for **Brukeren må endre passord ved neste påloggingsalternativ.** Når dette alternativet er aktivert, tilordnes brukeren et midlertidig passord og blir bedt om å endre passordet ved neste pålogging. Azure AD Koble til synkroniserer ikke midlertidige passord til Azure AD.

Du kan løse problemet ovenfor ved å utføre en av følgende oppgaver:

- Be brukeren om å logge på det lokale programmet (for eksempel Windows skrivebord) og endre passordet. Det nye passordet synkroniseres til Azure AD.
- Be en administrator oppdatere brukerens passord uten å aktivere alternativet Brukeren må endre passord ved neste pålogging **og** dele det nye passordet med brukeren.

3. Det lokale Active Directory User-objektet er **ikke riktig** konfigurert for objektsynkronisering eller passordsynkronisering. Hvis du vil feilsøke dette problemet, følger du fremgangsmåten som er beskrevet i feilsøking av [hashsynkronisering](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)av passord med Azure AD Koble til synkronisering .







