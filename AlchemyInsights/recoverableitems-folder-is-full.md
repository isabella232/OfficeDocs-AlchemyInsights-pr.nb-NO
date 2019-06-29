---
title: 1336 RecoverableItems mappen er full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370396"
---
# <a name="the-recoverable-items-folder-is-full"></a>Gjenopprettbare elementer-mappen er full

For Exchange Online-postbokser i Office 365 er standard lagringsgrensen for mappen gjenopprettelige elementer 30 GB. Lagringsgrensen for mappen gjenopprettelige elementer økes automatisk til 100 GB Hvis postboksen er plassert på rettstvist holder, eDiscovery sperring eller er knyttet til en oppbevaringspolicy for Office 365.

Når mappen gjenopprettelige elementer når lagringsgrensen, påvirkes postboks-funksjonalitet på følgende måter:

- Brukeren kan ikke slette elementer fra postboksen.

- Administrerte Mappeassistent kan ikke slette elementer som er basert på kode for oppbevaring eller innstillinger for administrerte mapper.

- Kopier på skrive siden beskyttelse prosessen kan ikke opprettholde versjoner av elementene som redigeres av brukeren for postbokser som har enkel gjenoppretting for elementer som er aktivert eller er satt på vent.

- For postbokser som har postboksen overvåkes logging er aktivert, kan ingen postboks loggoppføringer for sporing av endringer ikke lagres i overvåking-undermappe i mappen gjenopprettbare elementer.

Administratorer kan bruke for postbokser som ikke er på vent og, den `Search-Mailbox -SearchDumpsterOnly -DeleteContent` i Exchange Online PowerShell til å slette elementer i mappen gjenopprettbare elementer. Hvis du vil ha mer informasjon, kan du se følgende emner:

- [Søke etter og slette meldinger](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Søk-postboks](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Administratorer må fjerne sperringen før de kan Slettede elementer fra mappen gjenopprettelige elementer for postbokser som er på vent. Hvis du vil ha mer informasjon, kan du se [slette elementer i gjenopprettbare elementer-mappen for \\\cloud-based postbokser på holder](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Administratorer kan øke lagringskapasiteten av gjenopprettbare elementer mappen for postbokser på hold og sette opp en oppbevaringspolicy på postboksen som flytter elementer fra mappen gjenopprettelige elementer til brukerens Arkiv for å hindre at mappen gjenopprettelige elementer blir full, postboks. Se [øke gjenopprettbare elementer kvote for postbokser på hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
