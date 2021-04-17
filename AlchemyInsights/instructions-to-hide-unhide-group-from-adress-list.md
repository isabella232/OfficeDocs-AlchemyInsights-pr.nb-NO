---
title: Instruksjoner for å skjule/vise gruppe fra adresselisten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831887"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skjule Microsoft 365-gruppen fra adresselisten (GAL)

Hvis du vil skjule en Microsoft 365-gruppe fra adresselister (GAL) med Exchange-klienter (for eksempel Outlook eller OWA), bruker du følgende kommando i EXO-skallet:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Hvis du vil skjule Microsoft 365-gruppen fra å være synlig for Exchange-klienter, bruker du følgende kommando i EXO-skallet:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

