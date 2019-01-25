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
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481738"
---
# <a name="upn-sync-disabled"></a>UPN-sync deaktivert

Hvis du startet synkronisering til Azure AD før 30. mars 2016, kjører du følgende Azure AD PowerShell-cmdleten for å aktivere nedlastbare UPN som passer til din organisasjon bare:
  
 **Sett MsolDirSyncFeature-funksjonen er EnableSoftMatchOnUpn-Aktiver $True**
  
UPN myke treff er automatisk aktivert for organisasjoner som startet synkronisering til Azure AD på eller etter 30. mars 2016.
  
Hvis du vil ha mer informasjon om hvordan du aktiverer myke treff på UPN og andre synkroniseringsfunksjoner som, kan du se [koble til Azure AD service synkroniseringsfunksjoner](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

