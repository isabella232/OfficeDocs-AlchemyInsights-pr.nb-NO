---
title: 1336 RecoverableItems mappen er full
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
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510761"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen Gjenopprettelige elementer er full

For Exchange Online-postbokser er standard lagringsgrense for mappen Gjenopprettelige elementer 30 GB. Lagringsgrensen for mappen Gjenopprettelige elementer økes automatisk til 100 GB hvis postboksen er plassert på prosedyresperre, eDiscovery hold eller er tilordnet til en oppbevaringspolicy.

Når mappen Gjenopprettelige elementer når lagringsgrensen, påvirkes postboksfunksjonaliteten på følgende måter:

- Brukeren kan ikke slette elementer fra postboksen.

- Administrert mappeassistent kan ikke slette elementer basert på lagringskode eller administrerte mappeinnstillinger.

- For postbokser som har enkel elementgjenoppretting aktivert eller er plassert på vent, kan ikke beskyttelsesprosessen for copy-on-write-siden vedlikeholde versjoner av elementer som er redigert av brukeren.

- For postbokser som har postboks overvåking logging aktivert, ingen postboks overvåkingsloggoppføringer kan lagres i undermappen overvåkingser i mappen Gjenopprettelige elementer.

For postbokser som ikke er på vent, kan administratorer bruke `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandoen i Exchange Online PowerShell til å slette elementer i mappen Gjenopprettelige elementer. Hvis du vil ha mer informasjon, kan du se følgende emner:

- [Søke etter og slette meldinger](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Søkepostboks](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For postbokser som er på vent, må administratorer fjerne sperren før de kan slette elementer fra mappen Gjenopprettelige elementer. Hvis du vil ha mer informasjon, kan du se [Slette elementer i mappen Gjenopprettelige elementer i skybaserte postbokser på vent](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Hvis du vil hindre at mappen Gjenopprettelige elementer blir fullstendige, kan administratorer øke lagringsgrensen for mappen Gjenopprettelige elementer for postbokser som er på vent og konfigurere en postboksoppbevaringspolicy som flytter elementer fra mappen Gjenopprettelige elementer til brukerens arkivpostboks. Se [Øke kvoten gjenopprettelige elementer for postbokser på vent](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
