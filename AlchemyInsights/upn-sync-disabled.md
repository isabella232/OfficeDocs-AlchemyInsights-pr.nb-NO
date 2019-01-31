---
title: UPN-sync deaktivert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657980"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="54dfc-102">UPN-sync deaktivert</span><span class="sxs-lookup"><span data-stu-id="54dfc-102">UPN sync disabled</span></span>

<span data-ttu-id="54dfc-103">Hvis du startet synkronisering til Azure AD før 30. mars 2016, kjører du følgende Azure AD PowerShell-cmdleten for å aktivere nedlastbare UPN som passer til din organisasjon bare:</span><span class="sxs-lookup"><span data-stu-id="54dfc-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="54dfc-104">**Sett MsolDirSyncFeature-funksjonen er EnableSoftMatchOnUpn-Aktiver $True**</span><span class="sxs-lookup"><span data-stu-id="54dfc-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="54dfc-105">UPN myke treff er automatisk aktivert for organisasjoner som startet synkronisering til Azure AD på eller etter 30. mars 2016.</span><span class="sxs-lookup"><span data-stu-id="54dfc-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="54dfc-106">Hvis du vil ha mer informasjon om hvordan du aktiverer myke treff på UPN og andre synkroniseringsfunksjoner som, kan du se [koble til Azure AD service synkroniseringsfunksjoner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="54dfc-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

