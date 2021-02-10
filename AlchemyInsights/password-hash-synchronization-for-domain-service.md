---
title: Synkronisering av hash for passord for domenetjeneste
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177485"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Synkronisering av hash for passord for domenetjeneste

**Hvis Azure AD DS-forekomsten ber deg om å aktivere synkronisering av hash for passord**

Du kan støte på et scenario der du kjører et hybridmiljø med brukere som synkroniserer fra et lokalt Azure Active Directory Domain Services (AD DS)-miljø. Dette scenariet oppstår til tross for at du har synkronisering av hash for passord fra den lokale AD DS til Azure AD-leieren.

**Årsak**

Dette skjer fordi Azure AD Connect som standard ikke synkroniserer hash-kode for eldre LAN Manager (New Technology LAN Manager) og Kerberos som er nødvendige for Azure AD DS.

**Løsning** 

Du må konfigurere Azure AD Connect for å synkronisere hash-hash for passord som kreves for NTLM- og Kerberos-godkjenning.

Når Azure AD Connect er konfigurert, synkroniserer også en lokal kontooppretting eller endring av passord det eldre passordet til Azure AD. Se her [for](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) mer informasjon om dette og for veiledning om hvordan du aktiverer passordsynkronisering i Azure AD DS-hybridmiljøer.