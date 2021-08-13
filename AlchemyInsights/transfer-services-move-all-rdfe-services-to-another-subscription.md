---
title: Overføringstjenester – Flytt alle RDFE-tjenester til et annet abonnement
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940074"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Overføringstjenester – Flytt alle RDFE-tjenester til et annet abonnement

**Flytte ressurser**

Azure-ressurser kan flyttes til et annet Azure-abonnement eller en annen ressursgruppe under samme abonnement ved hjelp av Azure Portal, Azure PowerShell, Azure CLI eller REST API for å flytte ressurser.

Før du kan flytte ressurser, kan du se:

- [Sjekkliste før du flytter ressurser](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Tjenester som kan flyttes](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Slik validerer du flyttingen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Flytte veiledning for tjenester](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Hvis du vil flytte eksisterende ressurser til en annen ressursgruppe eller et annet abonnement, kan du bruke følgende:

- [Azure-portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Opplæring: [Flytte Azure-ressurser til en annen ressursgruppe eller et annet abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Feilsøke feil med Azure Resource Manager**

Se artiklene nedenfor for å lære om noen vanlige Azure-distribusjonsfeil og motta informasjon for å løse dem. Hvis du ikke finner feilkoden for distribusjonsfeilen, kan du se [Finne feilkode](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Feilsøke distribusjonsfeil](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Feilsøke flytting av Azure-ressurser til en ny ressursgruppe eller et nytt abonnement](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Vær oppmerksom på at hvis du vil oppgradere Azure-abonnementet, for eksempel bytte fra gratis til å betale mens du er på farten, må du konvertere abonnementet.

- Hvis du vil oppgradere en gratis prøveperiode, kan du se Oppgradere gratis prøveperioden eller [Microsoft Imagine Azure-abonnementet til Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Hvis du vil endre en pay-as-you-go-konto, kan du se Endre [Azure Pay-As-You-Go-abonnementet til et annet tilbud.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Slik legger du til eller knytter et Azure-abonnement til Azure Active Directory tenant:**

1. Logg på, og velg abonnementet du vil bruke, fra [Abonnementer-siden i Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Velg **Endre katalog**.
3. Se gjennom eventuelle advarsler som vises, og velg deretter **Endre**.
4. Katalogen er endret for abonnementet, og du får en melding om suksess.
5. Bruk *katalogbytteren* til å gå til den nye katalogen. Det kan ta opptil 10 minutter før alt vises riktig.

**Anbefalte dokumenter**

- [Overføre eierskap for et Azure-abonnement](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Flytte ressurser til ny ressursgruppe eller et nytt abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Administrere ressurser ved hjelp av Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
