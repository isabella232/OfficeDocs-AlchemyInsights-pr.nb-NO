---
title: 646 Hvordan du konfigurerer AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722572"
---
# <a name="configure-sync-features"></a>Konfigurere synkroniseringsfunksjoner

Azure AD Connect inneholder flere funksjoner som er aktivert som standard, eller som du kan aktivere senere. Noen funksjoner krever ekstra konfigurasjon i bestemte miljøer.

- [Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begrenser objektene synkroniseres til Azure AD. Som standard synkroniseres alle brukere, kontakter, grupper og Windows 10-datamaskinkontoer. Du kan inkludere eller utelate objekter basert på domener, ouer eller andre attributter.

- [Synkronisering av passordhash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer passordhashen fra den lokale Active Directory til Azure AD. Dette tillater passordbehandling på ett sted, men bruk av det samme passordet i både lokale og skymiljøer. Fordi Active Directory er den autoritative kilden, kan du bruke dine egne passordpolicyer.

- [Selvbetjent tilbakestilling av passord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) gjør det mulig for brukere å tilbakestille sine egne passord i skyen mens de fortsatt bruker den lokale passordpolicyen.

- [Enhetswriteback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) gjør at registrerte enheter i Azure AD kan skrives tilbake til den lokale Active Directory, slik at de kan brukes til betinget tilgang.

- [Forhindre utilsiktet sletting](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktivert som standard for å forhindre for mange samtidige objektslettinger (mer enn 500 objekter per synkronisering). Du kan endre denne innstillingen for å dekke behovene til organisasjonen.

- [Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktivert som standard for ekspressinstallasjoner og bidrar til å sikre at din versjon av Azure AD Connect alltid er oppdatert.
