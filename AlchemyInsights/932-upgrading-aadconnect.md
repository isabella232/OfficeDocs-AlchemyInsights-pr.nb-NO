---
title: 932 oppgraderer AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937953"
---
# <a name="upgrade-azure-ad-connect"></a>Oppgradering Azure AD koble

Som standard aktiveres automatisk oppgradering for Azure AD-tilkobling, som bidrar til å sikre at du kjører den nyeste versjonen. Hvis du vil kontrollere innstillingene for automatisk oppgradering, kan du bruke cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdleten vil returnere en av følgende verdier: 
  
- **Aktivert**: automatisk oppgradering er aktivert. 
    
- **Deaktivert**: automatisk oppgradering er deaktivert. 
    
- **Suspended**: systemet er ikke lenger berettiget til å motta automatiske oppgraderinger. Du kan ikke konfigurere denne verdien. Det er satt av systemet. 
    
Hvis du vil ha mer informasjon, kan du se [automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).
  
Hvis du vil laste ned den nyeste versjonen av Azure AD-tilkobling, kan du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
  

