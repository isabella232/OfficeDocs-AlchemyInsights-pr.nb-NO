---
title: Avbryte reservasjonen
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
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931242"
---
# <a name="cancelling-reservation"></a>Avbryte reservasjonen

- **Selvbetjening:** Du kan avbryte eller bytte en reservert forekomst selv ved å bruke [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Velg reservasjon, og klikk på refundere eller bytte. Vær oppmerksom på at du må ha eiertilgang på reservasjonsordren for å bytte eller refundere. Med tilgang til bare reservasjon kan du ikke gå videre med å refundere eller bytte. Spør eieren av reservasjonsordren om å gi deg eiertilgang til reservasjonsordren
- **Byttepolicy:** Du kan bytte reservasjon til en annen reservasjon av samme type – det er **ingen avgifter** på bytte av reservasjon. Den totale forpliktelsen med den nye reservasjonen skal være større enn summen av refusjonsbeløpet for byttet reservasjon og fremtidige månedlige betalinger (hvis aktuelt)
- **Refusjonspolicy:** Summen av refusjonen og de avbrutte fremtidige betalingene kan ikke overskride USD 50 000 i en 12-måneders rullerende vindu. Du må **for øyeblikket ikke betale avgift** på refusjoner, men kanskje på fremtidige refusjoner.  
    **Unntak:** Selvbetjent funksjon for å bytte og avbryte er ikke tilgjengelig for US Government Foretaksavtale-kunder
- Støtte for **API / PS / CLI** er ikke tilgjengelig for kansellering og refusjoner [Selvbetjente bytter og refusjoner for Azure-reservasjoner](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Selvbetjent funksjon for å bytte og avbryte er ikke tilgjengelig for US Government Foretaksavtale-kunder. Andre US Government-abonnementstyper, inkludert bruksbasert og CSP, støttes

Finn ut mer: [Slik behandles retur- og byttetransaksjoner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Finn ut mer: [Bytte- og refusjonspolicyer](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Andre spørsmål: [Gå til reservert forekomst-dokumenter](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Bytte en eksisterende reservert forekomst (selvbetjening)**

Du kan bytte en reservasjon med en annen reservasjon av samme type. DU kan også refundere en reservasjon, opptil USD 50 000 per år, hvis du ikke trenger den lenger. Selvbetjent funksjon for å bytte og avbryte er ikke tilgjengelig for US Government Foretaksavtale-kunder. Andre US Government-abonnementstyper, inkludert bruksbasert og CSP, støttes. Du må ha eiertilgang på reservasjonsordren for å bytte eller refundere en eksisterende reservasjon.

Følgende trinn veileder deg gjennom prosedyren for å fullføre transaksjonen

1. Logg på [Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Velg reservasjonene du vil refundere, og klikk på **Bytt**
2. Velg VM-produktet du vil kjøpe, og skriv inn et tall. Sørg for at den nye kjøpesummen er større enn retursummen[Bestem riktig størrelse før du kjøper](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Gå gjennom og fullfør transaksjonen

**Refusjon for en reservert forekomst**

Hvis du vil refundere en reservasjon, går du til **Reservasjonsinformasjon** og klikker på **Refusjon**

**Proporsjonal refusjon:**

**Eksempler på proporsjonale og minimumskrav for refusjon og bytte**  
Eksempel på forskuddsreservasjon:

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

**Anbefalte dokumenter**

- [Slik behandles retur- og byttetransaksjoner](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Bytte- og refusjonspolicyer](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)