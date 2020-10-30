---
title: Kansellere reservasjon
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807995"
---
# <a name="cancelling-reservation"></a>Kansellere reservasjon

- **Self-Service:** Du kan avbryte eller utveksle en reservert forekomst selv om du bruker [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Velg reservasjonen, og klikk på refusjon eller Exchange. Vær oppmerksom på at du må ha eier tilgang til reservasjons ordren til Exchange eller refusjon. Bare tilgang til reservasjonen vil ikke la deg fortsette med refusjon eller Exchange. Be eieren av reservasjons ordren om å gi deg eier tilgang til reservasjons ordren
- **Exchange-policy:** Du kan utveksle en reservasjon for en annen reservasjon av samme type – det er **ingen straffer** om reserverings utveksling. Den totale forpliktelsen med ny reservasjon må være større enn summen av beløp som er omsluttet av prochanged reservat ion, og de månedlige betalings betalingene (Hvis dette gjelder)
- **Refusjons policy:** Summen av refundering og annullerte fremtidige betalinger kan ikke overskride $50 000 KRONER i et rullende vindu på 12 måneder. Vi **lader for øyeblikket ikke noen straffer** på refunderinger, men kan belaste det på fremtidige tilbake betalinger  
    **Unntak:** Selv betjent Exchange og Cancel-funksjonen er ikke tilgjengelig for amerikanske Enterprise Agreement-kunder
- Støtte for **API/PS/CLI** er ikke tilgjengelig for annulleringer og refusjoner [selv betjening og refusjon for Azure reserveringer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selv betjent Exchange og Cancel-funksjonen er ikke tilgjengelig for amerikanske Enterprise Agreement-kunder. Andre US-myndighets abonnements typer, inkludert Betal etter hvert-og kryptografi tjeneste støttes

Finn ut mer: [hvordan retur-og Exchange-transaksjoner behandles](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Finn ut mer: [policyer for Exchange og refusjon](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Andre spørsmål: [gå til reserverte forekomst dokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Utveksle en eksisterende reservert forekomst (selv betjening)**

Du kan utveksle en reservasjon for en annen reservasjon av samme type. Du kan også refundere en reservasjon på opptil $50 000 KRONER per år hvis du ikke trenger den lenger. Selv betjent Exchange og Cancel-funksjonen er ikke tilgjengelig for amerikanske Enterprise Agreement-kunder. Andre US-offentlige abonnements typer, inkludert Betal etter hvert-og kryptografi tjeneste støttes. Du må ha eier tilgang til reservasjons ordren for å kunne utveksle eller refundere en eksisterende reservasjon.

Følgende Fremgangs måte fører til hvordan du kan fullføre transaksjonen

1. Logg på Azure- [portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Velg reservasjonene du vil refundere, og klikk på **Exchange**
2. Velg VM-produktet du vil kjøpe, og skriv inn et antall. Kontroller at det nye kjøps totalen er mer enn den returnerte summen [avgjør riktig størrelse før du kjøper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Se gjennom og Fullfør transaksjonen

**Refusjon for en reservert forekomst**

Hvis du vil refundere en reservasjon, går du til **reservasjons detaljer** og klikker **refusjon**

**Pro-klassifisert for pengene:**

**Eksempler på forhold og minimums krav for refusjon og utveksling**  
Forskudds reservasjon, eksempel:

- Du kjøper en langsiktig RI for $120 på 1. januar
- I syvende sjuende vil du refundere eller utveksle denne reservasjonen
- Siden reservasjonen er live i 97 dager, får du (1-97/365) * $120 tilbake. (for eksempel $88,1). Det er for øyeblikket ingen straff for refunderinger
- Hvis du utveksler, må det nye kjøpet være større enn $88,1
- Det er ingen straff for påfylling for øyeblikket

**Eksempel på reservasjon av fakturerings plan:**

- Du kjøper en langsiktig RI for $10 per måned
- I syvende sjuende vil du refundere eller utveksle denne reservasjonen
- Siden den siste betalingen skjedde 7 dager, får du (1-7/31) * $10 tilbake. (for eksempel $7,74)
- Fremtidige betalinger som ble avbrutt er $80. Det er for øyeblikket ingen straff for refunderinger
- Denne annulleringen vil trekke $87,74 fra deg er grensen på $50 000-refundering
- Hvis du utveksler, må den totale verdien for nytt Kjøp være større enn $87,74

**Anbefalte dokumenter**

- [Slik behandles retur-og Exchange-transaksjoner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Policyer for Exchange og refusjon](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)