---
title: Oppbevaringspolicyer i Exchange administrasjonssenter fungerer ikke
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
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502616"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Oppbevaringspolicyer i Administrasjonssenter for Exchange

 **Utgave:** Nylig opprettede eller oppdaterte oppbevaringspolicyer i Administrasjonssenter for Exchange gjelder ikke for postbokser eller elementer flyttes ikke til arkivpostboksen eller slettes. 
  
 **Grunnårsaker:**
  
- Dette kan skyldes **at administrert mappeassistent** ikke har behandlet brukerens postboks. Administrert mappeassistent prøver å behandle hver postboks i den skybaserte organisasjonen én gang hver sjuende dag. Hvis du endrer en oppbevaringskode eller bruker en annen oppbevaringspolicy på en postboks, kan du vente til administrert mappehjelp behandler postboksen, eller du kan kjøre cmdleten Start-ManagedFolderAssistant for å starte administrertmappeassistent for å behandle en bestemt postboks. Hvis du kjører denne cmdleten, kan du prøve eller feilsøke en oppbevaringspolicy eller innstillinger for oppbevaringskode. Hvis du vil ha mer informasjon, kan du gå [til Kjør assistenten for administrerte mapper](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kjør følgende kommando for å starte administrert mappeassistent for en bestemt postboks:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også skje hvis **RetentionHold** er **aktivert** på postboksen. Hvis postboksen er plassert på en RetentionHoldhold, behandles ikke oppbevaringspolicyen på postboksen i løpet av denne tiden. Hvis du vil ha mer informasjon om oppbevaringshold-innstillingen, kan du se Postboks [oppbevaring hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Løsning:**
    
  - Kontroller statusen for RetentionHoldHold-innstillingen på den bestemte postboksen i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
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

 **Merk:** Hvis en postboks er mindre enn 10 MB, behandler ikke assistenten for administrerte mapper automatisk postboksen.
 
Hvis du vil ha mer informasjon om oppbevaringspolicyer i administrasjonssenteret for Exchange, kan du se:
- [Oppbevaringskoder og oppbevaringspolicyer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Bruke en oppbevaringspolicy for postbokser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Legge til eller fjerne oppbevaringskoder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Slik identifiserer du typen hold som er plassert på en postboks](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
