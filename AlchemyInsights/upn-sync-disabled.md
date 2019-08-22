---
title: UPN-sync deaktivert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532340"
---
# <a name="upn-sync-disabled"></a>UPN-sync deaktivert

Hvis du startet synkronisering til Azure AD før 30. mars 2016, kjører du følgende Azure AD PowerShell-cmdleten for å aktivere nedlastbare UPN som passer til din organisasjon bare:
  
 **Sett MsolDirSyncFeature-funksjonen er EnableSoftMatchOnUpn-Aktiver $True**
  
UPN myke treff er automatisk aktivert for organisasjoner som startet synkronisering til Azure AD på eller etter 30. mars 2016.
  
Hvis du vil ha mer informasjon om hvordan du aktiverer myke treff på UPN og andre synkroniseringsfunksjoner som, kan du se [koble til Azure AD service synkroniseringsfunksjoner](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

