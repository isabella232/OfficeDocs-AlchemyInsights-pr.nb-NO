---
title: 646 hvordan du konfigurerer AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779520"
---
# <a name="configure-sync-features"></a>Konfigurere synkroniseringsfunksjoner

Koble til Azure AD inneholder flere funksjoner som er aktivert som standard, eller som du kan aktivere senere. Noen funksjoner krever mer konfigurasjon i bestemte miljøer.
  
- [Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) grenser objektene synkroniseres Azure AD. Som standard, alle brukere, kontakter, grupper og Windows 10 synkroniseres datamaskinkontoer. Du kan inkludere eller utelate objekter basert på domener, organisasjonsenheter eller andre attributter. 
    
- [Passord hash synkroniseringen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer passord hash-koden fra den lokale Active Directory til Azure AD. Dette gjør at passordadministrasjon på ett sted, men bruk av samme passord i både lokale og sky miljøer. Active Directory er den autoritative kilden, kan du bruke dine egne passordpolicyer for. 
    
- [Self service for å tilbakestille passord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) , lar brukerne tilbakestiller sine egne passord i skyen under fortsatt bruk av den lokale policyen. 
    
- [Enheten writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) tillater registrerte enheter i Azure AD skrives tilbake til den lokale Active Directory slik at de kan brukes for betinget tilgang. 
    
- [Forhindre utilsiktet slettinger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktivert som standard for å unngå for mange samtidige objektet slettinger (mer enn 500 objekter per synkronisering). Du kan endre denne innstillingen for å dekke behovene til organisasjonen. 
    
- [Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktivert som standard for express installasjoner og bidrar til å sikre din versjon av Azure AD koble alltid er oppdatert. 
    

