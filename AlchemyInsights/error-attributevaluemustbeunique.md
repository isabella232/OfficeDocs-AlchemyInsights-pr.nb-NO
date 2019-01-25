---
title: Feil AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499643"
---
# <a name="error-attributevaluemustbeunique"></a>Feil: AttributeValueMustBeUnique

Den vanligste årsaken til feilen i AttributeValueMustBeUnique er to objekter med forskjellige SourceAnchor (immutableId) har samme verdi for attributtene physicalDeliveryOfficeName og/eller UserPrincipalName. Feilen kan rettes AttributeValueMustBeUnique:
  
1. Identifisere dupliserte physicalDeliveryOfficeName, userPrincipalName eller andre attributtverdi som forårsaker feilen. Også identifisere hvilke to (eller flere) objekter som er involvert i konflikten. Rapporten genereres av Azure AD koble helse for synkronisering kan hjelpe deg med å identifisere de to objektene.
    
2. Identifisere hvilket objekt som skal fortsette med den dupliserte verdien og hvilket objekt som skal ikke.
    
3. Fjern den dupliserte verdien fra objektet som ikke skal har en verdi. Legg merke til at du bør gjøre endringen i katalogen der objektet som er kilde fra. I noen tilfeller må du kanskje slette ett av objektene i konflikt.
    
4. Hvis du har gjort endringer i lokalene på Annonsen, la Azure AD koble synkronisere endringen å få løst feilen.
    

