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
description: Hvis du får en feil melding når du aktiverer Office 2013 på RDS-distribusjoner (Remote Desktop Services), kan du vurdere å aktivere ADAL ved å redigere registeret.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709196"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Feil under aktivering av Office 2013 på eksterne skrive bords tjenester

Hvis du får en feil melding når du aktiverer Office 2013 på RDS-distribusjoner (Remote Desktop Services), kan du vurdere å aktivere ADAL ved å redigere registeret.
  
|**Registernøkkel**|**Type**|**Verdi**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Hvis du vil ha mer informasjon, kan du se [aktivere moderne godkjenning for Office 2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL er aktivert som standard i Microsoft 365-apper for Enterprise og Office 2016. Remote Desktop Services (RDS) har tidligere fått navnet Terminal Services.
  