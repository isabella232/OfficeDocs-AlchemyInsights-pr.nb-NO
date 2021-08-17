---
title: Administrere global adresseliste og frakoblet adressebok for organisasjoner
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
- "9002895"
- "5550"
ms.openlocfilehash: c5b73e2dae4d2b98b6af05e147f93a493bac5a88cfcb9ea67c979264aba34ceb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042171"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Administrere global adresseliste (GAL) og frakoblet adressebok (OAB) for organisasjoner

En global adresseliste (GAL) er en liste over e-postaktiverte objekter (en hvilken som helst type mottaker som kan motta en e-postmelding) i organisasjonen. Én GAL blir automatisk opprettet i hver organisasjon. Du kan opprette flere GAL-er til å skille brukere etter organisasjon eller sted, men én enkelt bruker kan bare se og bruke én GAL om gangen.

Enkelte e-postklienter, for eksempel Outlook for Windows, laster ned GAL-en til frakoblet bruk. Dette kalles en frakoblet adressebok (OAB). I Exchange Online oppdateres en OAB bare én gang hver 8. time, og deretter må kundene laste den ned for å oppdatere sin lokale OAB-kopi. Eventuelle endringer av mottakere må først være synlig i GAL for senere å komme med i OAB.

Her er noen vanlige GAL- og OAB-prosedyrer:

- Det kan være en rekke årsaker til at du vil at noen av objektene skal være skjult fra GAL. Se [Skjul mottakere fra adresselister](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Hvis du trenger å gi bestemte brukergrupper tilpassede visninger av organisasjonens GAL, kan du se [Adressebok-policyer i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Opprett en global adresseliste i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), og for å lære hvordan du arbeider med globale tillatelser, kan du se [Adresselister i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Vær oppmerksom på at hvis du oppretter nye GAL-er, vil du kanskje også opprette en ny OAB. Se [prosedyrer for Frakoblet adressebok](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).
