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
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivere innebygging av eldre dialogbokser for å åpne rapporter

**Symptom**

Brukere kan ikke åpne rapporter. «Noe har gått galt. Se tekniske detaljer for mer informasjon.»

**Årsak**

Rapporter lastes ikke inn i UCI med feilen «Skjemabeskrivelse er null eller ikke definert». Rapporter i UCI krever fortsatt eldre dialogbokser, så kundens system må ha *allowlegacydialogsembedding aktivert.*

**Løsning**

1. Gå til **Innstillinger >Administrasjon > Systeminnstillinger > Generelt-fanen**.

2. Sett «Aktiver innebygging av enkelte eldre dialogbokser i Unified Interface nettleserklient» til **Ja**.
