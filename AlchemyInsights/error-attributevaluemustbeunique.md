---
title: Feil AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002129"
---
# <a name="error-attributevaluemustbeunique"></a>Feil: AttributeValueMustBeUnique

Den vanligste årsaken til AttributeValueMustBeUnique-feilen er to objekter med forskjellig SourceAnchor (uforanderligId) har samme verdi for ProxyAddresses- og/eller UserPrincipalName-attributtene. Slik løser du AttributeValueMustBeUnique-feilen:
  
1. Identifiser de dupliserte proxyAddresses, userPrincipalName eller en annen attributtverdi som forårsaker feilen. Identifiser også hvilke to (eller flere) objekter som er involvert i konflikten. Rapporten som genereres av Azure AD Koble til Health for sync, kan hjelpe deg med å identifisere de to objektene.
    
2. Identifiser hvilket objekt som skal fortsette å ha den dupliserte verdien, og hvilket objekt som ikke skal det.
    
3. Fjern den dupliserte verdien fra objektet som IKKE skal ha denne verdien. Vær oppmerksom på at du bør gjøre endringen i katalogen der objektet er hentet fra. I noen tilfeller må du kanskje slette et av objektene i konflikt.
    
4. Hvis du har gjort endringen i den lokale AD-en, kan du la Azure AD Koble til å synkronisere endringen for at feilen skal bli løst.
    

