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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014905"
---
# <a name="delete-or-restore-applications"></a>Slette eller gjenopprette programmer

**Slik sletter du et program fra Azure ad-leieren**:

1. Velg **virksomhets programmer** i **Azure ad-portalen**. Finn og Velg programmet du vil slette.
2. Velg **Egenskaper** i delen **Behandle** i ruten til venstre.
3. Velg **Slett**, og velg deretter **Ja** for å bekrefte at du vil slette appen fra Azure ad-leieren din.

Hvis du vil ha mer informasjon om hvordan du sletter en app, kan du se [hurtigst Art: slette et program fra Azure Active Directory-leieren (Azure ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

I PowerShell fjerner [Fjern-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) -cmdleten program-proxy-konfigurasjoner fra et bestemt program i Azure Active Directory, og kan slette programmet fullstendig hvis det er angitt.

Du kan **gjenopprette et slettet program** ved hjelp av PowerShell. Når programmet du vil gjenopprette, er identifisert, kan du gjenopprette det ved hjelp av [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
