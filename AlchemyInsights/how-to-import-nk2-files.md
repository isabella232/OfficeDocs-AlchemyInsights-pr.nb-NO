---
title: How-skal-import-nk2-filer
ms.author: daeite
author: daeite
manager: joallard
ms.date: 5/3/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: ed0c679cf3ed9d363e552c04a5ae6d0fc72f88dd
ms.sourcegitcommit: 6a229919cf67005e7e67841e9e45f2f3aa6833ef
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630024"
---
# <a name="how-to-import-nk2-files"></a>Hvordan du importerer .nk2-filer 

Når du starter Microsoft Outlook 2013, Outlook-2016, 2019 i Outlook eller Outlook for Office 365 for første gang, importeres i hurtigbufferen for kallenavn (lagret i *Profilnavn*nk2-filen) til en skjult melding i standard meldingslager.

Hvis du vil importere .nk2-filer til Outlook 2013, Outlook-2016, 2019 i Outlook eller Outlook til Office 365, må du kontrollere at nk2-filen er i følgende mappe: %appdata%\Microsoft\Outlook

**Merknad**: nk2-filen må ha samme navn som gjeldende profil for Outlook 2013 eller Outlook-2016. Profilnavnet er som standard "Outlook". Hvis du vil kontrollere profilnavnet, gjør du følgende: 
1. Klikk **Start**, og klikk deretter **Kontrollpanel**.
2. Dobbeltklikk **e-post**.
3. Velg **Vis profiler**i dialogboksen e-postoppsett.
4. Velg **Start** > **kjører**.
5. I **Åpne** -boksen skriver du inn *outlook.exe /importnk2*, og velg deretter **OK**. 

Når du importerer .nk2-fil, flettes innholdet i filen til den eksisterende hurtigbufferen for kallenavn er lagret i postboksen.

**Merknad**: nk2-filen har fått nytt navn med filtypen OLD neste gang du starter Outlook 2013, Outlook-2016, 2019 i Outlook eller Outlook for Office 365. Hvis du Importer nk2-filen på nytt, må du fjerne filtypen OLD først.

Hvis du vil ha mer informasjon, kan du se [importere eller kopiere Autofullfør-listen til en annen datamaskin](https://support.microsoft.com/en-us/help/2806550/how-to-import-nk2-files-into-outlook%).