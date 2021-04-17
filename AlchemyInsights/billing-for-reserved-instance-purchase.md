---
title: Fakturering for reservert forekomstkjøp
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820331"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturering for reservert forekomstkjøp

Det reserverte forekomstkjøpet belastes betalingsmåten som er knyttet til abonnementet du valgte på kjøpstidspunktet. Abonnementstypen må være en bedriftsavtale (tilbudsnummer: MS-AZR-0017P), Pay-As-You-Go (tilbudsnummer: MS-AZR-0003P), Microsofts kundeavtale eller CSP.

- For et bedriftsabonnement trekkes avgiftene fra registreringens pengeforpliktelsessaldo eller belastes som overtid
- For pay-As-You-Go-abonnementet faktureres belastningene til kredittkortet eller fakturabetalingsmetoden på abonnementet

**Kansellering av reservasjon**

- **Selvbetjening:** Du kan avbryte eller utveksle en reservert forekomst selv ved hjelp av [Azure Portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Velg reservasjonen, og klikk på refusjon eller bytte. Vær oppmerksom på at du må ha eiertilgang på reservasjonsordren for å bytte eller refundere. Tilgang til bare reservasjonen lar deg ikke fortsette med refusjon eller bytte. Be eieren av reservasjonsordren om å gi deg eiertilgang til reservasjonsordren
- **Exchange-policy:** Du kan bytte en reservasjon for en annen reservasjon av samme type – det er ingen bøter på **reservasjonsbytte.** Den totale forpliktelsen med ny reservasjon bør være større enn summen av den byttede reservasjonens refusjonsbeløp og fremtidige månedlige innbetalinger (hvis aktuelt)
- **Refusjonspolicy:** Summen av refusjonen og de kansellerte fremtidige innbetalingene kan ikke overskride USD 50 000 i et 12-måneders rullende vindu. Vi **belaster for øyeblikket ikke** refusjonsgebyrer, men kan belaste den for fremtidige refusjoner

**Unntak:** Selvbetjent bytte- og annulleringsfunksjonalitet er ikke tilgjengelig for kunder med foretaksavtale for amerikanske myndigheter

- **API/PS/CLI-støtte** er ikke tilgjengelig for kansellering og refusjoner av selvbetjente bytter og [refusjoner for Azure-reservasjoner](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selvbetjent bytte- og annulleringsfunksjonalitet er ikke tilgjengelig for kunder med enterprise-avtale for amerikanske myndigheter. Andre abonnementstyper for amerikanske myndigheter, inkludert Pay-As-You-Go og CSP, støttes

Finn ut mer: [Hvordan retur-](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) og byttetransaksjoner behandles Finn ut mer: [Exchange-](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) og refusjonspolicyer Andre [spørsmål: Gå til reserverte forekomstdokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange an existing reserved instance (Self-service)**

Du kan bytte en reservasjon for en annen reservasjon av samme type. Du kan også refundere en reservasjon, opptil USD 50 000 per år, hvis du ikke lenger trenger den. Selvbetjent bytte- og annulleringsfunksjonalitet er ikke tilgjengelig for kunder med enterprise-avtale for amerikanske myndigheter. Andre abonnementstyper for amerikanske myndigheter, inkludert Pay-As-You-Go og CSP, støttes. Du må ha eiertilgang på reservasjonsordren for å bytte eller refundere en eksisterende reservasjon.

Fremgangsmåten nedenfor viser fremgangsmåten for å fullføre transaksjonen

1.Logg på [Azure-portalen.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Velg reservasjonene du vil refundere, og klikk **Exchange** 2.Velg VM-produktet du vil kjøpe, og skriv inn et antall. Kontroller at den nye innkjøpssummen er mer enn den totale retursummen [Bestem riktig størrelse før du kjøper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Se gjennom og fullfør transaksjonen

**Refusjon for en reservert forekomst**

Hvis du vil refundere en reservasjon, går du til **Reservasjonsdetaljer** og klikker **Refusjon**

**Pro-rated refundering:**

**Eksempler på prorasjons- og minimumskrav for refusjon og bytte** Eksempel på forhåndsreservasjon:

- Du kjøper en ettårsperiode RI for KR 120 den 1. januar
- 7. april vil du refundere eller bytte denne reservasjonen
- Siden reservasjonen har vært live i 97 dager, får du (1-97/365) * $ 120 tilbake. (det vil si $ 88,1). Det er for øyeblikket ingen refusjonsgebyr
- Hvis du bytter, bør det nye kjøpet være større enn USD 88,1
- Det er for øyeblikket ingen refusjonsgebyr

**Eksempel på reservasjon av faktureringsplan:**

- Du kjøper en ettårsperiode ri for $ 10 per måned
- 7. april vil du refundere eller bytte denne reservasjonen
- Siden den siste betalingen skjedde 7 dager, får du (1-7/31) * $ 10 tilbake. (det vil si $ 7,74)
- De fremtidige innbetalingene som kanselleres, er $ 80. Det er for øyeblikket ingen refusjonsgebyr
- Denne kanselleringen trekker fra $87,74 fra deg som refusjonsgrense på USD 50 000
- Hvis du bytter, bør den totale verdien av nytt kjøp være større enn $87,74

**Kan ikke se fakturaen for den siste faktureringsperioden**

Noen mulige årsaker til at du kanskje ikke ser en faktura:

- Du har et månedlig kredittbeløp med abonnementet som du ikke har overskredet, eller du har en gratis prøveperiode. En faktura genereres bare når du skylder penger
- Det er mindre enn 30 dager fra dagen du abonnerer på Azure
- Fakturaen er ikke generert ennå. Vent til slutten av faktureringsperioden
- Hvis du ikke er kontoadministrator, kan det hende at eldre fakturaer ikke er tilgjengelige for deg

**Last ned fakturaen fra Azure Portal (PDF)**

- Velg abonnementet ditt fra [Abonnementer-siden](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure Portal som [en bruker med tilgang til fakturaer](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Velg **fakturaer**
- Klikk **Last ned faktura** for å vise en kopi av PDF-fakturaen. Hvis det står **Ikke tilgjengelig**, kan du se Hvorfor ser jeg ikke en faktura for den [siste faktureringsperioden?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Motta fakturaen via e-post (PDF)**

- Velg abonnementet på [Abonnementer-siden.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Klikk **Fakturaer og** send fakturaen på e-post
- Klikk **på Meld deg på** og godta vilkårene. Du må melde deg på for hvert abonnement du eier

Obs! Hvis du ikke får en e-postmelding etter å ha fulgt trinnene, må du kontrollere at e-postadressen din er riktig i kommunikasjonsinnstillingene [på profilen din](https://account.windowsazure.com/profile)

**Last ned bruksdataene fra Azure-portalen**

- Logg deg på [Azure-kontosenteret](https://account.windowsazure.com/Subscriptions) som [kontoadministrator](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Velg abonnementet du vil finne faktura- og bruksinformasjonen for
- Velg **Faktureringslogg**
- Velg **Vis gjeldende kontoutdrag** for å se et anslag over kostnadene på tidspunktet da estimatet ble generert
- Velg **Last ned bruk** for å laste ned de daglige bruksdataene som en CSV-fil. Hvis du ser to tilgjengelige versjoner, kan du laste ned versjon 2

Andre spørsmål: [Gå til reserverte forekomstdokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Anbefalte dokumenter**

- [Grunnleggende om fakturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå hvordan rabatten for reservert forekomst brukes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Laste ned eller vise faktureringsfakturaen for Azure og data om daglig bruk](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå hvordan rabatten for reservert forekomst brukes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå bruk av reservert forekomst for pay-As-You-Go-abonnementet](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå bruk av reservert forekomst for enterprise-registreringen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows-programvarekostnader som ikke er inkludert i reserverte forekomster](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserverte forekomster i Partner Central Cloud Solution Provider (CSP)-program](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)