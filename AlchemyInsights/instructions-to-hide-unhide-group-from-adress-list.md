---
title: Instruksjoner for å skjule/utheve gruppe fra adresseliste
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768938"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Skjul gruppe for Office 365 fra adresseliste (GAL)

Hvis du vil skjule en gruppe for Office 365 fra adresselister (GAL) av Exchange-klienter (for eksempel Outlook eller OWA), kan du bruke følgende kommando i EXO-skallet:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Hvis du vil skjule Office 365-gruppen fra å være synlig for Exchange-klienter, bruker du følgende kommando i EXO-skallet:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

