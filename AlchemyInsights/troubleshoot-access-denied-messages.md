---
title: Feilsøke meldinger om ingen tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690792"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="ca054-102">Feilsøke meldinger om ingen tilgang</span><span class="sxs-lookup"><span data-stu-id="ca054-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="ca054-103">Hvis noen har fått meldingen «ingen tilgang» til en delt mappe i SharePoint, kan det hende at administratoren for nettsteds samlingen har aktivert modus for låsing av begrenset tilgang for bruker tillatelser.</span><span class="sxs-lookup"><span data-stu-id="ca054-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="ca054-104">Slik slår du av dette:</span><span class="sxs-lookup"><span data-stu-id="ca054-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="ca054-105">Gå til nettstedet, klikk Innstillinger-ikonet, og klikk deretter **Innstillinger for område**.</span><span class="sxs-lookup"><span data-stu-id="ca054-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="ca054-106">Klikk **funksjoner for område samling**under **administrasjon av område samling**.</span><span class="sxs-lookup"><span data-stu-id="ca054-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="ca054-107">Klikk **Deaktiver**ved siden av **låse modus for bruker tillatelse ved begrenset tilgang**.</span><span class="sxs-lookup"><span data-stu-id="ca054-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="ca054-108">Meldingen ingen tilgang kan også forekomme for delte mapper hvis området er et publiserings område.</span><span class="sxs-lookup"><span data-stu-id="ca054-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="ca054-109">Hvis du vil ha informasjon, kan du se [tilgang nektet ved tilgang til en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="ca054-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="ca054-110">Hvis en person har fått meldingen «ingen tilgang» når du prøver å vise tilgangs forespørsler, må brukeren legges til som enten en administrator for område samling eller medlem av eiere-gruppen for nettstedet.</span><span class="sxs-lookup"><span data-stu-id="ca054-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="ca054-111">Hvis du vil ha mer informasjon, kan du se [tilgang nektet tilgang til forespørsels listen](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="ca054-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="ca054-112">Hvis en bruker fikk meldingen «ingen tilgang» etter at de ble fjernet fra Active Directory lokalt og deretter lagt til på nytt, kan du se ingen [tilgang når en bruker konto synkroniseres til Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="ca054-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

