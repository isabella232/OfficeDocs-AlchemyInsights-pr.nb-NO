---
title: Samtidig ledelse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40910376"
---
# <a name="co-management"></a>Samtidig ledelse

**Forutsetninger for migrering fra config Manager hybrid til Intune**

- Se gjennom [denne artikkelen](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).
- [Legg til en Intune-lisens for brukerne](https://docs.microsoft.com/intune/licenses-assign).
- Bruk [kanten nettleser](https://www.microsoft.com/windows/microsoft-edge) når du konfigurerer co-Management.

**Hvordan jeg installerer config Manager-klienten på Intune-administrerte enheter**

Se [INTUNE MDM-Managed Windows-enheter](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).

**Hva om jeg bare ønsker å endre MDM autoritet?**

MDM Authority kan endres uten å åpne en støtte sak. Les følgende dokumentasjon for å bistå i endring av MDM-myndigheten:
- [Endre MDM-instans fra Konfigurasjonsbehandling til frittstående Intune](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [Endre MDM-instans fra frittstående Intune til config Manager](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)