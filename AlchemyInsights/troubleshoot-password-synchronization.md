---
title: Feilsøking i forbindelse med synkronisering av passord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303329"
---
# <a name="troubleshoot-password-synchronization"></a>Feilsøking i forbindelse med synkronisering av passord

Slik feilsøker du problemer der ingen passord er synkronisert med Azure AD koble versjon 1.1.614.0 eller senere:
  
1. Åpne en ny Windows PowerShell-økt på koble til Azure AD-server med alternativet **Kjør som Administrator** . 
    
2. Kjøre **Set-ExecutionPolicy RemoteSigned** eller **Set-ExecutionPolicy ubegrenset**. 
    
3. Start veiviseren Koble til Azure AD.
    
4. Naviger til den ** tilleggsoppgaver ** velger ** feilsøke **, og klikk **Neste**. 
    
5. Klikk **Start for å starte feilsøking** -menyen i PowerShell på siden feilsøking. 
    
6. Velg **Feilsøking i forbindelse med synkronisering av passord**på hovedmenyen. 
    
7. I sub-menyen velger du **synkronisering av passord fungerer ikke i det hele tatt**. 
    
 **Forstå resultatet av feilsøkingen oppgaven**
  
Feilsøking oppgaven utfører følgende kontroller:
  
- Validerer at funksjonen for synkronisering av passord er aktivert for Azure AD-leier.
    
- Validerer at Azure AD koble til serveren ikke er i modus for oppsamling.
    
- For hvert eksisterende lokale Active Directory connector (som tilsvarer en eksisterende Active Directory-skog):
    
- 
  - Validerer at funksjonen for synkronisering av passord er aktivert.
    
  - Søker etter passord synkroniseringshendelser livstegn i hendelsesloggene for Windows-program.
    
  - For hver Active Directory-domene under lokale Active Directory connector:
    
  - Validerer at domenet kan nås fra Azure AD koble til serveren.
    
  - Validerer at Active Directory Domain Services (AD DS)-kontoer som brukes av den lokale Active Directory connector har riktig brukernavn, passord og tillatelser som kreves for synkronisering av passord.
    
Hvis du vil ha mer hjelp, feilsøking i forbindelse med synkronisering av passord, kan du se [Feilsøking i forbindelse med synkronisering av passord med koble til Azure AD-synkronisering](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

