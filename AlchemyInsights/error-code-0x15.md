---
title: Feilkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du får en feilmelding mens du aktiverer Office 2013 på RDS-distribusjoner (Remote Desktop Services), bør du vurdere å aktivere ADAL ved å redigere registeret.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100771"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Feil under aktivering Office 2013 på eksterne skrivebordstjenester

Hvis du får en feilmelding mens du aktiverer Office 2013 på RDS-distribusjoner (Remote Desktop Services), bør du vurdere å aktivere ADAL ved å redigere registeret.
  
|**Registernøkkel**|**Type**|**Verdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Hvis du vil ha mer informasjon, kan du [se Aktivere moderne godkjenning for Office 2013 på Windows enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL er aktivert som standard i Microsoft 365 Apps for enterprise og Office 2016. Remote Desktop Services (RDS) ble tidligere kalt Terminal Services.
  