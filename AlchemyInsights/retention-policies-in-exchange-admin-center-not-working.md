---
title: Oppbevaringspolicyer i Exchange administrasjonssenteret fungerer ikke
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28302589"
---
 **Problem:** Opprettet nylig eller oppdatert oppbevaringspolicyer i administrasjonssenteret Exchange er ikke å bruke på postbokser eller varer ikke flyttes til arkiv-postboks eller slettet. 
  
 **Årsaker:**
  
- Dette kan være fordi den **Administrerte Mappeassistent** ikke behandlet brukerens postboks. Administrerte Mappeassistent prøver å behandle hver postboks i organisasjonen \\\cloud-based én gang hver sjuende dag. Hvis du endrer en kode for oppbevaring, eller bruke en annen oppbevaringspolicy på en postboks, kan du vente til den administrerte mappen hjelpe behandler postboksen, eller du kan kjøre cmdleten Start-ManagedFolderAssistant for å starte administrert Mappeassistent for å behandle en bestemt postboks. Kjøre denne cmdleten er nyttig for testing eller feilsøke en oppbevaringspolicy eller innstillingene for oppbevaring av koden. Hvis du vil ha mer informasjon, kan du gå til [kjører forvaltet Mappeassistent](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kjør følgende kommando for å starte administrert Mappeassistent for en bestemt postboks: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også være skje hvis **RetentionHold** er **aktivert** for postboksen. Hvis postboksen er plassert i en RetentionHold, behandles ikke oppbevaringspolicy på postboksen i løpet av denne tiden. For mer dataarkiveringsløsninger på RetentionHold innstillingen se: [Postboks oppbevaring Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Løsning:**
    
  - Kontrollere statusen for RetentionHold-innstillingen i den bestemte postboksen i [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kjør følgende kommando for å **deaktivere** RetentionHold på en bestemt postboks: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Nå, kjøre den administrerte mappen hjelperen på nytt:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Merk:** Hvis en postboks er mindre enn 10 MB, behandler administrert Mappeassistent automatisk ikke postboksen. 
  

