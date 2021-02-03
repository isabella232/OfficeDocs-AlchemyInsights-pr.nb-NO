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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="73393-102">Endre EWS-begrensningsinnstillinger</span><span class="sxs-lookup"><span data-stu-id="73393-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="73393-103">Kjør den automatiserte testen som gjør det mulig å endre EWS-begrensningspolicyen så lenge overføringen varer.</span><span class="sxs-lookup"><span data-stu-id="73393-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="73393-104">Vær oppmerksom på at selv etter at dette kjøres, vil EWS-importer fremdeles være begrenset til 150 MB per 5 minutter per postkasse. For å oppnå en høyere overføringshastighet kan du overføre flere brukere samtidig.</span><span class="sxs-lookup"><span data-stu-id="73393-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="73393-105">Vær oppmerksom på at endringer i EWS-begrensningspolicyer ikke har noen effekt på følgende overføringstyper (ved hjelp av Microsoft-verktøy): Hybrid, fullstendig/trinnvis (RPC/HTTP), IMAP, G Suite, fellesmappe eller PST-importtjeneste.</span><span class="sxs-lookup"><span data-stu-id="73393-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>