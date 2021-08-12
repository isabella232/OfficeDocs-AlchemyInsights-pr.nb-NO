---
title: 646 Slik konfigurerer du AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963652"
---
# <a name="configure-sync-features"></a>Konfigurere synkroniseringsfunksjoner

Azure AD Koble til inneholder flere funksjoner som er aktivert som standard, eller som du kan aktivere senere. Noen funksjoner krever ekstra konfigurasjon i bestemte miljøer.

- [Filtreringsbegrensninger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objektene synkroniseres med Azure AD. Som standard synkroniseres alle brukere, kontakter, grupper Windows 10 datamaskinkontoer. Du kan inkludere eller utelate objekter basert på domener, OUs eller andre attributter.

- [Synkronisering av hash for passord](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer hash-hash for passord fra den lokale Active Directory til Azure AD. Dette tillater passordbehandling på ett sted, men bruk av samme passord i både lokale miljøer og i skymiljøer. Fordi Active Directory er den autoritative kilden, kan du bruke dine egne passordpolicyer.

- [Selvbetjent tilbakestilling av passord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) gjør det mulig for brukere å tilbakestille sine egne passord i skyen samtidig som de bruker den lokale passordpolicyen.

- [Med tilbakeskriving](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) av enheter kan registrerte enheter i Azure AD skrives tilbake til den lokale Active Directory, slik at de kan brukes for betinget tilgang.

- [Forhindre utilsiktede](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) slettinger er aktivert som standard for å forhindre for mange samtidige slettinger av objekter (mer enn 500 objekter per synkronisering). Du kan endre denne innstillingen for å dekke behovene til organisasjonen.

- [Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktivert som standard for ekspressinstallasjoner og bidrar til å sikre at din versjon av Azure AD Koble til alltid er oppdatert.
