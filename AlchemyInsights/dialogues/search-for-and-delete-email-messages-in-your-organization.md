---
title: Søke etter og slette e-postmeldinger i organisasjonen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525436"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Søke etter og slette e-postmeldinger i organisasjonen

Følg disse trinnene:

1. Hvis du ikke er global administrator, må du legge til kontoen i **rollegruppen for eDiscovery-ansvarlig** eller rollen for samsvarssøkebehandling for å søke etter **meldinger.** Hvis du vil slette meldinger, må du bli med i **rollegruppen for** organisasjonsadministrasjon eller rollen Søke etter og **fjerne administrasjon.** Tillatelser til disse rollene tilordnes i [sikkerhets- & samsvarssenteret.](https://protection.office.com)
2. [Opprett et innholdssøk](https://docs.microsoft.com/office365/securitycompliance/content-search) for å finne meldingen du vil slette.
3. [Koble til Sikkerhets- &-senteret PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Hvis du bruker MFA, kan du se disse instruksjonene: Koble til [Sikkerhets-& Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) ved hjelp av godkjenning med flere faktorer
4. Slette meldingen: Kjør `New-ComplianceSearchAction` cmdleten for å slette meldingen. Slettede meldinger flyttes til en brukers mappe for gjenopprettelige elementer. Hvis du vil ha en eksempelkommando, kan du se [Trinn 3: Slette meldingen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
