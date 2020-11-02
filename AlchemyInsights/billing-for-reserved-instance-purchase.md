---
title: Fakturering for å kjøpe reservert forekomst
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823164"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturering for å kjøpe reservert forekomst

Det reserverte forekomst innkjøpet belastes betalings metoden knyttet til abonnementet du velger på kjøps tidspunktet. Abonnements typen må være en Enterprise Agreement (tilbuds nummer: MS-AZR-0017P), Betal etter hvert-(tilbuds nummer: MS-AZR-0003P), Microsoft Customer Agreement eller CSP.

- For et bedrifts abonnement trekkes kostnadene fra registreringens penge forpliktelses saldo eller belastet som over
- For Betal etter hvert-abonnement faktureres kostnadene til kreditt kortet eller betalings metoden for fakturaer i abonnementet

**Kansellere reservasjon**

- **Self-Service:** Du kan avbryte eller utveksle en reservert forekomst selv om du bruker [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Velg reservasjonen, og klikk på refusjon eller Exchange. Vær oppmerksom på at du må ha eier tilgang til reservasjons ordren til Exchange eller refusjon. Bare tilgang til reservasjonen vil ikke la deg fortsette med refusjon eller Exchange. Be eieren av reservasjons ordren om å gi deg eier tilgang til reservasjons ordren
- **Exchange-policy:** Du kan utveksle en reservasjon for en annen reservasjon av samme type – det er **ingen straffer** om reserverings utveksling. Den totale forpliktelsen med ny reservasjon må være større enn summen av beløp som er omsluttet av prochanged reservat ion, og de månedlige betalings betalingene (Hvis dette gjelder)
- **Refusjons policy:** Summen av refundering og annullerte fremtidige betalinger kan ikke overskride $50 000 KRONER i et rullende vindu på 12 måneder. Vi **lader for øyeblikket ikke noen straffer** på refunderinger, men kan belaste det på fremtidige tilbake betalinger

**Unntak:** Selv betjent Exchange og Cancel-funksjonen er ikke tilgjengelig for amerikanske Enterprise Agreement-kunder

- Støtte for **API/PS/CLI** er ikke tilgjengelig for annulleringer og refusjoner [selv betjening og refusjon for Azure reserveringer](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selv betjent Exchange og Cancel-funksjonen er ikke tilgjengelig for amerikanske Enterprise Agreement-kunder. Andre US-myndighets abonnements typer, inkludert Betal etter hvert-og kryptografi tjeneste støttes

Finn ut mer: [hvordan retur-og Exchange-transaksjoner behandles](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Finn ut mer: [policyer for Exchange og refusjon](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) andre spørsmål: [gå til reserverte forekomst dokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Utveksle en eksisterende reservert forekomst (selv betjening)**

Du kan utveksle en reservasjon for en annen reservasjon av samme type. Du kan også refundere en reservasjon på opptil $50 000 KRONER per år hvis du ikke trenger den lenger. Selv betjent Exchange og Cancel-funksjonen er ikke tilgjengelig for amerikanske Enterprise Agreement-kunder. Andre US-offentlige abonnements typer, inkludert Betal etter hvert-og kryptografi tjeneste støttes. Du må ha eier tilgang til reservasjons ordren for å kunne utveksle eller refundere en eksisterende reservasjon.

Følgende Fremgangs måte fører til hvordan du kan fullføre transaksjonen

1. Logg deg på [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Velg reservasjonene du vil refundere, og klikk **Exchange** 2. Velg det virtuelle produktet du vil kjøpe, og skriv inn et antall. Kontroller at den nye kjøps summen er mer enn den returnerte summen [avgjør riktig størrelse før du kjøper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. se gjennom og Fullfør transaksjonen

**Refusjon for en reservert forekomst**

Hvis du vil refundere en reservasjon, går du til **reservasjons detaljer** og klikker **refusjon**

**Pro-klassifisert for pengene:**

**Eksempler på forhold og minimums krav for refusjon og utveksling** Forskudds reservasjon, eksempel:

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

**Kan ikke se fakturaen for den siste fakturerings perioden**

Noen mulige årsaker til at du kanskje ikke ser en faktura:

- Du har et månedlig kredit beløp med abonnementet du ikke har overskredet, eller du har en gratis prøve periode. En faktura genereres bare når du skylder penger
- Det er mindre enn 30 dager fra dagen du abonnerer på Azure
- Fakturaen er ennå ikke generert. Vente til slutten av fakturerings perioden
- Hvis du ikke er konto administrator, kan det hende at eldre fakturaer ikke er tilgjengelige for deg

**Last ned fakturaen fra Azure-portalen (PDF)**

- Velg abonnementet fra [abonnementer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) -siden i Azure-portalen som [en bruker med tilgang til fakturaer](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Velg **fakturaer**
- Klikk **Last ned faktura** for å vise en kopi av PDF-fakturaen. Hvis det **ikke er tilgjengelig** , kan du se [Hvorfor kan jeg ikke se en faktura for den siste fakturerings perioden?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Motta fakturaen i e-post (PDF)**

- Velg abonnementet ditt fra [abonnementer](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) -siden. Klikk **fakturaer** og send deretter e-post til fakturaen min
- Klikk **på Velg i** og godta vilkårene. Du må velge for hvert abonnement du eier

Obs! hvis du ikke får en e-post når du følger trinnene, må du kontrollere at e-postadressen din er riktig i [kommunikasjons innstillingene i profilen din](https://account.windowsazure.com/profile)

**Last ned bruks dataene fra Azure-portalen**

- Logg på [Azure Account Center](https://account.windowsazure.com/Subscriptions) som [konto administrator](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Velg abonnementet du vil ha informasjon om faktura og bruk
- Velg **fakturerings Logg**
- Velg **Vis gjeldende utdrag** for å se en beregning av kostnadene dine på det tidspunktet estimatet ble generert
- Velg **Last ned bruk** for å laste ned de daglige bruks dataene som en CSV-fil. Hvis du ser to versjoner tilgjengelig, kan du laste ned versjon 2

Andre spørsmål: [gå til reserverte forekomst dokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Anbefalte dokumenter**

- [Grunnleggende om fakturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå hvordan rabatten for reservert forekomst brukes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Last ned eller Vis faktura-og daglig bruks data for Azure-fakturering](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå hvordan rabatten for reservert forekomst brukes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå reservert forekomst av bruk av abonnementet for Betal etter hvert](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå reservert forekomst av bruk av bedrifts registrering](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Program vare kostnader i Windows som ikke er inkludert i reserverte forekomster](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserverte forekomster i partner sentral Sky løsning leverandør (CSP) program](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)