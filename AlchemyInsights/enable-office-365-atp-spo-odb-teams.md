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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543937"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams

1. Gå til https://protection.office.com og logg på.
2. Velg **Klarerte vedlegg for** policy for  >    >  **trusselbehandling**.
3. Velg **Aktiver Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams**, og klikk deretter **Lagre**.
4. (Anbefales) Som global administrator eller SharePoint Online-administrator kjører du [Set-SPOTenant-cmdleten](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **parameteren DisallowInfectedFileDownload** satt til *sann*.
5. (Anbefales) [Konfigurere varsler](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.

> [!NOTE]
> Microsoft Defender for Office 365 vil ikke skanne hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer skannes asynkront gjennom en prosess som bruker delings- og gjesteaktivitetshendelser, sammen med smart heuristikk og trusselsignaler for å identifisere skadelige filer. Se [Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).