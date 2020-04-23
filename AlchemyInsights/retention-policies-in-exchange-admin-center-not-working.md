---
title: Oppbevaringspolicyer i Administrasjonssenter for Exchange fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742442"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Oppbevaringspolicyer i administrasjonssenteret for Exchange

 **Problem:** Nylig opprettede eller oppdaterte oppbevaringspolicyer i Administrasjonssenter for Exchange gjelder ikke for postbokser eller elementer flyttes ikke til arkivpostboksen eller slettes. 
  
 **Grunnårsaker:**
  
- Dette kan skyldes at **hjelperen for administrerte mapper** ikke har behandlet brukerens postboks. Hjelperen for administrert mappe prøver å behandle alle postbokser i den skybaserte organisasjonen én gang hver sjuende dag. Hvis du endrer en oppbevaringskode eller bruker en annen oppbevaringspolicy på en postboks, kan du vente til administrertmappeassisten behandler postboksen, eller du kan kjøre cmdleten Start-ManagedFolderAssistant for å starte administrert mappeassistent for å behandle en bestemt postboks. Kjøring av denne cmdleten er nyttig for testing eller feilsøking av en oppbevaringspolicy eller innstillinger for oppbevaringskode. Hvis du vil ha mer informasjon, kan du gå [til Kjør assistenten for administrertmappe](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kjør følgende kommando for å starte administrert mappeassistent for en bestemt postboks:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også skje hvis **RetentionHold** er **aktivert** i postboksen. Hvis postboksen er plassert på en OppbevaringHold, behandles ikke oppbevaringspolicyen på postboksen i løpet av den tiden. Hvis du vil ha mer informasjon om oppbevaringshold-innstillingen, kan du se: [Oppbevaringssperre for postboks](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Løsning:**
    
  - Kontroller statusen for RetentionHold-innstillingen på den bestemte postboksen i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kjør følgende kommando for å **deaktivere** RetentionHold på en bestemt postboks:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Kjør nå assistenten for administrerte mapper på nytt:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Merk:** Hvis en postboks er mindre enn 10 MB, behandler ikke hjelperen for administrertmappe automatisk postboksen.
 
Hvis du vil ha mer informasjon om oppbevaringspolicyer i administrasjonssenteret for Exchange, kan du se:
- [Oppbevaringskoder og oppbevaringspolicyer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Bruke en oppbevaringspolicy på postbokser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Legge til eller fjerne oppbevaringskoder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Slik identifiserer du typen sperring plassert på en postboks](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
