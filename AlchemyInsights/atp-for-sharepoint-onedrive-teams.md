---
title: ATP for SharePoint, OneDrive og Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712467"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP for SharePoint, OneDrive og Microsoft Teams

Følg denne fremgangsmåten for å aktivere avansert trusselbeskyttelse:

1. Gå [https://protection.office.com](https://protection.office.com) til og logg på med en global administrator- eller sikkerhetsadministratorkonto.

2. Velg **Policysikre** \> **vedlegg**i navigasjonsruten til venstre under **Trusselbehandling**.

3. Velg **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams**.

4. [Opprett en policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) for aktivitetsvarsling for å motta varsler når vi oppdager skadelige filer.

Hvis du vil ha fullstendige instruksjoner, kan du se dette [emnet](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).

**Merk:** Ved utforming skanner ikke ATP hver eneste fil i SharePoint Online, OneDrive for Business eller Microsoft Teams. Filer skannes asynkront av en prosess som bruker delingsaktivitet, gjesteaktivitet og trusselsignaler til å identifisere skadelige filer. Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
