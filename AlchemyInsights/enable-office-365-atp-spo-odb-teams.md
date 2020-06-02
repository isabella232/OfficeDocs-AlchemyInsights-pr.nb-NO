---
title: Aktivere Office 365 ATP for SharePoint, OneDrive og Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506927"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere avansert trusselbeskyttelse for Office 365 for SharePoint Online, OneDrive og Microsoft Teams

1. Gå til https://protection.office.com og logg på.
2. Velg Sikker vedlegg for **trusselbehandling**  >  **Policy**  >  **Safe Attachments**.
3. Velg **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams**, og klikk deretter **Lagre**.
4. (Anbefales) Som en global administrator eller en SharePoint Online-administrator kjører du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parameteren **DisallowInfectedFileDownload** satt til *true*.
5. (Anbefales) [Konfigurer varsler](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.

> [!NOTE]
> ATP vil skanne hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer skannes asynkront, gjennom en prosess som bruker delings- og gjesteaktivitetshendelser, sammen med smarte heuristikk og trusselsignaler for å identifisere skadelige filer. Se [ATP for SharePoint, OneDrive og Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).