---
title: Feil attributtVerdi må væreunik
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703183"
---
# <a name="error-attributevaluemustbeunique"></a>Feil: AttributeValuemustbeUnique

Den vanligste årsaken til AttributtverdiMustBeUnique-feilen er to objekter med forskjellige SourceAnchor (immutableId) har samme verdi for Attributtadressene og/eller UserPrincipalName-attributtene. Slik løser du AttributtverdiMustBeUnique-feilen:
  
1. Identifiser dupliserte proxy-adresser, userPrincipalName eller annen attributtverdi som forårsaker feilen. Identifiser også hvilke to (eller flere) objekter som er involvert i konflikten. Rapporten som genereres av Azure AD Connect Health for synkronisering, kan hjelpe deg med å identifisere de to objektene.
    
2. Identifiser hvilket objekt som skal fortsette å ha den dupliserte verdien, og hvilket objekt som ikke skal.
    
3. Fjern den dupliserte verdien fra objektet som IKKE skal ha denne verdien. Vær oppmerksom på at du bør gjøre endringen i katalogen der objektet er hentet fra. I noen tilfeller må du kanskje slette ett av objektene i konflikt.
    
4. Hvis du gjorde endringen i den lokale AD, kan du la Azure AD Connect synkronisere endringen for at feilen skal bli løst.
    

