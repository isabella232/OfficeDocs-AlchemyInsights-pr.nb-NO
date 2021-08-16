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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003398"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Aktivere innebygging av eldre dialogbokser for å åpne rapporter

**Symptom**

Brukere kan ikke åpne rapporter. «Noe har gått galt. Se tekniske detaljer for mer informasjon.»

**Årsak**

Rapporter lastes ikke inn i UCI med feilen «Skjemabeskrivelse er null eller ikke definert». Rapporter i UCI krever fortsatt eldre dialogbokser, så kundens system må ha *allowlegacydialogsembedding aktivert.*

**Løsning**

1. Gå til **Innstillinger >Administrasjon > System Innstillinger > Generelt-fanen**.

2. Sett «Aktiver innebygging av enkelte eldre dialogbokser i Unified Interface nettleserklient» til **Ja**.
