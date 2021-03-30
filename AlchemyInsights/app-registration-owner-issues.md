---
title: Problemer med appregistreringseier
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404779"
---
# <a name="app-registration-owner-issues"></a>Problemer med appregistreringseier

Her er de tilgjengelige metodene for å legge til hovedstoler som eiere for appregistreringer:

- Bruke Azure AD PowerShell-modulen –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referanse: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Bruke Azure CLI – `az ad app owner add`

    Referanse: [eier av az-annonseappen](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Bruke MS Graph –

    Referanse: [Legg til eier – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Bruke Azure AD Portal – Gå til [portal.azure.com](https://portal.azure.com/) > Azure Active Directory >-appregistrering > Velg programmet > Eiere > Legg til eiere

**Kan du ikke vise programmet på appregistreringsbladet selv om du er eieren av programmet?**

Eieren av en app er ikke en administrativ rolle. Hvis innstillingen [Begrens tilgang](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) til administrasjonsportalen for Azure AD er aktivert, kan bare administrator vise programmene i appregistreringsportalen. Hvis en eier skal kunne vise programmene, kan du enten deaktivere denne innstillingen (Angi denne til NEI) eller tilordne administratorrollen til eieren for bare det bestemte programmet. Men for dette krever du en Azure AD Premium P2-lisens og aktiverer [privilegert identitetsbehandling.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
