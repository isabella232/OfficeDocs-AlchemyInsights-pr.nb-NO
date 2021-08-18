---
title: Aktivere kostnadsstyring
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
ms.openlocfilehash: 62f3cfb161c4f8da735bd288a2d6e22971b4aada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325472"
---
# <a name="enable-cost-management"></a>Aktivere kostnadsstyring

**Hva betyr «kostnader er deaktivert for organisasjonen»?**

Organisasjoner som Microsoft Foretaksavtale (EA) eller Microsoft Customer Agreement (MCA)-kontoer, kan deaktivere tilgang til kostnadsinformasjon og prisinformasjon.

Når de har logget på Azure-portalen, kan de bruke fakturerings-API-ene til å få fakturaer (når de er valgt inn) og bruksdetaljer.

**Slik tillater du at flere brukere får tilgang til fakturaer**

1. Gå til **Abonnementer-bladet** i Azure Portal.
2. Velg **Fakturaer** og deretter **Tilgang til fakturaer**.
3. Aktiver tilgangen, etterfulgt av å lagre endringene, slik at brukere i abonnementsomfangsroller kan laste ned fakturaer.

**Obs!** Kontoadministratoren kan også konfigurere slik at fakturaer sendes via e-post. Hvis du vil ha mer informasjon, [kan du se Få fakturaen i e-post](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Slik legger du til brukere i faktureringsleserrollen**

1. Gå til **Abonnementer-bladet** i Azure Portal.
2. Velg **Access-kontroll (IAM),** og klikk deretter Legg **til**.
3. Velg **Faktureringsleser** på **siden Velg en rolle.**
4. Skriv inn e-postmeldingen til brukeren du vil invitere, og klikk deretter **OK** for å sende invitasjonen.
5. Følg instruksjonene i invitasjons-e-postmeldingen for å logge på som en faktureringsleser. Hvis du vil ha mer informasjon, [kan du se Gi tilgang til fakturering](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Anbefalte dokumenter**

- [Aktivere DA- og AO-visninger via EA-portalen](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kostnader som er inkludert i Kostnadsstyring](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Støttede Microsoft Azure tilbud](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Se gjennom kostnader i kostnadsanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Gi tilgang til faktureringsinformasjon](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Kontroller tilgang til en Microsoft-kundeavtale](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






