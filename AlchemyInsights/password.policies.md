---
title: Passordpolicyer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747047"
---
# <a name="password-policies"></a><span data-ttu-id="d6155-102">Passordpolicyer</span><span class="sxs-lookup"><span data-stu-id="d6155-102">Password policies</span></span>

<span data-ttu-id="d6155-103">**Jeg har problemer med passordpolicyen for en bruker**</span><span class="sxs-lookup"><span data-stu-id="d6155-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="d6155-104">Passordpolicyen for en bruker avhenger av om brukeren bare er skybasert eller lokalt.</span><span class="sxs-lookup"><span data-stu-id="d6155-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="d6155-105">Bare skybrukere må velge et passord som oppfyller kravene i denne artikkelen: Passordpolicyer som [bare gjelder for brukerkontoer i skyen](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="d6155-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="d6155-106">Lokale brukere må velge et passord som oppfyller de lokale kravene.</span><span class="sxs-lookup"><span data-stu-id="d6155-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="d6155-107">Hvis en lokal bruker ikke kan angi passordet sitt, må du kontrollere lokale krav.</span><span class="sxs-lookup"><span data-stu-id="d6155-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="d6155-108">**Jeg vet ikke hvordan jeg angir eller kontrollerer utløpspolicyer for passord**</span><span class="sxs-lookup"><span data-stu-id="d6155-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="d6155-109">Du kan angi og kontrollere utløpspolicyen for skybrukere i leieren ved hjelp av PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d6155-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="d6155-110">Følg instruksjonene i denne artikkelen: [Angi eller kontrollere passordpolicyene ved hjelp av PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="d6155-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="d6155-111">Policyen for passordutløp for lokale brukere er angitt i den lokale AD-en.</span><span class="sxs-lookup"><span data-stu-id="d6155-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="d6155-112">**Andre nyttige koblinger:**</span><span class="sxs-lookup"><span data-stu-id="d6155-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="d6155-113">Komme i gang med tilbakestilling av passord</span><span class="sxs-lookup"><span data-stu-id="d6155-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="d6155-114">Feilsøke administratorstartet tilbakestilling av passord</span><span class="sxs-lookup"><span data-stu-id="d6155-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
