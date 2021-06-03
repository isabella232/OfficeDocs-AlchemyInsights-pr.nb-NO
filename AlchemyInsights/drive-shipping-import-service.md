---
title: Diskforsendelse i Microsoft 365 importtjenesten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731654"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Diskforsendelse i Microsoft 365 importtjenesten

Bruk Diskforsendelse ved å kopiere PSTer til en harddisk og deretter sende harddisken til Microsoft.

Slik starter du jobben:

1. Velg Importer Microsoft 365 i **samsvarssenteret** for informasjon under **Informasjonsstyring**.

1. Velg **Velg importjobbtype**, og velg deretter **Neste**.

1. Hvis du vil se trinnene for dette importalternativet, velger du **Lever harddisker til en av våre fysiske plasseringer**.

Her er noen ting du må huske på:

- Du må være tilordnet rollen Importer postboks i Exchange Online importere PST-filer til Microsoft 365 postbokser.
Ytelsen kan påvirkes for PST-er som er større enn 20 GB.

- Bare 2,5-tommers SSD-er (solid state drives) eller 2,5-tommers eller 3,5-tommers SATA II/III interne harddisker støttes.
Harddisken som inneholder PST-filer, må krypteres med BitLocker.

- Kostnaden for å importere PST-filer til Microsoft 365 postbokser ved hjelp av stasjonsforsendelse er USD 2 per GB med data.

Hvis du vil ha mer informasjon om hvordan du bruker diskforsendelsesmetoden for import av PSTer, kan du se Bruke stasjonsforsendelse til [å importere organisasjonens PST-filer](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).