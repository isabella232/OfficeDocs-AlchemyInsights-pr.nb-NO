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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499391"
---
<span data-ttu-id="04a83-103">Hvis du får en feil under aktivering av Office 2013 på Remote Desktop Services (RDS)-distribusjoner, kan du vurdere å gi ADAL ved å redigere registret.</span><span class="sxs-lookup"><span data-stu-id="04a83-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="04a83-104">**Registernøkkel**</span><span class="sxs-lookup"><span data-stu-id="04a83-104">**Registry key**</span></span>|<span data-ttu-id="04a83-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="04a83-105">**Type**</span></span>|<span data-ttu-id="04a83-106">**Verdi**</span><span class="sxs-lookup"><span data-stu-id="04a83-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="04a83-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="04a83-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="04a83-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="04a83-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="04a83-109">1.</span><span class="sxs-lookup"><span data-stu-id="04a83-109">1</span></span>  <br/> |
   
<span data-ttu-id="04a83-110">Hvis du vil ha mer informasjon, se [Aktivere moderne godkjenning for 2013 Office på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="04a83-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="04a83-p101">ADAL er aktivert som standard i Office 365 ProPlus og Office-2016. > remote Desktop Services (RDS) ble tidligere kalt Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="04a83-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

