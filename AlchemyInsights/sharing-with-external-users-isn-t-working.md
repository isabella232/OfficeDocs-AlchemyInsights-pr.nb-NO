---
title: Deling med eksterne brukere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502240"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løs problemer med deling av SharePoint-innhold med eksterne brukere

Kontroller at ekstern deling er slått på for organisasjonen:
  
1. Gå til [siden tjenester &amp; -tillegg i administrasjonssenteret for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **områder**.
    
2. Kontroller at innstillingen er slått på "på". Hvis "bare eksisterende eksterne brukere" er valgt, må du kontrollere at den eksterne brukeren er oppført i administrasjonssenteret for Microsoft 365.
    
Kontroller at ekstern deling den er slått på for området. For en klassisk områdesamling:
  
1. Klikk **områder**i ruten til venstre i det nye administrasjonssenteret for SharePoint.
    
2. Velg området eller områdene, og klikk **deling**på båndet.
    
For et gruppeområde som tilhører en Office 365-gruppe, eller et område for kommunikasjon:
  
- Disse nye områdetypene har samme Delings innstilling som innstillingen for hele organisasjonen, med mindre innstillingen for hele organisasjonen tillater deling av filer ved hjelp av koblinger som ikke krever pålogging. I dette tilfellet tillater områdene deling med nye og eksisterende eksterne brukere som logger på. Hvis du vil endre innstillingen for bestemte områder, kan du bruke det nye administrasjonssenteret for SharePoint eller PowerShell. [Finn ut mer](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Innstillingen for ekstern deling for et hvilket som helst område kan være mer begrenset enn innstillingen for hele organisasjonen, men ikke mer ettergivende enn innstillingen for hele organisasjonen. 
  

