---
title: Oppbevarings policyer i Exchange admin Center fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740519"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Oppbevarings policyer i administrasjons senteret for Exchange

Hvis du vil at vi skal kjøre automatiske kontroller for innstillingene som nevnes nedenfor, velger du tilbake-knappen < øverst på siden, og deretter skriver du inn e-postadressen til brukeren som har problemer med oppbevarings policyer.

 **Problem:** Nylig opprettede eller oppdaterte oppbevarings policyer i administrasjons senteret for Exchange gjelder ikke for post bokser eller elementer flyttes ikke til arkiv post boksen eller slettes. 
  
 **Hoved årsaker:**
  
- Dette kan være fordi **assistenten for forvaltede mapper** ikke har behandlet brukerens post boks. Den forvaltede mappe assistenten prøver å behandle alle post bokser i en sky BAS ert organisasjon én gang i løpet av sju dager. Hvis du endrer en oppbevarings kode eller bruker en annen oppbevarings policy i en post boks, kan du vente til den administrerte mappe assistenten behandler post boksen, eller du kan kjøre Start-ManagedFolderAssistant-cmdleten for å starte en bestemt post boks i den forvaltede mappe. Hvis du kjører denne cmdleten, er det nyttig å teste eller feilsøke en oppbevarings kode-innstilling. Hvis du vil ha mer informasjon, kan du se [kjøre assistenten for forvaltede mapper](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Løsning:** Kjør følgende kommando for å starte den forvaltede mappe assistenten for en bestemt post boks:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Dette kan også skje hvis **RetentionHold** er **aktivert** på post boksen. Hvis post boksen er plassert på en RetentionHold, blir ikke oppbevarings policyen i post boksen behandlet i den perioden. Hvis du vil ha mer informasjon på RetentionHold-innstillingen, kan du se: [Oppbevarings plass for post boks](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Løsning**
    
  - Kontroller statusen for RetentionHold-innstillingen for den bestemte post boksen i [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kjør følgende kommando for å **deaktivere** RetentionHold for en bestemt post boks:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Kjør deretter den administrerte mappe assistenten på nytt:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Obs!** Hvis en post boks er mindre enn 10 MB, vil ikke assistenten for forvaltet mappe automatisk behandle post boksen.
 
Hvis du vil ha mer informasjon om oppbevarings policyer i administrasjons senteret for Exchange, kan du se:
- [Oppbevarings koder og oppbevarings policyer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Bruke en oppbevarings policy på post bokser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Legge til eller fjerne oppbevarings koder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Identifisere hvilken type sperring som skal plasseres i en post boks](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
