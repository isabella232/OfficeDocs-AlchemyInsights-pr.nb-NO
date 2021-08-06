---
title: Abonnementstilgang
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
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999249"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Kan ikke logge på Azure på grunn av nettleserproblemer (nettleseren henger, fortsetter å spinne, lastes ikke inn osv.)

Du kan bli påvirket av et strømbrudd. Kontroller om det er et pågående strømbrudd: [Azure-tilstandsstatus](https://status.azure.com/status/history/).

Logg av alle aktive Azure-økter. Start en privat eller inkognitomodus i nettleseren.

Du kan også prøve å oppdatere nettleseren, bruke en annen nettleser og slette informasjonskapsler for buffer hvis den ovenfor ikke fungerer.

Finn ut mer: [Feilsøke påloggingsproblemer](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Får ikke tilgang til abonnementer**

Kontroller at riktig Azure-katalog er valgt fra kontoen øverst til høyre i [Azure-portalen.](https://portal.azure.com/)

Kontroller at [kontoen](https://account.windowsazure.com/Subscriptions)som brukes, er kontoadministratoren, i Azure-kontosenteret.

Finn ut mer: [Feilsøke ingen abonnementer funnet](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Får ikke tilgang til faktureringsloggen**

Kontoadministratoren må sørge for at brukeren som får tilgang til faktureringsinformasjonen, legges til i Azure Active Directory som gjestebruker: Legge til eller [slette en ny bruker](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Brukeren må deretter gis en global administratorrolle: [Tilordne rolle til brukere](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Etter dette kan brukeren få faktureringstilgang ved hjelp av RBAC-policyer: [Gi tilgang til fakturering](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Anbefalte dokumenter**

-   [Jeg kan ikke logge på for å administrere Azure-abonnementet mitt](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)