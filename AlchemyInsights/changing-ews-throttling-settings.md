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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="e62dd-102">Endre EWS-begrensningsinnstillinger</span><span class="sxs-lookup"><span data-stu-id="e62dd-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="e62dd-103">Kjør den automatiserte testen som gjør det mulig å endre EWS-begrensningspolicyen så lenge overføringen varer.</span><span class="sxs-lookup"><span data-stu-id="e62dd-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="e62dd-104">Vær oppmerksom på at selv etter at dette kjøres, vil EWS-importer fremdeles være begrenset til 150 MB per 5 minutter per postkasse. For å oppnå en høyere overføringshastighet kan du overføre flere brukere samtidig.</span><span class="sxs-lookup"><span data-stu-id="e62dd-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="e62dd-105">Vær oppmerksom på at endringer i EWS-begrensningspolicyer ikke har noen effekt på følgende overføringstyper (ved hjelp av Microsoft-verktøy): Hybrid, fullstendig/trinnvis (RPC/HTTP), IMAP, G Suite, fellesmappe eller PST-importtjeneste.</span><span class="sxs-lookup"><span data-stu-id="e62dd-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>