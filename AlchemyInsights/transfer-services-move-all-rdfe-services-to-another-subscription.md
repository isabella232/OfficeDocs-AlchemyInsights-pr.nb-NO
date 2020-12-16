---
title: Overføre tjenester – flytte alle RDFE-tjenester til et annet abonnement
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692171"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Overføre tjenester – flytte alle RDFE-tjenester til et annet abonnement

**Flytte ressurser**

Azure-ressurser kan flyttes til enten et annet Azure-abonnement eller en ressurs gruppe under samme abonnement ved hjelp av Azure Portal, Azure PowerShell, Azure CLI eller REST-API-en til å flytte ressurser.

Før du kan flytte ressurser, kan du se:

- [Sjekk liste før du flytter ressurser](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Tjenester som kan flyttes](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Slik validerer du flyttingen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Flytte veiledning for tjenester](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Hvis du vil flytte eksisterende ressurser til en annen ressurs gruppe eller-abonnement, kan du bruke:

- [Azure-Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST-API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Opplæring: [flytte Azure-ressurser til andre ressurs grupper eller-abonnementer](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Feilsøke feil med Azure Resource Manager**

Se artiklene nedenfor for å lære om noen vanlige distribusjons feil i Azure, og motta informasjon for å løse dem. Hvis du ikke finner feil koden for distribusjons feilen, kan du se [finne feil koden](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Feilsøke distribusjons feil](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Feilsøke flytting av Azure-ressurser til ny ressurs gruppe eller et abonnement](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Vær oppmerksom på at hvis du vil oppgradere Azure-abonnementet, for eksempel bytte fra gratis til Betal etter hvert, må du konvertere abonnementet.

- Hvis du vil oppgradere en gratis prøve versjon, kan du se [oppgradere gratis prøve versjon eller Microsoft Forestill deg Azure-abonnementet til å betale etter](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)hvert.
- Hvis du vil endre en betal som-a-konto, kan du se [endre abonnementet på Azure Betal-etter-farten til et annet tilbud](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Slik legger du til eller knytter et Azure-abonnement til Azure Active Directory-leieren:**

1. Logg på, og Velg abonnementet du vil bruke fra abonnementer- [siden i Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Velg **endre katalog**.
3. Se gjennom eventuelle advarsler som vises, og velg deretter **endre**.
4. Katalogen er endret for abonnementet, og du vil få en vellykket melding.
5. Bruk *katalog* -bytte ren for å gå til den nye katalogen. Det kan ha opptil ti minutter før alt vises på riktig måte.

**Anbefalte dokumenter**

- [Overføre eierskap for et Azure-abonnement](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Flytte ressurser til ny ressurs gruppe eller et abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Behandle ressurser ved hjelp av Azure-portalen](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
