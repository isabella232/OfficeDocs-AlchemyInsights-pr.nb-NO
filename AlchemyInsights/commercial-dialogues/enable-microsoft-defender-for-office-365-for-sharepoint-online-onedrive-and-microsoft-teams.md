---
title: Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058875"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams

1. Bruk den globale administrator- eller sikkerhetsadministratorlegitimasjonen til å logge på Office 365 sikkerhets- og [samsvarssenteret.](https://protection.office.com/)
2. Velg **Trusselbehandling** i den venstre ruten, og velg deretter **Policy** Safe  >  [vedlegg](https://protection.office.com/safeattachment).
3. Velg **Aktiver Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams**, og velg deretter **Lagre**.
    > [!TIP]
    >
    > - Som global administrator eller SharePoint Online-administrator kjører du følgende PowerShell-cmdlet med **parameteren DisallowInfectedFileDownload** angitt til *sann:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Konfigurere varsler for oppdagede filer](https://go.microsoft.com/fwlink/?linkid=2092110)

Hvis du vil ha mer informasjon, kan du [se Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
