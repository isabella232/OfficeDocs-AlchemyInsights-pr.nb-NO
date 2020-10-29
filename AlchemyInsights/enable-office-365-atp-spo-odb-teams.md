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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801062"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams

1. Gå til https://protection.office.com og Logg på.
2. Velg sikre **administrasjons**  >  **policyer** for  >  **klarerte vedlegg** .
3. Velg **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams** , og klikk deretter **Lagre** .
4. Anbefaler Som global administrator eller administrator for SharePoint Online kjører du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **DisallowInfectedFileDownload** -parameteren angitt til *sann* .
5. Anbefaler [Konfigurer varsler](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.

> [!NOTE]
> ATP vil skal kunne skanne hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer skannes asynkront, gjennom en prosess som bruker hendelser for Delings-og gjeste aktivitet, sammen med smarte heuristikk og trussel signaler for å identifisere skadelige filer. Se [ATP for SharePoint, OneDrive og Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).