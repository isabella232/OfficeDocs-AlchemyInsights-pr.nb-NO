---
title: Brukeren får feil AADSTS7000112 Yammer er deaktivert
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198365"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Brukeren får feil AADSTS7000112 Yammer er deaktivert

Hvis du får feilmeldingen "AADSTS7000112: Programmet '00000005-0000-0ff1-ce00-00000000000'(Yammer) er deaktivert", finnes det et problem med tjenestehovedstolen i Azure AD. En administrator kan ha deaktivert tjenestekontohaveren for å blokkere tilgangen til Yammer.

Deaktivering av servicekontohaveren anbefales ikke og kan forårsake flere problemer. Hvis du vil ha mer informasjon om den støttede tilnærmingen for å blokkere brukertilgang til Yammer, kan du se [Deaktivere Yammer-tilgang for Microsoft 365-brukere](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Slik løser du dette problemet i Azure Portal og gjenoppretter brukertilgang til Yammer:

1.  Åpne Azure Active Directory-siden, og velg **Enterprise-programmer** under **Behandle** i venstre navigasjonsrute.
3.  Skriv inn **Office 365 Yammer** i søkeboksen, og velg programnavnet for å åpne innstillinger.
4.  Velg **Egenskaper** under **Behandle** i navigasjonsruten til venstre.
5.  Angi verdien for Aktivert for brukere til **Yes**å logge **Save** **på?**
6.  Logg på Yammer på nytt. Det kan hende du må slette informasjonskapsler.

Du kan også kjøre PowerShell-kommandoer for å angi verdien. Hvis du vil ha mer informasjon, kan du se ["Beklager, men vi har problemer med å logge deg på" feil når du klikker Yammer-flisen i Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 