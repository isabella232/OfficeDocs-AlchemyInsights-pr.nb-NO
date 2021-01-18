---
title: Problem med å bli med i VM-er
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885667"
---
# <a name="issue-joining-vms"></a>Problem med å bli med i VM-er

Hvis du vil løse problemer som oppstår mens du prøver å koble til VM-er, utfører du følgende trinn:

1. Prøv å logge på med **UPN** -formatet (for eksempel «joeuser@contoso.com») i stedet for **sAMAccountName** -formatet (CONTOSO\joeuser).
2. Kontroller at du har aktivert passord synkronisering i henhold til trinnene som er beskrevet i *komme i gang* -veiledningen.
3. Kontroller at den berørte bruker kontoen ikke er en ekstern konto i Azure AD-leieren. Eksterne brukere kan ikke logge seg på det forvaltede domenet fordi Azure AD Domain Services ikke har legitimasjon for slike bruker kontoer.
4. Hvis den berørte bruker kontoen er en bruker konto som bare er en sky, må du sørge for at brukere har endret passordet sitt etter at du aktiverte Azure AD Domain Services. Dette trinnet fører til at legitimasjons nummer som kreves for Azure AD Domain Services, genereres.
5. Hvis de berørte bruker kontoene synkroniseres fra en lokal katalog, må du kontrollere at den anbefalte utgivelsen av Azure AD Connect er konfigurert til å utføre en fullstendig synkronisering.
6. Hvis problemet vedvarer etter at du har bekreftet trinn 4, utfører du følgende kommandoer fra synkroniserings maskinen:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.