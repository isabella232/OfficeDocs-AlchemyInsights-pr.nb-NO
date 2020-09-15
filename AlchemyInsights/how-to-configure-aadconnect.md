---
title: 646 slik konfigurerer du AADConnect
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704498"
---
# <a name="configure-sync-features"></a>Konfigurere synkroniserings funksjoner

Azure AD Connect inkluderer flere funksjoner som er aktivert som standard, eller som du kan aktivere senere. Noen funksjoner krever ytterligere konfigurasjon i bestemte miljøer.

- [Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begrenser at objektene er synkronisert med Azure ad. Som standard er alle brukere, kontakter, grupper og Windows 10-data maskin kontoer synkronisert. Du kan inkludere eller utelate objekter basert på domener, organisasjons enheter eller andre attributter.

- [Passord nummer synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer passord nummeret fra den lokale Active Directory til Azure ad. Dette gjør det mulig for passord behandling på ett sted, men bruker samme passord i lokale og Sky miljøer. Fordi Active Directory er den autoritative kilden, kan du bruke dine egne passord policyer.

- [Selv betjent tilbakestilling av passord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) lar brukere tilbakestille sine egne passord i skyen mens de fremdeles bruker den lokale passord policyen.

- [Bakgrunns skriving for enheter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) lar registrerte enheter i Azure ad skrives tilbake til den lokale Active Directory, slik at de kan brukes til betinget tilgang.

- [Unngå utilsiktede](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) slettinger er aktivert som standard for å forhindre for mange samtidige objekt slettinger (mer enn 500 objekter per synkronisering). Du kan endre denne innstillingen for å oppfylle organisasjonens behov.

- [Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktivert som standard for hurtig installasjoner og hjelper deg med å sikre at din versjon av Azure ad Connect alltid er oppdatert.
