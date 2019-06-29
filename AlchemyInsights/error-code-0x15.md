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
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388254"
---
<span data-ttu-id="8bec8-103">Hvis du får en feil under aktivering av Office 2013 på Remote Desktop Services (RDS)-distribusjoner, kan du vurdere å gi ADAL ved å redigere registret.</span><span class="sxs-lookup"><span data-stu-id="8bec8-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="8bec8-104">**Registernøkkel**</span><span class="sxs-lookup"><span data-stu-id="8bec8-104">**Registry key**</span></span>|<span data-ttu-id="8bec8-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="8bec8-105">**Type**</span></span>|<span data-ttu-id="8bec8-106">**Verdi**</span><span class="sxs-lookup"><span data-stu-id="8bec8-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8bec8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="8bec8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="8bec8-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="8bec8-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="8bec8-109">1</span><span class="sxs-lookup"><span data-stu-id="8bec8-109">1</span></span>  <br/> |

<span data-ttu-id="8bec8-110">Hvis du vil ha mer informasjon, se [Aktivere moderne godkjenning for 2013 Office på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="8bec8-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="8bec8-111">ADAL er aktivert som standard i Office 365 ProPlus og Office-2016.</span><span class="sxs-lookup"><span data-stu-id="8bec8-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="8bec8-112">> remote Desktop Services (RDS) ble tidligere kalt Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="8bec8-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  