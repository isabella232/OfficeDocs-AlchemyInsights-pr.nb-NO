---
title: ATP for SharePoint-, OneDrive- og Microsoft Teams
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
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508421"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP for SharePoint-, OneDrive- og Microsoft Teams

Følg denne fremgangsmåten for å aktivere avansert trusselbeskyttelse:

1. Gå til [https://protection.office.com](https://protection.office.com) og logg på med en global administrator- eller sikkerhetsadministratorkonto.

2. Velg **Policysikre** vedlegg i den venstre navigasjonsruten under **Trusselbehandling** \> **Safe Attachments**.

3. Velg **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams**.

4. [Opprett en policy for aktivitetsvarsler](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) for å motta varsler når vi oppdager skadelige filer.

Hvis du vil ha fullstendige instruksjoner, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Merk:** Etter utforming skanner ikke ATP hver enkelt fil i SharePoint Online, OneDrive for Business eller Microsoft Teams. Filer skannes asynkront av en prosess som bruker delingsaktivitet, gjesteaktivitet og trusselsignaler til å identifisere skadelige filer. Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
