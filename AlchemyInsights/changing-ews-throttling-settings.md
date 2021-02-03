---
title: Endre EWS-begrensningsinnstillinger
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075906"
---
# <a name="changing-ews-throttling-settings"></a>Endre EWS-begrensningsinnstillinger

Kjør den automatiserte testen som gjør det mulig å endre EWS-begrensningspolicyen så lenge overføringen varer. Vær oppmerksom på at selv etter at dette kjøres, vil EWS-importer fremdeles være begrenset til 150 MB per 5 minutter per postkasse. For å oppnå en høyere overføringshastighet kan du overføre flere brukere samtidig.

Vær oppmerksom på at endringer i EWS-begrensningspolicyer ikke har noen effekt på følgende overføringstyper (ved hjelp av Microsoft-verktøy): Hybrid, fullstendig/trinnvis (RPC/HTTP), IMAP, G Suite, fellesmappe eller PST-importtjeneste.