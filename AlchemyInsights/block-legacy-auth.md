---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820187"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="3b314-102">Blokkere eldre godkjenning</span><span class="sxs-lookup"><span data-stu-id="3b314-102">Blocking legacy authentication</span></span>

<span data-ttu-id="3b314-103">Eldre godkjenning er en term som refererer til en godkjenningsforespørsel fra:</span><span class="sxs-lookup"><span data-stu-id="3b314-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="3b314-104">Eldre Office-klienter som ikke bruker moderne godkjenning (for eksempel Office 2010-klient).</span><span class="sxs-lookup"><span data-stu-id="3b314-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="3b314-105">Alle klienter som bruker eldre e-postprotokoller, for eksempel IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="3b314-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="3b314-106">Hvis du vil ha mer informasjon om hvordan du blokkerer eldre godkjenning og aktiverer moderne godkjenning, kan du se [Blokkere eldre godkjenning](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="3b314-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="3b314-107">Sikkerhetsstandarder i Azure Active Directory (Azure AD) gjør det enklere å være sikker og beskytte organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="3b314-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="3b314-108">Sikkerhetsstandarder inneholder forhåndskonfigurerte sikkerhetsinnstillinger for vanlige angrep.</span><span class="sxs-lookup"><span data-stu-id="3b314-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="3b314-109">Hvis du vil ha mer informasjon om sikkerhetsstandarder, kan du [se Hva er sikkerhetsstandarder?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="3b314-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="3b314-110">**Obs!** Hvis leieren ble opprettet den 22. oktober 2019, er det mulig at du opplever den nye virkemåten for sikker som standard og allerede har sikkerhetsstandarder aktivert i leieren.</span><span class="sxs-lookup"><span data-stu-id="3b314-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="3b314-111">I et forsøk på å beskytte alle våre brukere rulles sikkerhetsstandarder ut til alle nye tenanter opprettet.</span><span class="sxs-lookup"><span data-stu-id="3b314-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
