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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207694"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Løse problemer med å dele SharePoint-innhold med eksterne brukere

Kontroller at eksterne deling er aktivert for organisasjonen:
  
1. Gå til den [tjenester &amp; tillegg side i administrasjonssenteret for Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), og klikk **områder**.
    
2. Kontroller at innstillingen slås til "On". Hvis "Bare eksisterende eksterne brukere" er valgt, må du kontrollere at den eksterne brukeren er oppført i administrasjonssenteret for Microsoft 365.
    
Kontroller at eksternt delingen som er aktivert for området. For en klassisk områdesamling:
  
1. Klikk **områdesamlinger**i klassisk SharePoint administrasjonssenteret, i ruten til venstre.
    
2. Velg område eller områder, og klikk **Deling**på båndet.
    
For et gruppeområde som tilhører en gruppe for Office 365, eller et område for kommunikasjon:
  
- Slike området har den samme delte innstillingen som innstilling for bedriften, med mindre innstillingen for hele organisasjonen kan dele filer ved hjelp av koblinger som ikke krever pålogging. I dette tilfellet Tillat områdene deling med nye og eksisterende eksterne brukere som logger på. Hvis du vil endre innstillingen for bestemte områder, bruke den nye SharePoint-administrasjonssenteret (forhåndsvisning) eller PowerShell. [Lær mer](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Eksterne delte innstillingen for et område kan være mer restriktive enn innstillingene for hele organisasjonen, men ikke mer tillatte DACLer enn innstillingen for hele organisasjonen. 
  

