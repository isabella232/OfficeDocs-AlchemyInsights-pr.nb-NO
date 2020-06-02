---
title: Feilkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du får en feilmelding mens du aktiverer Office 2013 på distribusjoner av Remote Desktop Services (RDS), kan du vurdere å aktivere ADAL ved å redigere registret.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506855"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Feil under aktivering av Office 2013 på Remote Desktop Services

Hvis du får en feilmelding mens du aktiverer Office 2013 på distribusjoner av Remote Desktop Services (RDS), kan du vurdere å aktivere ADAL ved å redigere registret.
  
|**Registernøkkel**|**Type**|**Verdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Hvis du vil ha mer informasjon, kan du se [Aktivere moderne godkjenning for Office-2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL er aktivert som standard i Microsoft 365 Apps for enterprise og Office 2016. Remote Desktop Services (RDS) ble tidligere kalt Terminal Services.
  