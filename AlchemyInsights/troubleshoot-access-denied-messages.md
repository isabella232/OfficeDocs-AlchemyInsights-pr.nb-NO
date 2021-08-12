---
title: Feilsøke meldinger som ikke får tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939892"
---
# <a name="troubleshoot-access-denied-messages"></a>Feilsøke meldinger som ikke får tilgang

Hvis noen fikk meldingen Ingen tilgang til en delt mappe i SharePoint, kan administratoren for nettstedssamlingen ha aktivert låsemodus for brukertillatelse med begrenset tilgang. Slik deaktiverer du dette: 
  
1. Bla til nettstedet, klikk ikonet Innstillinger, og klikk **deretter** Innstillinger .
    
2. Klikk **Funksjoner for nettstedssamling** under Administrasjon av **nettstedssamling**.
    
3. Klikk Deaktiver ved siden **av Modus for** låsing av brukertillatelse med begrenset **tilgang.**
    
Meldingen Ingen tilgang kan også oppstå for delte mapper hvis nettstedet er et publiseringsnettsted. Hvis du vil ha informasjon, [kan du se Ingen tilgang når du åpner en delt mappe](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
Hvis en person fikk meldingen Ingen tilgang når de prøver å vise tilgangsforespørsler, må brukeren legges til som enten administrator for nettstedssamlingen eller medlem av Eiere-gruppen for området. Hvis du vil ha mer informasjon, [kan du se Listen Ingen tilgang til tilgangsforespørsler](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Hvis en bruker fikk meldingen Ingen tilgang etter at de ble fjernet fra Active Directory lokalt og deretter lagt til igjen, kan du se Ingen tilgang når en [brukerkonto synkroniseres til Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

