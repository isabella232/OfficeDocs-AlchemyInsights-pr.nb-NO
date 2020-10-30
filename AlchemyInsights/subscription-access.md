---
title: Abonnements tilgang
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
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807716"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Kan ikke logge på Azure på grunn av nett leser problemer (nett leser henger, beholder rotering, lastes ikke inn, osv.)

Du kan bli påvirket av brudd. Kontroller om det oppstår et løpende avbrudd: [Azure Health-status](https://status.azure.com/status/history/).

Logg av alle aktive Azure-økter. Start en privat eller inkognito modus for nett leseren.

Du kan også prøve å oppdatere nett leseren, bruke en annen nett leser, slette hurtig buffer informasjons kapsler hvis ovenfor ikke fungerer.

Les mer: [Feilsøke påloggings problemer](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Får ikke tilgang til abonnementer**

I [Azure-portalen](https://portal.azure.com/)må du kontrollere at riktig Azure-katalog er valgt fra kontoen øverst til høyre.

I [Azure-konto senteret](https://account.windowsazure.com/Subscriptions)kontrollerer du at kontoen som brukes, er konto administratoren.

Finn ut mer: [Feilsøke ingen abonnementer funnet](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Får ikke tilgang til fakturerings loggen**

Konto administratoren må sørge for at brukeren som har tilgang til fakturerings informasjonen, legges til i Azure Active Directory som gjeste bruker: [legge til eller slette en ny bruker](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Brukeren må deretter gis en global administrator rolle: [Tilordne rolle til brukere](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Legg inn dette, kan brukeren få tilgang til fakturering ved hjelp av RBAC-policyer: [gi tilgang til fakturering](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Anbefalte dokumenter**

-   [Jeg kan ikke logge på for å administrere Azure-abonnementet mitt](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)