---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685607"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="e4b4b-102">Blokkere eldre godkjenning</span><span class="sxs-lookup"><span data-stu-id="e4b4b-102">Blocking legacy authentication</span></span>

<span data-ttu-id="e4b4b-103">Eldre godkjenning er en term som refererer til en godkjennings forespørsel gjort av:</span><span class="sxs-lookup"><span data-stu-id="e4b4b-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="e4b4b-104">Eldre Office-klienter som ikke bruker moderne godkjenning (for eksempel Office 2010-klient).</span><span class="sxs-lookup"><span data-stu-id="e4b4b-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="e4b4b-105">Alle klienter som bruker eldre e-postprotokoller som IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="e4b4b-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="e4b4b-106">Hvis du vil ha mer informasjon om blokkering av eldre godkjenning og aktivering av moderne godkjenning, kan du se [blokkere eldre godkjenning](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="e4b4b-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="e4b4b-107">Sikkerhets standarder i Azure Active Directory (Azure AD) gjør det enklere å være sikre og beskytte organisasjonen din.</span><span class="sxs-lookup"><span data-stu-id="e4b4b-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="e4b4b-108">Sikkerhets standarder inneholder forhånds kon figurerte sikkerhets innstillinger for vanlige angrep.</span><span class="sxs-lookup"><span data-stu-id="e4b4b-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="e4b4b-109">Hvis du vil ha mer informasjon om sikkerhets standarder, kan du se [Hva er sikkerhets standarder?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="e4b4b-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="e4b4b-110">**Obs!** hvis leieren din ble opprettet på eller etter oktober 22nd, 2019, er det mulig at du opplever den nye, sikreste standard virke måten og allerede har sikkerhets standarder aktivert i leieren din.</span><span class="sxs-lookup"><span data-stu-id="e4b4b-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="e4b4b-111">I et tiltak for å beskytte alle brukerne, blir sikkerhets standarder rullet ut til alle nye tenanter som opprettes.</span><span class="sxs-lookup"><span data-stu-id="e4b4b-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
