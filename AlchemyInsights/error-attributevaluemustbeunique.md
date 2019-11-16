---
title: Feil AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "36527029"
---
# <a name="error-attributevaluemustbeunique"></a>Feil: AttributeValueMustBeUnique

Den vanligste årsaken til AttributeValueMustBeUnique-feilen er to objekter med ulike SourceAnchor (immutableId) har samme verdi for physicalDeliveryOfficeName og/eller UserPrincipalName-attributter. Slik reparerer du AttributeValueMustBeUnique-feilen:
  
1. Identifiser den dupliserte physicalDeliveryOfficeName, userPrincipalName eller en annen attributtverdi som forårsaker feilen. Identifiser også hvilke to (eller flere) objekter som er involvert i konflikten. Rapporten som genereres av Azure AD Connect Health for synkronisering, kan hjelpe deg med å identifisere de to objektene.
    
2. Identifiser hvilket objekt som skal fortsette å ha den dupliserte verdien og hvilket objekt som ikke skal.
    
3. Fjern den dupliserte verdien fra objektet som ikke skal ha denne verdien. Merk at du bør gjøre endringen i katalogen der objektet er Hentet fra. I noen tilfeller må du kanskje slette ett av objektene i konflikt.
    
4. Hvis du har gjort endringen i lokalene AD, la Azure AD koble synkronisere endringen for feilen å få løst.
    

