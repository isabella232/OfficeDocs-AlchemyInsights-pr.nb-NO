---
title: Bruke e-postprofiler med Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555250"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="bb0dd-102">Bruke e-postprofiler med Intune</span><span class="sxs-lookup"><span data-stu-id="bb0dd-102">Using email profiles with Intune</span></span>

<span data-ttu-id="bb0dd-103">Intune kan brukes til å opprette og distribuere e-postprofiler for den opprinnelige (innebygde) e-postklienten på flere enhetsplattformer.</span><span class="sxs-lookup"><span data-stu-id="bb0dd-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="bb0dd-104">Hvis du vil ha informasjon om noen av begrensningene som er knyttet til e-postprofiler, inkludert hvordan tilstedeværelsen av eksisterende profiler håndteres og hvordan du fjerner e-postprofiler, kan du se Legge til [e-postinnstillinger på enheter ved hjelp av Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="bb0dd-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="bb0dd-105">Hvis du vil ha mer informasjon om hvordan du oppretter e-postprofiler for hver enhetsplattform, kan du se:</span><span class="sxs-lookup"><span data-stu-id="bb0dd-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="bb0dd-106">Innstillinger for Android-enheter for å konfigurere e-post, godkjenning og synkronisering i Intune</span><span class="sxs-lookup"><span data-stu-id="bb0dd-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="bb0dd-107">Legge til e-postinnstillinger for iOS- og iPadOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bb0dd-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="bb0dd-108">Innstillinger for e-postprofil i Microsoft Intune for enheter som kjører Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="bb0dd-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="bb0dd-109">Innstillinger for e-postprofil for enheter som kjører Windows 10 i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bb0dd-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="bb0dd-110">**Vanlige synkroniseringsproblem**</span><span class="sxs-lookup"><span data-stu-id="bb0dd-110">**Common syncing issue**</span></span>

<span data-ttu-id="bb0dd-111">**En KNOX på Android-e-postprofil hindrer at brukerkontakter, kalender og oppgaver synkroniseres til brukerenheter.**</span><span class="sxs-lookup"><span data-stu-id="bb0dd-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="bb0dd-112">KNOX på Android KNOX-e-postprofilen gir administratoren muligheten til å bestemme hvilke innholdstyper som synkroniseres med enheten ved å angi at hver av dem er aktivert.</span><span class="sxs-lookup"><span data-stu-id="bb0dd-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="bb0dd-113">Hvis innstillingen for noen av innholdstypene er satt til **Ikke konfigurert** (standard), synkroniseres ikke denne innholdstypen automatisk.</span><span class="sxs-lookup"><span data-stu-id="bb0dd-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="bb0dd-114">En bruker kan aktivere innholdstypen de vil ha direkte på enheten manuelt, men denne konfigurasjonen overskrives av policyinnstillingen Intune, og synkroniseringen stopper for denne innholdstypen.</span><span class="sxs-lookup"><span data-stu-id="bb0dd-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

