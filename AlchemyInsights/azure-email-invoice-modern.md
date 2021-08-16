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
ms.openlocfilehash: caf300873c3a9a97502819c7938ecc86491795d2fc7b6f022ead5d38ca965b8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082843"
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
