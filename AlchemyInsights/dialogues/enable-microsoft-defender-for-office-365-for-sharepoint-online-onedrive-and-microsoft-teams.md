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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695648"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams

1. Bruk legitimasjonen for global administrator eller sikkerhetsadministrator, og logg på sikkerhets- og samsvarssenteret for [Office 365.](https://protection.office.com/)
2. Velg **trusselbehandling** i den venstre ruten, og velg deretter **Policysikkert**  >  [vedlegg.](https://protection.office.com/safeattachment)
3. Velg **Slå på Microsoft Defender for Office 365 for SharePoint, OneDrive** og Microsoft Teams, og velg deretter **Lagre.**
    > [!TIP]
    >
    > - Som global administrator eller sharePoint Online-administrator kan du kjøre følgende PowerShell-cmdlet med **disallowInfectedFileDownload-parameteren** satt til *sann:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Konfigurere varsler for oppdagede filer](https://go.microsoft.com/fwlink/?linkid=2092110)

Hvis du vil ha mer informasjon, kan du se [Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
