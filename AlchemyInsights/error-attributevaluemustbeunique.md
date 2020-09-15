---
title: Feil AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709160"
---
# <a name="error-attributevaluemustbeunique"></a>Feil: AttributeValueMustBeUnique

Den vanligste årsaken til AttributeValueMustBeUnique-feilen er to objekter med ulike SourceAnchor (immutableId) har samme verdi for ProxyAddresses-og/eller UserPrincipalName-attributtene. Slik løser du AttributeValueMustBeUnique-feilen:
  
1. Identifiser den dupliserte proxyAddresses, userPrincipalName eller en annen attributtverdi som for år saker feilen. Du kan også identifisere hvilke to (eller flere) objekter som er involvert i konflikten. Rapporten som genereres av Azure AD Connect-tilstanden for synkronisering, kan hjelpe deg med å identifisere de to objektene.
    
2. Identifisere hvilket objekt som skal fortsette å ha den dupliserte verdien, og hvilket objekt som ikke skal være.
    
3. Fjern den dupliserte verdien fra objektet som ikke skal ha den verdien. Vær oppmerksom på at du bør gjøre endringen i katalogen der objektet er kilde. I noen tilfeller må du kanskje slette en av de andre objektene i konflikt.
    
4. Hvis du har gjort endringen i den lokale ANNONSEN, kan du la Azure AD Connect synkronisere endringen for å løse problemet.
    

