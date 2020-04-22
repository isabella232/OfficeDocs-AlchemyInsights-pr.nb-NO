---
title: UPN-synkronisering deaktivert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726113"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering deaktivert

Hvis du begynte å synkronisere med Azure AD før 30.
  
 **Set-MsolDirSyncFeature --funksjonen EnableSoftMatchOnUpn -Aktiver $True**
  
UPN soft match aktiveres automatisk for organisasjoner som begynte å synkronisere til Azure AD på eller etter 30.
  
Hvis du vil vite mer om hvordan du aktiverer myk samsvar på UPN og andre synkroniseringsfunksjoner, kan du se [Azure AD Connect synkroniseringstjenestefunksjoner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

