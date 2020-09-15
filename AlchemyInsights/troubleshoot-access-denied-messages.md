---
title: Feilsøke meldinger om ingen tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690792"
---
# <a name="troubleshoot-access-denied-messages"></a>Feilsøke meldinger om ingen tilgang

Hvis noen har fått meldingen «ingen tilgang» til en delt mappe i SharePoint, kan det hende at administratoren for nettsteds samlingen har aktivert modus for låsing av begrenset tilgang for bruker tillatelser. Slik slår du av dette: 
  
1. Gå til nettstedet, klikk Innstillinger-ikonet, og klikk deretter **Innstillinger for område**.
    
2. Klikk **funksjoner for område samling**under **administrasjon av område samling**.
    
3. Klikk **Deaktiver**ved siden av **låse modus for bruker tillatelse ved begrenset tilgang**.
    
Meldingen ingen tilgang kan også forekomme for delte mapper hvis området er et publiserings område. Hvis du vil ha informasjon, kan du se [tilgang nektet ved tilgang til en delt mappe](https://go.microsoft.com/fwlink/?linkid=2004317).
  
Hvis en person har fått meldingen «ingen tilgang» når du prøver å vise tilgangs forespørsler, må brukeren legges til som enten en administrator for område samling eller medlem av eiere-gruppen for nettstedet. Hvis du vil ha mer informasjon, kan du se [tilgang nektet tilgang til forespørsels listen](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Hvis en bruker fikk meldingen «ingen tilgang» etter at de ble fjernet fra Active Directory lokalt og deretter lagt til på nytt, kan du se ingen [tilgang når en bruker konto synkroniseres til Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

