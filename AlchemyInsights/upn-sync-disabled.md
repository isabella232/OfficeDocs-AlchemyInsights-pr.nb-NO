---
title: UPN-synkronisering deaktivert
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782160"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering deaktivert

Hvis du begynte å synkronisere til Azure AD før 30. mars 2016, kjører du følgende Azure AD PowerShell-cmdlet for å aktivere UPN soft match bare for organisasjonen:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN soft match aktiveres automatisk for organisasjoner som begynte å synkronisere til Azure AD på eller etter 30. mars 2016.
  
Hvis du vil lære mer om hvordan du aktiverer myk samsvar på UPN og andre synkroniseringsfunksjoner, kan du se [Funksjoner for Azure AD Connect-synkroniseringstjeneste](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

