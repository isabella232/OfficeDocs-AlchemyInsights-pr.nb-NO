---
title: Logg på Microsoft Edge automatisk
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398738"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="ddbc6-102">Logg på Microsoft Edge automatisk</span><span class="sxs-lookup"><span data-stu-id="ddbc6-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="ddbc6-103">Microsoft Edge bruker standardkontoen for operativsystemet til å logge på en bruker automatisk i henhold til hvordan brukerens enhet er konfigurert.</span><span class="sxs-lookup"><span data-stu-id="ddbc6-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="ddbc6-104">Scenariene for hver type enhetskonfigurasjon og den avhengige bruker påloggingsprosessen er beskrevet nedenfor:</span><span class="sxs-lookup"><span data-stu-id="ddbc6-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="ddbc6-105">**Enheten er hybrid/AAD-J**: Dette alternativet er tilgjengelig på Windows 10, windows på lavere nivå og tilsvarende serverversjoner.</span><span class="sxs-lookup"><span data-stu-id="ddbc6-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="ddbc6-106">Brukere blir automatisk logget på med Azure Active Directory-kontoene (AD)..</span><span class="sxs-lookup"><span data-stu-id="ddbc6-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="ddbc6-107">**Enheten er domeneføyd:** Dette alternativet er tilgjengelig i Windows 10, windows på lavere nivå og tilsvarende serverversjoner.</span><span class="sxs-lookup"><span data-stu-id="ddbc6-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="ddbc6-108">Brukere med domenekontoer er som standard ikke logget på automatisk. Hvis du vil aktivere automatisk pålogging for dem, bruker du **policyen ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="ddbc6-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="ddbc6-109">Hvis du vil aktivere automatisk pålogging for brukere med Azure AD-kontoer, kan du vurdere hybridkobling av enhetene sine.</span><span class="sxs-lookup"><span data-stu-id="ddbc6-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="ddbc6-110">**Operativsystemets standardkonto** er en Microsoft-konto: Dette alternativet er tilgjengelig på Windows 10 RS3 (versjon 1709, bygg 10.0.16299) og nyere versjoner.</span><span class="sxs-lookup"><span data-stu-id="ddbc6-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="ddbc6-111">Det er usannsynlig at dette skjer på bedriftsenheter.</span><span class="sxs-lookup"><span data-stu-id="ddbc6-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="ddbc6-112">Hvis standardkontoen for operativsystemet er en Microsoft-konto, logger Microsoft Edge imidlertid automatisk på brukeren med Microsoft-kontoen.</span><span class="sxs-lookup"><span data-stu-id="ddbc6-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
