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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910375"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løse problemer med deling SharePoint innhold med eksterne brukere

Kontroller at ekstern deling er aktivert for organisasjonen:
  
1. Gå til [ &amp; Tjenester-tillegg-siden i Administrasjonssenter for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **Nettsteder**.
    
2. Kontroller at innstillingen er slått til På. Hvis Bare eksisterende eksterne brukere er valgt, må du kontrollere at den eksterne brukeren er oppført i Administrasjonssenter for Microsoft 365.
    
Kontroller at ekstern deling er aktivert for nettstedet. For en klassisk nettstedssamling:
  
1. Klikk områder SharePoint i den venstre ruten i det nye **administrasjonssenteret.**
    
2. Velg nettstedet eller nettstedene, og klikk Deling på **båndet.**
    
For et gruppenettsted som tilhører en Microsoft 365 gruppe eller et kommunikasjonsnettsted:
  
- Disse nye nettstedstypene har samme delingsinnstilling som innstillingen for hele organisasjonen, med mindre innstillingen for hele organisasjonen tillater deling av filer ved hjelp av koblinger som ikke krever pålogging. I dette tilfellet tillater nettstedene deling med nye og eksisterende eksterne brukere som logger på. Hvis du vil endre innstillingen for bestemte nettsteder, bruker du det nye SharePoint eller PowerShell. [Finn ut mer](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Innstillingen for ekstern deling for alle områder kan være mer restriktiv enn innstillingen for hele organisasjonen, men ikke mer tillatt enn innstillingen for hele organisasjonen. 
  

