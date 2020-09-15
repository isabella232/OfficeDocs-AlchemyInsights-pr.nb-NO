---
title: Deling med eksterne brukere fungerer ikke
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691584"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løse problemer med å dele SharePoint-innhold med eksterne brukere

Kontroller at ekstern deling er aktivert for organisasjonen din:
  
1. Gå til [siden tjenester &amp; -tillegg i administrasjons senteret for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **områder**.
    
2. Kontroller at innstillingen er slått på. Hvis det er merket av for bare eksisterende eksterne brukere, må du kontrollere at den eksterne brukeren er oppført i administrasjons senteret for Microsoft 365.
    
Kontroller at ekstern deling den er slått på for området. For en klassisk område samling:
  
1. Klikk **områder**i den venstre ruten i det nye administrasjons senteret for SharePoint.
    
2. Velg nettstedet eller nett stedene, og klikk **deling**på båndet.
    
For et gruppe nettsted som tilhører en Microsoft 365-gruppe eller et kommunikasjons område:
  
- Disse nye område typene har samme Delings innstilling som hele organisasjonen, med mindre innstillingen for hele organisasjonen tillater deling av filer ved hjelp av koblinger som ikke krever pålogging. I dette tilfellet tillater områdene deling med nye og eksisterende eksterne brukere som logger seg på. Hvis du vil endre innstillingen for bestemte nett steder, bruker du det nye administrasjons senteret for SharePoint eller PowerShell. [Finn ut mer](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Innstillingen for ekstern deling for et nettsted kan være mer begrenset enn organisasjonens omfattende innstilling, men ikke mer tolerant enn innstillingen for hele organisasjonen. 
  

