---
title: Slette foreldreløse brukere fra lokal server
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198581"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Slette foreldreløse brukere fra lokal server

Hvis du vil fjerne en foreldreløs bruker, gjør du følgende:

1. Tvinge katalogsynkronisering ved å følge instruksjonene i [Hva er hybrid identitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Hvis du vil kontrollere katalogsynkronisering, kan du se [Hva er hybrid identitet med Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Hvis synkronisering fungerer på riktig måte, men slettingen av Active Directory-objekt ikke overføres til Azure AD, fjerner du det foreldreløse objektet manuelt ved hjelp av en av følgende Azure Active Directory-modul for Windows PowerShell-cmdleter:

    Fjern MsolContact  
    Fjern MsolGroup  
    Fjern MsolUser

    Hvis du for eksempel vil fjerne foreldreløse bruker-ID-john.smith@contoso.com, som opprinnelig ble opprettet ved hjelp av katalogsynkronisering, kjører du cmdleten:

    Fjern MsolUser – UserPrincipalName John.Smith@Contoso.com