---
title: Opprette Intune-policyer og -profiler
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: af8f1a3dfaccaca52f187f387274d63b22631b2d
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704651"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="ef8c9-102">Opprette Intune-policy og -profiler</span><span class="sxs-lookup"><span data-stu-id="ef8c9-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="ef8c9-103">I Intune kan du opprette policyer og profiler som gjør forskjellige ting.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="ef8c9-104">**Registreringsprofiler:** Forhåndskonfigurer enhetene dine etter plattform, aktiver bruker affinitet, bruk godkjenning med flere faktorer og mer.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="ef8c9-105">[Hva er enhetsregistrering](https://docs.microsoft.com/intune/device-enrollment)og opprettingsprofiler for [Android,](https://docs.microsoft.com/intune/android-enroll) [iOS,](https://docs.microsoft.com/intune/ios-enroll) [macOS](https://docs.microsoft.com/intune/macos-enroll)og [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) er gode ressurser.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="ef8c9-106">**Samsvarspolicyer:** Definer reglene og innstillingene som enheter må følge for å overholde samsvarsvilkårene.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="ef8c9-107">Du kan også bruke samsvarspolicyer til å overvåke enheter og varsle brukerne om manglende overholdelse.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="ef8c9-108">Kom i gang med [policyer for enhetssamsvar.](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="ef8c9-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="ef8c9-109">**Policyer for betinget** tilgang: Bidra til å sikre organisasjonsressurser, avhengig av betingelsene du angir.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="ef8c9-110">For enheter som ikke overholder samsvar, kan du for eksempel bruke betinget tilgang til å begrense tilgangen til e-post og SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="ef8c9-111">[Det som er betinget tilgang](https://docs.microsoft.com/intune/conditional-access) [og vanlige måter å bruke betinget tilgang](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) på, er gode ressurser for å komme i gang.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="ef8c9-112">**Konfigurasjonsprofiler:** Administrer funksjoner og innstillinger på enheter, inkludert e-postinnstillinger, legg til et WiFi-nettverk, bruk innebygde maler, kontroller iOS- og macOS-enhetsfunksjoner og mer.</span><span class="sxs-lookup"><span data-stu-id="ef8c9-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="ef8c9-113">Komme i gang [på enhetskonfigurasjonsprofiler.](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="ef8c9-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="ef8c9-114">Nyttige koblinger:</span><span class="sxs-lookup"><span data-stu-id="ef8c9-114">Helpful links:</span></span>

- [<span data-ttu-id="ef8c9-115">Vanlige spørsmål, problemer og løsninger med enhetspolicyer og profiler i Intune</span><span class="sxs-lookup"><span data-stu-id="ef8c9-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="ef8c9-116">Feilsøke policyer og profiler i Intune</span><span class="sxs-lookup"><span data-stu-id="ef8c9-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)
