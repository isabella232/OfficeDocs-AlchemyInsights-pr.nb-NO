---
title: 1336 RecoverableItems-mappen er full
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741276"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen gjen opprettelige elementer er full

For Exchange Online-postbokser er standard lagrings grense for mappen gjen opprettelige elementer 30 GB. Lagrings grensen for mappen gjen opprettelige elementer økes automatisk til 100 GB hvis post boksen er plassert på en rettslig sperre, i eDiscovery-sperring eller tilordnes til en oppbevarings policy.

Når mappen gjen opprettelige elementer når lagrings grensen, påvirkes post boks funksjonaliteten på følgende måter:

- Brukeren kan ikke slette elementer fra post boksen.

- Assistenten for forvaltede mapper kan ikke slette elementer basert på oppbevarings kode eller innstillinger for forvaltede mapper.

- For post bokser som har en enkelt vare gjenoppretting aktivert eller som er satt på vent, kan ikke tillatelse til å opprettholde versjonen av elementer som er redigert av brukeren, bli behandlet.

- For post bokser der overvåkings logging for post boks er aktivert, kan ikke oppføringer i overvåkings loggen for post boksen lagres i overvåkings under mappen i mappen gjen opprettelige elementer.

For post bokser som ikke er på vent, kan administratorer bruke `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandoen i Exchange Online PowerShell til å slette elementer i mappen gjen opprettelige elementer. Hvis du vil ha mer informasjon, kan du se følgende emner:

- [Søke etter og slette meldinger](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Søk – post boks](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

For post bokser som er på vent, må administratorer fjerne sperringen før de kan slette elementer fra mappen gjen opprettelige elementer. Hvis du vil ha mer informasjon, kan du se [slette elementer i mappen gjen opprettelige elementer i Sky BAS ert post bokser på vent](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

For å hindre at mappen gjen opprettelige elementer blir full, kan administratorer øke lagrings grensen for mappen gjen opprettelige elementer for post bokser på vent og konfigurere en oppbevarings policy for post boks som flytter elementer fra mappen gjen opprettelige elementer til brukerens arkiv post boks. Se [øke gjenopprettende element kvoten for post bokser som er sperret](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
