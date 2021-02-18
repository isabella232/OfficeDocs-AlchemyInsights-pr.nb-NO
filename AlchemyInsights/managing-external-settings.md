---
title: Administrere eksterne innstillinger
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294314"
---
# <a name="managing-external-settings"></a>Administrere eksterne innstillinger

**Kunngjøring**

- [Avvikling av støtte for WebView-pålogging fra Google fra og med 4. januar 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support) Test om appene påvirkes ved å følge Googles veiledning om testing av kompatibilitet
- Pass på å bruke systemets nettvisning eller systemleser når du logger på brukerne med Google-kontoer for forbrukere

**Behandle invitasjonsinnstillinger**

Bekreft at du har [konfigurert innstillingene for eksternt samarbeid](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) slik at de riktige personene kan sende invitasjoner.

**Behandle tillatelser for gjestebrukertilgang**

1. Globale administratorer kan behandle gjestetilgangstillatelser i katalogen via Azure Portal ved å konfigurere gjestetilgangstillatelsene på siden Innstillinger for eksternt samarbeid. [Lær mer om denne innstillingen.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)
2. Hvis du vil at gjestene skal få tilgang til apper som Teams eller SharePoint, må du bekrefte at du har konfigurert disse appene til å tillate gjestetilgang. Finn ut mer om [Teams-innstillinger](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) og [SharePoint.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurere invitasjoner:**

- [Aktivere B2B eksternt samarbeid og styre hvem som kan invitere gjester](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Tillate eller blokkere invitasjoner til brukere fra bestemte organisasjoner](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**Konfigurere tillatte identitetsleverandører:**

- [Google Federation](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Direkte forbund](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Engangspassordgodkjenning for e-post](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
