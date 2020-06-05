---
title: Instruksjoner for å skjule/vise gruppe fra adresselisten
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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580018"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="d31a1-102">Skjul Microsoft 365-gruppen fra adresselisten (GAL)</span><span class="sxs-lookup"><span data-stu-id="d31a1-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="d31a1-103">Hvis du vil skjule en Microsoft 365-gruppe fra adresselister (GAL) for Exchange-klienter (for eksempel Outlook eller OWA), bruker du følgende kommando i EXO-skallet:</span><span class="sxs-lookup"><span data-stu-id="d31a1-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="d31a1-104">Hvis du vil skjule Microsoft 365-gruppen fra å være synlig for Exchange-klienter, kan du bruke følgende kommando i EXO-skallet:</span><span class="sxs-lookup"><span data-stu-id="d31a1-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

