---
title: UPN-synkronisering deaktivert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749523"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="1d491-102">UPN-synkronisering deaktivert</span><span class="sxs-lookup"><span data-stu-id="1d491-102">UPN sync disabled</span></span>

<span data-ttu-id="1d491-103">Hvis du har begynt å synkronisere til Azure AD før 30. mars 2016, kan du kjøre følgende Azure AD PowerShell-cmdlet for å aktivere UPN-samsvar for bare din organisasjon:</span><span class="sxs-lookup"><span data-stu-id="1d491-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="1d491-104">**Set-MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-enable $True**</span><span class="sxs-lookup"><span data-stu-id="1d491-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="1d491-105">Myk samsvar for UPN aktiveres automatisk for organisasjoner som startet synkronisering til Azure AD på eller etter 30. mars 2016.</span><span class="sxs-lookup"><span data-stu-id="1d491-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="1d491-106">Hvis du vil lære mer om hvordan du aktiverer myk samsvar for UPN-og andre synkroniserings funksjoner, kan du se [funksjoner for Azure ad Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="1d491-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

