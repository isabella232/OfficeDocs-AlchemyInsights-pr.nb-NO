---
title: Feilkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du får en feil under aktivering av Office 2013 på Remote Desktop Services (RDS)-distribusjoner, kan du vurdere å gi ADAL ved å redigere registret.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527031"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Feil under aktivering Office 2013 på eksterne skrivebordstjenester

Hvis du får en feil under aktivering av Office 2013 på Remote Desktop Services (RDS)-distribusjoner, kan du vurdere å gi ADAL ved å redigere registret.
  
|**Registernøkkel**|**Type**|**Verdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Hvis du vil ha mer informasjon, se [Aktivere moderne godkjenning for 2013 Office på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL er aktivert som standard i Office 365 ProPlus og Office-2016. Remote Desktop Services (RDS) ble tidligere kalt Terminal Services.
  