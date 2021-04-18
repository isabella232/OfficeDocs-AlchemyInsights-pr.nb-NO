---
title: Opprette en delingspolicy for å tillate brukerne å dele kalenderen med personer utenfor organisasjonen
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
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816281"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a>Opprette en delingspolicy for å tillate brukerne å dele kalenderen med personer utenfor organisasjonen

1. Gå til **Administrator** > **Exchange** fra instrumentbordet i administrasjonssenteret for Microsoft 365.
2. Gå til **organisasjon** > **deling**.
3. Klikk på **Ny** i listevisning under **Individuell deling**.
4. Skriv inn et egendefinert navn for delingspolicyen i **policynavn**-boksen i **ny delingspolicy**.
5. Klikk på **Legg til** for å definere delingsregler for policyen.
6. Velg ett av følgende alternativer i **delingsregel**, for å angi domenene du vil dele med:
    - **Dele med alle domener**
    - **Dele med et bestemt domene**
8. Hvis du velger **Dele med et bestemt domene**, skriver du inn navnet på domenet du vil dele med. Hvis du trenger å skrive inn mer enn ett domene for denne delingspolicyen, lagrer du innstillingene for det første domenet, og redigerer deretter delingsreglene for å legge til flere domener.
9. Hvis du vil angi informasjonen som kan deles, merker du av for **Del kalendermappe**, og velger deretter ett av følgende alternativer:
    - **Informasjon om ledig/opptatt i kalenderen bare med tidspunkt**
    - **Informasjon om ledig/opptatt i kalenderen med tidspunkt, emne og sted**
    - **All avtaleinformasjon i kalenderen, inkludert tidspunkt, emne, sted og tittel**
11. Klikk på **lagre** for å angi reglene i delingspolicyen.
12. Hvis du vil angi denne delingspolicyen som den nye standard delingspolicyen for alle brukerne i organisasjonen, merker du av for **Gjør denne policyen til standard delingspolicy**.
13. Klikk på **lagre** for å opprette delingspolicyen.  

**For full forståelse av dette emnet kan du lese:**

- [Opprette en delingspolicy i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [Bruke en delingspolicy på postbokser i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [Endre, deaktivere eller fjerne en delingspolicy i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)