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
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813769"
---
# <a name="error-attributevaluemustbeunique"></a>Feil: AttributeValueMustBeUnique

Den vanligste årsaken til AttributeValueMustBeUnique-feilen er to objekter med forskjellig SourceAnchor (uforanderligId) har samme verdi for ProxyAddresses- og/eller UserPrincipalName-attributtene. Slik løser du AttributeValueMustBeUnique-feilen:
  
1. Identifiser de dupliserte proxyAddresses, userPrincipalName eller en annen attributtverdi som forårsaker feilen. Identifiser også hvilke to (eller flere) objekter som er involvert i konflikten. Rapporten som genereres av Azure AD Connect Health for synkronisering, kan hjelpe deg med å identifisere de to objektene.
    
2. Identifiser hvilket objekt som skal fortsette å ha den dupliserte verdien, og hvilket objekt som ikke skal det.
    
3. Fjern den dupliserte verdien fra objektet som IKKE skal ha denne verdien. Vær oppmerksom på at du bør gjøre endringen i katalogen der objektet er hentet fra. I noen tilfeller må du kanskje slette et av objektene i konflikt.
    
4. Hvis du har gjort endringen i den lokale AD-en, kan du la Azure AD Connect synkronisere endringen for at feilen skal bli løst.
    

