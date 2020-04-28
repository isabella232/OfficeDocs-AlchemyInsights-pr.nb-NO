---
title: Instruksjoner for å skjule/vise gruppe fra adresseliste
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908353"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skjule Microsoft 365-gruppe fra adresseliste (GAL)

Hvis du vil skjule en Microsoft 365-gruppe fra adresselister (GAL) for Exchange-klienter (for eksempel Outlook eller OWA), bruker du følgende kommando i EXO-skallet:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Hvis du vil skjule Microsoft 365-gruppen fra å være synlig for Exchange-klienter, bruker du følgende kommando i EXO-skallet:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

