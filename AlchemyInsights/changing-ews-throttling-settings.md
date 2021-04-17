---
title: Endre EWS-begrensningsinnstillinger
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818045"
---
# <a name="changing-ews-throttling-settings"></a>Endre EWS-begrensningsinnstillinger

Kjør den automatiserte testen som gjør det mulig å endre EWS-begrensningspolicyen så lenge overføringen varer. Vær oppmerksom på at selv etter at dette kjøres, vil EWS-importer fremdeles være begrenset til 150 MB per 5 minutter per postkasse. For å oppnå en høyere overføringshastighet kan du overføre flere brukere samtidig.

Vær oppmerksom på at endringer i EWS-begrensningspolicyer ikke har noen effekt på følgende overføringstyper (ved hjelp av Microsoft-verktøy): Hybrid, fullstendig/trinnvis (RPC/HTTP), IMAP, G Suite, fellesmappe eller PST-importtjeneste.