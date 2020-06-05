---
title: Deling med eksterne brukere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582784"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løse problemer med å dele SharePoint-innhold med eksterne brukere

Kontroller at ekstern deling er aktivert for organisasjonen:
  
1. Gå til [ &amp; siden Tjenester-tillegg i administrasjonssenteret for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **Områder**.
    
2. Kontroller at innstillingen er slått til "På". Hvis "Bare eksisterende eksterne brukere" er valgt, må du kontrollere at den eksterne brukeren er oppført i administrasjonssenteret for Microsoft 365.
    
Kontroller at ekstern deling den er aktivert for området. For en klassisk områdesamling:
  
1. Klikk **områder**i ruten til venstre i det nye administrasjonssenteret for SharePoint.
    
2. Velg området eller områdene, og klikk **Deling**på båndet.
    
For et gruppeområde som tilhører en Microsoft 365-gruppe eller et kommunikasjonsområde:
  
- Disse nye områdetypene har samme delingsinnstilling som innstillingen for hele organisasjonen, med mindre innstillingen for hele organisasjonen tillater deling av filer ved hjelp av koblinger som ikke krever pålogging. I dette tilfellet tillater nettstedene deling med nye og eksisterende eksterne brukere som logger på. Hvis du vil endre innstillingen for bestemte områder, kan du bruke det nye administrasjonssenteret for SharePoint eller PowerShell. [Finn ut mer](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Innstillingen for ekstern deling for et hvilket som helst område kan være mer restriktiv enn innstillingen for hele organisasjonen, men ikke mer tillatt enn innstillingen for hele organisasjonen. 
  

