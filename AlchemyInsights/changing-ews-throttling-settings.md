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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968386"
---
# <a name="changing-ews-throttling-settings"></a>Endre EWS-begrensningsinnstillinger

Kjør den automatiserte testen som gjør det mulig å endre EWS-begrensningspolicyen så lenge overføringen varer. Vær oppmerksom på at selv etter at dette kjøres, vil EWS-importer fremdeles være begrenset til 150 MB per 5 minutter per postkasse. For å oppnå en høyere overføringshastighet kan du overføre flere brukere samtidig.

Vær oppmerksom på at endringer i EWS-begrensningspolicyer ikke har noen effekt på følgende overføringstyper (ved hjelp av Microsoft-verktøy): Hybrid, fullstendig/trinnvis (RPC/HTTP), IMAP, G Suite, fellesmappe eller PST-importtjeneste.