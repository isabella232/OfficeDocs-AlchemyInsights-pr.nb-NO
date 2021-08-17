---
title: Fakturering for kjøp av reservert forekomst
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
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104029"
---
# <a name="billing-for-reserved-instance-purchase"></a>Fakturering for kjøp av reservert forekomst

Kjøpet av den reserverte forekomsten blir belastet betalingsmetoden som er knyttet til abonnementet du velger på kjøpstidspunktet. Abonnementtypen må være en bedriftsavtale (tilbudsnummer: MS-AZR-0017P), bruksbasert (tilbudsnummer: MS-AZR-0003P), Microsoft-kundeavtale eller CSP.

- Kostnadene trekkes fra registreringens betalingsforpliktelsessaldo eller belastes som overforbruk for et bedriftsabonnement.
- Når det gjelder bruksbasert betaling, faktureres kostnadene til kredittkoret eller fakturabetalingsmetoden på abonnementet

**Avbryte reservasjonen**

- **Selvbetjening:** Du kan avbryte eller bytte en reservert forekomst selv ved å bruke [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Velg reservasjon, og klikk på refundere eller bytte. Vær oppmerksom på at du må ha eiertilgang på reservasjonsordren for å bytte eller refundere. Med tilgang til bare reservasjon kan du ikke gå videre med å refundere eller bytte. Spør eieren av reservasjonsordren om å gi deg eiertilgang til reservasjonsordren
- **Byttepolicy:** Du kan bytte reservasjon til en annen reservasjon av samme type – det er **ingen avgifter** på bytte av reservasjon. Den totale forpliktelsen med den nye reservasjonen skal være større enn summen av refusjonsbeløpet for byttet reservasjon og fremtidige månedlige betalinger (hvis aktuelt)
- **Refusjonspolicy:** Summen av refusjonen og de avbrutte fremtidige betalingene kan ikke overskride USD 50 000 i en 12-måneders rullerende vindu. Du må **for øyeblikket ikke betale avgift** på refusjoner, men kanskje på fremtidige refusjoner.

**Unntak:** Selvbetjent funksjon for å bytte og avbryte er ikke tilgjengelig for US Government Foretaksavtale-kunder

- Støtte for **API / PS / CLI** er ikke tilgjengelig for kansellering og refusjoner [Selvbetjente bytter og refusjoner for Azure-reservasjoner](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selvbetjent funksjon for å bytte og avbryte er ikke tilgjengelig for US Government Foretaksavtale-kunder. Andre US Government-abonnementstyper, inkludert bruksbasert og CSP, støttes

Finn ut mer: [Hvordan retur-](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) og byttetransaksjoner behandles Finn ut [mer:](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Exchange policyer og refusjonspolicyer Andre [spørsmål: Gå til reserverte forekomstdokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Bytte en eksisterende reservert forekomst (selvbetjening)**

Du kan bytte en reservasjon med en annen reservasjon av samme type. DU kan også refundere en reservasjon, opptil USD 50 000 per år, hvis du ikke trenger den lenger. Selvbetjent funksjon for å bytte og avbryte er ikke tilgjengelig for US Government Foretaksavtale-kunder. Andre US Government-abonnementstyper, inkludert bruksbasert og CSP, støttes. Du må ha eiertilgang på reservasjonsordren for å bytte eller refundere en eksisterende reservasjon.

Følgende trinn veileder deg gjennom prosedyren for å fullføre transaksjonen

1.Logg på [Azure-portalen.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Velg reservasjonene du vil refundere, og **klikk Exchange** 2.Velg VM-produktet du vil kjøpe, og skriv inn et antall. Kontroller at den nye innkjøpssummen er mer enn den totale retursummen [Bestem riktig størrelse før du kjøper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Se gjennom og fullfør transaksjonen

**Refusjon for en reservert forekomst**

Hvis du vil refundere en reservasjon, går du til **Reservasjonsinformasjon** og klikker på **Refusjon**

**Proporsjonal refusjon:**

**Pro-rasjoner og eksempler på minimumskrav for refusjon og bytte** Eksempel på forhåndsreservasjon:

- Du kjøper et RI for en 1-årsperiode for USD 120 1. januar
- 7. april må du refundere eller bytte denne reservasjonen.
- Siden reservasjonen har vært tilgjengelig i 97 dager, får du (1-97/365) USD 120 tilbake. (dvs. USD 88,1). Det er for øyeblikket ingen avgifter på refusjoner
- Hvis du bytter, må det nye kjøpet være på mer enn USD 88,1
- Det er ingen avgifter på refusjoner for øyeblikket

**Eksempel på faktueringsplanreservasjon:**

- Du kjøper et RI for en 1-årsperiode for USD 10 per måned
- 7. april må du refundere eller bytte denne reservasjonen.
- Siden forrige betaling var for 7 dager siden, får du (1-7/31) * USD 10 tilbake. (dvs. USD 7,74).
- Fremtidige betalinger som er avbrutt er USD 80. Det er for øyeblikket ingen avgifter på refusjoner
- Denne kanselleringen vil trekke fra USD 87,74 fra refusjonsgrensen på USD 50 000
- Hvis du bytter, må totalverdien på det nye kjøpet være mer enn USD 87,74

**Kan ikke se fakturaen for den siste faktureringsperioden**

Noen mulige årsaker til at du kanskje ikke ser en faktura:

- Du har et månedlig kredittbeløp med abonnementet som du ikke har overskredet, eller du har en gratis prøveperiode. En faktura genereres bare når du skylder penger
- Det er mindre enn 30 dager fra dagen du abonnerer på Azure
- Fakturaen er ikke generert ennå. Vent til slutten av faktureringsperioden
- Hvis du ikke er kontoadministrator, kan det hende at eldre fakturaer ikke er tilgjengelige for deg

**Last ned fakturaen fra Azure-portalen (.pdf)**

- Velg abonnementet ditt fra [Abonnementer-siden](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i Azure Portal som [en bruker med tilgang til fakturaer](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Velg **fakturaer**
- Klikk **Last ned faktura** for å vise en kopi av PDF-fakturaen. Hvis det står **Ikke tilgjengelig**, kan du se Hvorfor ser jeg ikke en faktura for den [siste faktureringsperioden?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Motta fakturaen via e-post (.pdf)**

- Velg abonnementet på [Abonnementer-siden.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Klikk **Fakturaer og** send fakturaen på e-post
- Klikk **på Meld deg på** og godta vilkårene. Du må melde deg på for hvert abonnement du eier

Obs! Hvis du ikke får en e-postmelding etter å ha fulgt trinnene, må du kontrollere at e-postadressen din er riktig i kommunikasjonsinnstillingene [på profilen din](https://account.windowsazure.com/profile)

**Last ned bruksdataene fra Azure-portalen**

- Logg deg på [Azure-kontosenteret](https://account.windowsazure.com/Subscriptions) som [kontoadministrator](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Velg abonnementet du vil finne faktura- og bruksinformasjonen for
- Velg **Faktureringslogg**
- Velg **Vis gjeldende kontoutdrag** for å se et anslag over kostnadene på tidspunktet da estimatet ble generert
- Velg **Last ned bruk** for å laste ned de daglige bruksdataene som en CSV-fil. Hvis du ser to tilgjengelige versjoner, kan du laste ned versjon 2

Andre spørsmål: [Gå til reservert forekomst-dokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Anbefalte dokumenter**

- [Grunnleggende om fakturering](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå hvordan rabatten for reservert forekomst brukes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Laste ned eller vise faktureringsfakturaen for Azure og data om daglig bruk](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå hvordan rabatten for reservert forekomst brukes](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå bruk av reservert forekomst for pay-As-You-Go-abonnementet](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Forstå bruk av reservert forekomst for enterprise-registreringen](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows programvarekostnader som ikke er inkludert i reserverte forekomster](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Reserverte forekomster i Partner Central Leverandør av skyløsninger (CSP)-program](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)