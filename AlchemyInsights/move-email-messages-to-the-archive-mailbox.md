---
title: Flytte e-postmeldinger i postboksen arkiv
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941723"
---
Har problemer med arkiveringen elementer til arkiv-postboks. Kontroller at du har utført trinnene nedenfor:
  
1. Bekreft at en **Arkiver postboks** er aktivert. Hvis ikke, kan du bruke fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til å aktivere arkiv-postboks. 
    
2. Opprett en **kode for oppbevaring** med handlingen **Gå til arkiv** som inneholder ønsket **Oppbevaring alder**i Exchange administrasjonssenteret, velg **Oppbevaring koder** under **Behandling av overholdelse**.
    
3. I administrasjonssenteret for Exchange velger **Oppbevaringspolicyer**, opprette en **Oppbevaringspolicy** og legge til din **flytte til** oppbevaring-ID i policyen. 
    
4. [Tilordne oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til bestemte brukerens postboks. Policyen om samme gjelder både **Primær** og **Arkiv** -postboks. 
    
Brukerens postboks har nå en arkiveringspolicy til å flytte elementer til arkiv-postboks. Det kan være nødvendig å tvinge den administrerte mappen hjelperen (MFA) til å kjøre og bruke de nye innstillingene i brukerens postboks. Kjør følgende kommando når du [er koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) å starte administrert Mappeassistent for en bestemt postboks: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Vil ha mer informasjon om hvordan du konfigurerer en arkiveringspolicy for, kan du se [Konfigurere en policy for arkivering og sletting for postbokser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

