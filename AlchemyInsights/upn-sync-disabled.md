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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038121"
---
# <a name="upn-sync-disabled"></a>UPN-synkronisering deaktivert

Hvis du begynte å synkronisere til Azure AD før 30. mars 2016, kjører du følgende Azure AD PowerShell-cmdlet for å aktivere UPN soft match bare for organisasjonen:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN soft match aktiveres automatisk for organisasjoner som begynte å synkronisere til Azure AD på eller etter 30. mars 2016.
  
Hvis du vil lære mer om hvordan du aktiverer myk samsvar på UPN og andre synkroniseringsfunksjoner, kan du [se Azure AD Koble til synkroniseringstjenestefunksjoner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

