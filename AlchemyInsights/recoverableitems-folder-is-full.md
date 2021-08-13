---
title: Mappen 1336 RecoverableItems er full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061765"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen Gjenopprettelige elementer er full

For Exchange Online postbokser er standard lagringsgrense for mappen Gjenopprettelige elementer 30 GB. Lagringsgrensen for mappen Gjenopprettelige elementer økes automatisk til 100 GB hvis postboksen er plassert på rettslig sperre, eDiscovery-sperring eller er tilordnet en oppbevaringspolicy.

Når mappen Gjenopprettelige elementer når lagringsgrensen, påvirkes postboksfunksjonaliteten på følgende måter:

- Brukeren kan ikke slette elementer fra postboksen.

- Assistenten for administrert mappe kan ikke slette elementer basert på oppbevaringskode eller administrerte mappeinnstillinger.

- For postbokser som har gjenoppretting av enkeltelement aktivert eller er satt på vent, kan ikke sidebeskyttelsesprosessen for kopi ved skriving vedlikeholde versjoner av elementer som er redigert av brukeren.

- For postbokser der overvåkingslogging for postboks er aktivert, kan ingen oppføringer i overvåkingsloggen for postboks lagres i undermappen Overvåkinger i mappen Gjenopprettelige elementer.

For postbokser som ikke er på vent, kan administratorer bruke kommandoen i PowerShell Exchange Online å slette elementer i mappen `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Gjenopprettelige elementer. Hvis du vil ha mer informasjon, kan du se følgende emner:

- [Søke etter og slette meldinger](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For postbokser som er sperret, må administratorer fjerne sperringen før de kan slette elementer fra mappen Gjenopprettelige elementer. Hvis du vil ha mer informasjon, kan du se Slette elementer i mappen Gjenopprettelige elementer i [skybaserte postbokser på vent](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

For å hindre at mappen Gjenopprettelige elementer blir full, kan administratorer øke lagringsgrensen for mappen Gjenopprettelige elementer for postbokser på vent og konfigurere en oppbevaringspolicy for postboksen som flytter elementer fra mappen Gjenopprettelige elementer til brukerens arkivpostboks. Se [Øke kvoten for gjenopprettelige elementer for postbokser på vent](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
