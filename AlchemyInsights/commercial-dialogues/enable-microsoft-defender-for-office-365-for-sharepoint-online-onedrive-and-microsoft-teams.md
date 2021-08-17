---
title: Aktivere Safe vedlegg for SharePoint Online, OneDrive og Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894472"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivere Safe vedlegg for SharePoint Online, OneDrive og Microsoft Teams

1. Bruk den globale administrator- eller sikkerhetsadministratorlegitimasjonen, åpne Microsoft 365 Defender-portalen på , og gå deretter til Policyer & regler Trusselpolicyer Safe Vedlegg i <https://security.microsoft.com>  \>  \>  **Policyer-delen**

   Hvis du vil gå direkte **til Safe Vedlegg-siden,** bruker du <https://security.microsoft.com/safeattachmentv2> .

2. Klikk **Globale Safe på** siden **Vedlegg.**
3. Velg **Aktiver Microsoft Defender for** Office 365 for SharePoint, OneDrive og Microsoft Teams på undermenyen som **vises,** og velg deretter Lagre .

    > [!TIP]
    >
    > Gjør følgende for å forbedre beskyttelsen av Safe vedlegg for SharePoint, OneDrive og Microsoft Teams:
    >
    > - Hvis du vil hindre brukere i å laste ned skadelige filer, bruker du verdien `$true` for *disallowInfectedFileDownload-parameteren* på **[Set-SPOTenant-cmdleten](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** i SharePoint Online PowerShell. Hvis du vil ha mer [informasjon, kan du se Bruke SharePoint PowerShell](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)til å hindre brukere i å laste ned skadelige filer .
    > - [Opprette en varslingspolicy for oppdagede filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Hvis du vil ha mer [informasjon, kan du Safe vedlegg for](https://go.microsoft.com/fwlink/?linkid=2092041)Office 365 for SharePoint, OneDrive og Microsoft Teams .
