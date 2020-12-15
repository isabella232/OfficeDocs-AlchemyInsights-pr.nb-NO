---
title: Logge på Microsoft Edge automatisk
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677769"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="cf5d3-102">Logge på Microsoft Edge automatisk</span><span class="sxs-lookup"><span data-stu-id="cf5d3-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="cf5d3-103">Microsoft Edge bruker operativ systemets standard konto til automatisk å logge seg på en bruker i henhold til hvordan brukerens enhet er konfigurert.</span><span class="sxs-lookup"><span data-stu-id="cf5d3-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="cf5d3-104">Scenariene for hver type enhets konfigurasjon og den avhengige bruker påloggings prosessen beskrives nedenfor:</span><span class="sxs-lookup"><span data-stu-id="cf5d3-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="cf5d3-105">**Enheten er hybrid/AAD-J**: dette alternativet er tilgjengelig i Windows 10, Windows på lavere nivå og tilsvarende serverversjoner.</span><span class="sxs-lookup"><span data-stu-id="cf5d3-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="cf5d3-106">Brukere logges automatisk på med Azure Active Directory-kontoer (AD).</span><span class="sxs-lookup"><span data-stu-id="cf5d3-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="cf5d3-107">**Enheten er domene tilknyttet**: dette alternativet er tilgjengelig i Windows 10, Windows på lavere nivå og tilsvarende serverversjoner.</span><span class="sxs-lookup"><span data-stu-id="cf5d3-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="cf5d3-108">Som standard logges ikke brukere med domene kontoer automatisk. Hvis du vil aktivere automatisk pålogging for dem, bruker du **ConfigureOnPremisesAccountAutoSignIn** -policyen.</span><span class="sxs-lookup"><span data-stu-id="cf5d3-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="cf5d3-109">Hvis du vil aktivere automatisk pålogging for brukere med Azure AD-kontoer, bør du vurdere å bli med i hybrid tilkobling til enhetene sine.</span><span class="sxs-lookup"><span data-stu-id="cf5d3-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="cf5d3-110">**Standard kontoen for operativ systemet er en Microsoft-konto**: dette alternativet er tilgjengelig på Windows 10 RS3 (versjon 1709, bygg 10.0.16299) og nyere versjoner.</span><span class="sxs-lookup"><span data-stu-id="cf5d3-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="cf5d3-111">Det er lite sannsynlig at scenarioet oppstår på bedrifts enheter.</span><span class="sxs-lookup"><span data-stu-id="cf5d3-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="cf5d3-112">Hvis for eksempel operativ systemets standard konto er en Microsoft-konto, logger Microsoft Edge automatisk på brukeren med Microsoft-kontoen.</span><span class="sxs-lookup"><span data-stu-id="cf5d3-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
