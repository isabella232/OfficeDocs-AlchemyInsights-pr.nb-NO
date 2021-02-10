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
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="0ccb3-102">Synkronisering av hash for passord for domenetjeneste</span><span class="sxs-lookup"><span data-stu-id="0ccb3-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="0ccb3-103">**Hvis Azure AD DS-forekomsten ber deg om å aktivere synkronisering av hash for passord**</span><span class="sxs-lookup"><span data-stu-id="0ccb3-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="0ccb3-104">Du kan støte på et scenario der du kjører et hybridmiljø med brukere som synkroniserer fra et lokalt Azure Active Directory Domain Services (AD DS)-miljø.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="0ccb3-105">Dette scenariet oppstår til tross for at du har synkronisering av hash for passord fra den lokale AD DS til Azure AD-leieren.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="0ccb3-106">**Årsak**</span><span class="sxs-lookup"><span data-stu-id="0ccb3-106">**Cause**</span></span>

<span data-ttu-id="0ccb3-107">Dette skjer fordi Azure AD Connect som standard ikke synkroniserer hash-kode for eldre LAN Manager (New Technology LAN Manager) og Kerberos som er nødvendige for Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="0ccb3-108">**Løsning**</span><span class="sxs-lookup"><span data-stu-id="0ccb3-108">**Workaround**</span></span> 

<span data-ttu-id="0ccb3-109">Du må konfigurere Azure AD Connect for å synkronisere hash-hash for passord som kreves for NTLM- og Kerberos-godkjenning.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="0ccb3-110">Når Azure AD Connect er konfigurert, synkroniserer også en lokal kontooppretting eller endring av passord det eldre passordet til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="0ccb3-111">Se her [for](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) mer informasjon om dette og for veiledning om hvordan du aktiverer passordsynkronisering i Azure AD DS-hybridmiljøer.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>