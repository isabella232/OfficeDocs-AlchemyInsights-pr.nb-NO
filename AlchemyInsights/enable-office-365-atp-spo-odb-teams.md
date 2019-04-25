---
title: Aktivere Office 365 ATP for SharePoint, OneDrive og Microsoft Team
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403042"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Office 365 Avansert trussel beskyttelse for SharePoint Online, OneDrive og Microsoft Team

1. Gå til https://protection.office.com og logger deg på.
2. Velg **Threat management** > **Policy** > **Sikker vedlegg**.
3. Velg **Slå på ATP-Antallet for SharePoint, OneDrive, og Microsoft Team**, og klikk deretter **Lagre**.
4. (Anbefales) Som en global administrator eller en administrator for SharePoint Online, kjører du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **DisallowInfectedFileDownload** -parameteren angitt til *Sann*.
5. (Anbefales) [Angi varsler](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.

> [!NOTE]
> ATP vil nFor skanning hver enkelt fil i SharePoint Online, OneDrive, eller Microsoft Teams. Filer skannes asynkront, gjennom en prosess som bruker deling og gjest aktivitet hendelser, sammen med smart heuristisk og trusselen signaler til å identifisere ondsinnede filer. Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).