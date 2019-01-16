---
title: Feilkode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Hvis du får en feil under aktivering av Office 2013 på Remote Desktop Services (RDS)-distribusjoner, kan du vurdere å gi ADAL ved å redigere registret.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303110"
---
Hvis du får en feil under aktivering av Office 2013 på Remote Desktop Services (RDS)-distribusjoner, kan du vurdere å gi ADAL ved å redigere registret. 
  
|**Registernøkkel**|**Type**|**Verdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Hvis du vil ha mer informasjon, se [Aktivere moderne godkjenning for 2013 Office på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL er aktivert som standard i Office 365 ProPlus og Office-2016. > Remote Desktop Services (RDS) ble tidligere kalt Terminal Services. 
  

