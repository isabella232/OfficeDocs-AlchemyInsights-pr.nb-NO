---
title: Aktivere Office 365 ATP for SharePoint, OneDrive og Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332168"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams

1. Gå til https://protection.office.com og logg på.
2. Velg **Policy for**  >  **trusselbehandling Safe**  >  **vedlegg**.
3. Velg **Aktiver Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams**, og klikk deretter **Lagre**.
4. (Anbefales) Som global administrator eller SharePoint Online-administrator kjører du [Set-SPOTenant-cmdleten](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **parameteren DisallowInfectedFileDownload** satt til *sann*.
5. (Anbefales) [Konfigurere varsler](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.

**Obs!** Microsoft Defender for Office 365 skanner ikke hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer skannes asynkront gjennom en prosess som bruker delings- og gjesteaktivitetshendelser, sammen med smart heuristikk og trusselsignaler for å identifisere skadelige filer. Se [Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
