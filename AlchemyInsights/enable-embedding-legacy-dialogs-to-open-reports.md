---
title: Aktivere innebygging av eldre dialogbokser for å åpne rapporter
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814273"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="e7369-102">Aktivere innebygging av eldre dialogbokser for å åpne rapporter</span><span class="sxs-lookup"><span data-stu-id="e7369-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="e7369-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="e7369-103">**Symptom**</span></span>

<span data-ttu-id="e7369-104">Brukere kan ikke åpne rapporter.</span><span class="sxs-lookup"><span data-stu-id="e7369-104">Users are unable to open reports.</span></span> <span data-ttu-id="e7369-105">«Noe har gått galt.</span><span class="sxs-lookup"><span data-stu-id="e7369-105">"Something has gone wrong.</span></span> <span data-ttu-id="e7369-106">Se tekniske detaljer for mer informasjon.»</span><span class="sxs-lookup"><span data-stu-id="e7369-106">Check technical details for more details."</span></span>

<span data-ttu-id="e7369-107">**Årsak**</span><span class="sxs-lookup"><span data-stu-id="e7369-107">**Cause**</span></span>

<span data-ttu-id="e7369-108">Rapporter lastes ikke inn i UCI med feilen «Skjemabeskrivelse er null eller ikke definert».</span><span class="sxs-lookup"><span data-stu-id="e7369-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="e7369-109">Rapporter i UCI krever fortsatt eldre dialogbokser, så kundens system må ha *allowlegacydialogsembedding aktivert.*</span><span class="sxs-lookup"><span data-stu-id="e7369-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="e7369-110">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="e7369-110">**Solution**</span></span>

1. <span data-ttu-id="e7369-111">Gå til **Innstillinger >Administrasjon > Systeminnstillinger > Generelt-fanen**.</span><span class="sxs-lookup"><span data-stu-id="e7369-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="e7369-112">Sett «Aktiver innebygging av enkelte eldre dialogbokser i Unified Interface nettleserklient» til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="e7369-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
