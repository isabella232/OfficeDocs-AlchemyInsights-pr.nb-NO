---
title: Moderne e-postfakturering i Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820835"
---
# <a name="email-invoicing-in-azure"></a>E-postfakturering i Azure

Du må ha rollen eier eller bidragsyter på faktureringsprofilen eller faktureringskontoen for å oppdatere innstillingen for e-postfakturering. Når du har aktivert dette, får alle brukere som har rollene eier, bidragsyter, lesere og fakturaansvarlig på en faktureringsprofil, faktura på e-post.

1. Logg på [Azure-portalen](https://portal.azure.com/).
2. Søk etter **Kostnadsadministrasjon + fakturering**.
3. Velg **Fakturaer** fra venstre side, og velg deretter **E-postfaktura** fra toppen av siden.
4. Hvis du har flere faktureringsprofiler, velger du en faktureringsprofil og deretter **Aktiver**.

5. Velg **Oppdater**.
6. Hvis du har flere faktureringsprofiler, velger du en faktureringsprofil og deretter **Aktiver**.

Du gir andre tilgang til å vise, laste ned og betale fakturaer ved å tilordne dem rollen fakturaansvarlig for en MCA- eller MPA-faktureringsprofil. Hvis du har aktivert å få faktura på e-post, får brukerne også fakturaene på e-post.

1. Logg på [Azure-portalen](https://portal.azure.com/).
2. Søk etter **Kostnadsadministrasjon + fakturering**.
3. Velg **Faktureringsprofiler** fra venstre side. Velg en faktureringsprofil som du vil tilordne rollen fakturaansvarlig, fra listen over faktureringsprofiler.
4. Velg **Tilgangskontroll (IAM)** fra venstre side, og velg deretter **Legg til** fra toppen av siden.

Velg **Fakturaansvarlig** i rullegardinlisten Rolle. Angi e-postadressen til brukeren for å gi tilgang. Velg **Lagre** for å tilordne rollen.
