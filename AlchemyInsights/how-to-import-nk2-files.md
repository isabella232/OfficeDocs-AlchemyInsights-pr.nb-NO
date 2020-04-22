---
title: hvordan-å-importere-nk2-filer
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759341"
---
# <a name="how-to-import-nk2-files"></a>Slik importerer du NK2-filer 

Når du starter Microsoft Outlook 2013, Outlook-2016, Outlook 2019 eller Outlook for Microsoft 365 for første gang, importeres hurtigbufferen for kallenavn (lagret i *profilnavnet*NK2-filen) til en skjult melding i standard meldingslageret.

Hvis du vil importere NK2-filer til Outlook-2013, Outlook-2016, Outlook-2019 eller Outlook for Microsoft 365, må du kontrollere at NK2-filen er i følgende mappe: %appdata%\Microsoft\Outlook

**Merk:** NK2-filen må ha samme navn som gjeldende Outlook 2013- eller Outlook 2016-profil. Som standard er profilnavnet "Outlook". Hvis du vil kontrollere profilnavnet, gjør du følgende: 
1. Klikk **Start**, og klikk deretter **Kontrollpanel**.
2. Dobbeltklikk **E-post**.
3. Velg **Vis profiler**i dialogboksen Oppsett av e-post .
4. Velg **Start** > **kjør**.
5. Skriv inn *outlook.exe /importnk2*i **Åpne** -boksen, og velg deretter **OK**. 

Når du importerer NK2-filen, flettes innholdet i filen til den eksisterende hurtigbufferen for kallenavn som er lagret i postboksen.

**Merk:**.nk2 filen er omdøpt med en .old filtype neste gang du starter Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook for Microsoft 365. Hvis du vil importere NK2-filen på nytt, fjerner du den gamle filtypen først.

Hvis du vil ha mer informasjon, kan du se [Importere eller kopiere autofullføringslisten til en annen datamaskin](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).