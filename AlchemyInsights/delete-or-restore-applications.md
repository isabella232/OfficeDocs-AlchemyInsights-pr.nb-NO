---
title: Slette eller gjenopprette programmer
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102580"
---
# <a name="delete-or-restore-applications"></a>Slette eller gjenopprette programmer

**Slik sletter du et program fra Azure AD-leieren:**

1. Velg **Enterprise-programmer** i Azure **AD-portalen**. Deretter finner og velger du programmet du vil slette.
2. Velg Egenskaper i **Behandle-delen** i den venstre **ruten.**
3. Velg **Slett**, og velg deretter **Ja** for å bekrefte at du vil slette appen fra Azure AD-leieren.

Hvis du vil ha mer informasjon om hvordan du sletter en app, kan du se Hurtigstart: Slette et program fra Azure Active Directory [(Azure AD) tenant.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

I PowerShell fjerner [Remove-AzureADApplicationProxyApplication-cmdleten](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) Application Proxy-konfigurasjoner fra et bestemt program i Azure Active Directory, og kan slette programmet fullstendig hvis det er angitt.

Du kan **gjenopprette et slettet program ved hjelp** av PowerShell. Når programmet du vil gjenopprette, er identifisert, kan du gjenopprette det ved hjelp [av Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
