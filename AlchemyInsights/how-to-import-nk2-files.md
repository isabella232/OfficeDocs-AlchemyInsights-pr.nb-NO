---
title: slik importerer du-nk2-filer
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043215"
---
# <a name="how-to-import-nk2-files"></a>Slik importerer du NK2-filer 

Når du starter Microsoft Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook for Microsoft 365 for første gang, importeres hurtigbufferen for kallenavnet (lagret i NK2-filen for profilnavn) til en skjult melding i standard meldingslageret.

Hvis du vil importere NK2-filer til Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook for Microsoft 365, må du kontrollere at NK2-filen er i følgende mappe: %appdata%\Microsoft\Outlook

**Obs!** NK2-filen må ha samme navn som gjeldende Outlook 2013 eller Outlook 2016 profil. Som standard er profilnavnet «Outlook». Følg disse trinnene for å kontrollere profilnavnet: 
1. Klikk **Start** og deretter **Kontrollpanel**.
2. Dobbeltklikk **E-post**.
3. Velg Vis profiler i dialogboksen Oppsett av **e-post.**
4. Velg **Start** > **Kjør**.
5. Skriv inn **outlook.exe** */importnk2* i Åpne-boksen, og velg deretter **OK**. 

Når du har importert NK2-filen, flettes innholdet i filen inn i den eksisterende hurtigbufferen for kallenavn som er lagret i postboksen.

**Obs!** NK2-filen får nytt navn med filtypen .old neste gang du starter Outlook 2013, Outlook 2016, Outlook 2019 eller Outlook for Microsoft 365. Hvis du vil importere NK2-filen på nytt, fjerner du den gamle filtypen først.

Hvis du vil ha mer informasjon, kan du [se Importere eller kopiere listen for autofullfør til en annen datamaskin](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).