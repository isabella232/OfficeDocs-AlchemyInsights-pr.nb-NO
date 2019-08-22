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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="f2a9b-103">Feil under aktivering Office 2013 på eksterne skrivebordstjenester</span><span class="sxs-lookup"><span data-stu-id="f2a9b-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="f2a9b-104">Hvis du får en feil under aktivering av Office 2013 på Remote Desktop Services (RDS)-distribusjoner, kan du vurdere å gi ADAL ved å redigere registret.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="f2a9b-105">**Registernøkkel**</span><span class="sxs-lookup"><span data-stu-id="f2a9b-105">**Registry key**</span></span>|<span data-ttu-id="f2a9b-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="f2a9b-106">**Type**</span></span>|<span data-ttu-id="f2a9b-107">**Verdi**</span><span class="sxs-lookup"><span data-stu-id="f2a9b-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f2a9b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="f2a9b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="f2a9b-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="f2a9b-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="f2a9b-110">1</span><span class="sxs-lookup"><span data-stu-id="f2a9b-110">1</span></span>  <br/> |

<span data-ttu-id="f2a9b-111">Hvis du vil ha mer informasjon, se [Aktivere moderne godkjenning for 2013 Office på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="f2a9b-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="f2a9b-112">ADAL er aktivert som standard i Office 365 ProPlus og Office-2016.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="f2a9b-113">Remote Desktop Services (RDS) ble tidligere kalt Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  