---
title: Aktivere kostnads styring
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677741"
---
# <a name="enable-cost-management"></a>Aktivere kostnads styring

**Hva er kostnadene deaktivert for organisasjonen?**

Organisasjoner som bruker Enterprise Agreement (EA) eller MCA-kontoer (Microsoft Customer Agreement), kan deaktivere tilgang til kostnads informasjon og pris informasjon.

Når du logger deg på Azure-portalen, kan de bruke fakturerings-APIene til å få fakturaer i en programmatisk (når det er registrert) og bruks detaljer.

**Slik tillater du at flere brukere får tilgang til fakturaer**

1. Gå til **abonnements blad** i Azure-portalen.
2. Velg **fakturaer** og deretter **tilgang til fakturaer**.
3. Slå på Access, etterfulgt av endringer, slik at brukere i abonnements relaterte roller kan laste ned fakturaer.

> [!NOTE]
> Konto administratoren kan også konfigurere til å få fakturaer sendt via e-post. Hvis du vil ha mer informasjon, kan du se [få fakturaen i e-post](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Slik legger du til brukere i rollen som fakturerings leser**

1. Gå til **abonnements blad** i Azure-portalen.
2. Velg **tilgangs kontroll (iam)** , og klikk deretter **Legg til**.
3. Velg **fakturerings leser** på siden **Velg en rolle** .
4. Skriv inn e-postadressen til brukeren du vil invitere, og klikk deretter **OK** for å sende invitasjonen.
5. Følg instruksjonene som er oppgitt i invitasjons-e-post for å logge på som en fakturerings leser. Hvis du vil ha mer informasjon, kan du se [gi tilgang til fakturering](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Anbefalte dokumenter**

- [Aktiver DA og AO visninger via Enterprise Portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kostnader som er inkludert i kostnads styring](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Støttet Microsoft Azure-tilbud](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Se gjennom kostnader i kostnads analyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Gi tilgang til fakturerings informasjon](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kontrollere tilgang til en Microsoft-kunde avtale](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






