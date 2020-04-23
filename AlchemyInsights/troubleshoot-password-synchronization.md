---
title: Feilsøke synkronisering av passord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732519"
---
# <a name="troubleshoot-password-synchronization"></a>Feilsøke synkronisering av passord

Slik feilsøker du problemer der ingen passord synkroniseres med Azure AD Connect versjon 1.1.614.0 eller senere:
  
1. Åpne en ny Windows PowerShell-økt på Azure AD Connect-serveren med alternativet **Kjør som administrator.**

2. Kjør **Set-ExecutionPolicy RemoteSigned** eller **Set-ExecutionPolicy ubegrenset**.

3. Start veiviseren for AD-tilkobling for Azure.

4. Gå til **Flere oppgaver-siden,** velg **Feilsøking**, og klikk **Neste**.

5. Klikk Start på feilsøking-siden **for å starte feilsøkingsmenyen** i PowerShell.

6. Velg **Feilsøk synkronisering av passord i**hovedmenyen.

7. Velg Synkronisering av **passord fungerer ikke i**det hele tatt .

**Forstå resultatene av feilsøkingsoppgaven**
  
Feilsøkingsoppgaven utfører følgende kontroller:
  
- Validerer at funksjonen for synkronisering av passord er aktivert for Azure AD-leieren.

- Validerer at Azure AD Connect-serveren ikke er i oppsamlingsmodus.

- For hver eksisterende lokale Active Directory-kobling (som tilsvarer en eksisterende Active Directory-skog):

- 
  - Validerer at funksjonen for synkronisering av passord er aktivert.

  - Søker etter hjerterytmehendelser for synkronisering av passord i hendelsesloggene for Windows-programmet.

  - For hvert Active Directory-domene under den lokale Active Directory-koblingen:

  - Validerer at domenet kan nås fra Azure AD Connect-serveren.

  - Validerer at Active Directory Domain Services (AD DS)-kontoer som brukes av den lokale Active Directory-koblingen, har riktig brukernavn, passord og tillatelser som kreves for synkronisering av passord.

Hvis du vil ha mer hjelp til å feilsøke passordsynkronisering, kan du se [Feilsøke synkronisering av passord med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  