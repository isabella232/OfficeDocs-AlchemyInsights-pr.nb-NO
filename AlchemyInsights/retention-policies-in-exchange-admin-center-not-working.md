---
title: Oppbevaringspolicyer i Exchange administrasjonssenteret fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551352"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Oppbevaringspolicyer i Exchange administrasjonssenteret

 **Problem:** Opprettet nylig eller oppdatert oppbevaringspolicyer i administrasjonssenteret Exchange er ikke å bruke på postbokser eller varer ikke flyttes til arkiv-postboks eller slettet. 
  
 **Årsaker:**
  
- Dette kan være fordi den **Administrerte Mappeassistent** ikke behandlet brukerens postboks. Administrerte Mappeassistent prøver å behandle hver postboks i organisasjonen \\\cloud-based én gang hver sjuende dag. Hvis du endrer en kode for oppbevaring, eller bruke en annen oppbevaringspolicy på en postboks, kan du vente til den administrerte mappen hjelpe behandler postboksen, eller du kan kjøre cmdleten Start-ManagedFolderAssistant for å starte administrert Mappeassistent for å behandle en bestemt postboks. Kjøre denne cmdleten er nyttig for testing eller feilsøke en oppbevaringspolicy eller innstillingene for oppbevaring av koden. Hvis du vil ha mer informasjon, kan du gå til [kjører forvaltet Mappeassistent](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kjør følgende kommando for å starte administrert Mappeassistent for en bestemt postboks:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også være skje hvis **RetentionHold** er **aktivert** for postboksen. Hvis postboksen er plassert i en RetentionHold, behandles ikke oppbevaringspolicy på postboksen i løpet av denne tiden. For mer dataarkiveringsløsninger på RetentionHold innstillingen se: [Postboks oppbevaring Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Løsning:**
    
  - Kontrollere statusen for RetentionHold-innstillingen i den bestemte postboksen i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
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
 
For mer informasjon om oppbevaringspolicyer i administrasjonssenteret Exchange, kan du se:
- [Koder for oppbevaring og oppbevaringspolicyer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Bruk en oppbevaringspolicy på postbokser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Legge til eller fjerne koder for oppbevaring](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Slik identifiserer du typen sperring som er plassert på en postboks](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
