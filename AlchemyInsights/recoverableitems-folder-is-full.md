---
title: 1336 RecoverableItems-mappen er full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720261"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen Gjenopprettelige elementer er full

For Exchange Online-postbokser er standard lagringsgrense for mappen Gjenopprettelige elementer 30 GB. Lagringsgrensen for mappen Gjenopprettelige elementer økes automatisk til 100 GB hvis postboksen er plassert på rettstvistsperre, eDiscovery-sperring eller tilordnes til en oppbevaringspolicy.

Når mappen Gjenopprettelige elementer når lagringsgrensen, påvirkes postboksfunksjonaliteten på følgende måter:

- Brukeren kan ikke slette elementer fra postboksen.

- Hjelperen for administrert mappe kan ikke slette elementer basert på innstillinger for oppbevaringskode eller administrertmappe.

- For postbokser som har enkel elementgjenoppretting aktivert eller plassert på vent, kan ikke copy-on-write-sidebeskyttelsesprosessen vedlikeholde versjoner av elementer som er redigert av brukeren.

- For postbokser som har postboksen overvåking logging aktivert, ingen postboks overvåkingslogg oppføringer kan lagres i mappen Revisjoner undermappen i mappen Gjenopprettelige elementer.

For postbokser som ikke er på vent, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kan administratorer bruke kommandoen i Exchange Online PowerShell til å slette elementer i mappen Gjenopprettelige elementer. Hvis du vil ha mer informasjon, kan du se følgende emner:

- [Søke etter og slette meldinger](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Søk-postboks](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For postbokser som er på vent, må administratorer fjerne sperringen før de kan slette elementer fra mappen Gjenopprettelige elementer. Hvis du vil ha mer informasjon, kan du se [Slette elementer i mappen Gjenopprettelige elementer i skybaserte postbokser på vent](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

For å forhindre at mappen Gjenopprettelige elementer blir full, kan administratorer øke lagringsgrensen for mappen Gjenopprettelige elementer for postbokser på vent og konfigurere en postboksoppbevaringspolicy som flytter elementer fra mappen Gjenopprettelige elementer til brukerens arkivpostboks. Se [Øke kvoten for gjenopprettelige elementer for postbokser på vent](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
