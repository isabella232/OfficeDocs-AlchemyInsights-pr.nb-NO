---
title: ATP for SharePoint, OneDrive og Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715570"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP for SharePoint, OneDrive og Microsoft Teams

Følg disse trinnene for å aktivere Advanced Threat Protection:

1. Gå til [https://protection.office.com](https://protection.office.com) og Logg på med en global administrator-eller sikkerhets administrator konto.

2. Velg **policy** klarerte vedlegg i den venstre navigasjons ruten under **trussel administrasjon** \> **Safe Attachments**.

3. Velg **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams**.

4. [Opprette en policy for aktivitets varsel](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) for å motta varsler når vi oppdager skadelige filer.

Hvis du vil ha fullstendige instruksjoner, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Obs**! ATP kan ikke skanne hver enkelt fil i SharePoint Online, OneDrive for Business eller Microsoft Teams. Filer skannes asynkront av en prosess som bruker Delings aktivitet, gjeste aktivitet og trussel signaler til å identifisere skadelige filer. Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
