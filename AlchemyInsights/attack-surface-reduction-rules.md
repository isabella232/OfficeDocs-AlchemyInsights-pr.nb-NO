---
title: Regler for reduksjon av angrepsoverflater
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676437"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="26757-102">Regler for reduksjon av angrepsoverflater</span><span class="sxs-lookup"><span data-stu-id="26757-102">Attack surface reduction rules</span></span>

<span data-ttu-id="26757-103">Hvis du utelater filer eller mapper, kan beskyttelsen som leveres av regler for reduksjon av angrepsoverflater, reduseres kraftig.</span><span class="sxs-lookup"><span data-stu-id="26757-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="26757-104">Filer som ville ha blitt blokkert av en regel, kan kjøres, og ingen rapport eller hendelse registreres.</span><span class="sxs-lookup"><span data-stu-id="26757-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="26757-105">En utelatelse gjelder for alle regler som tillater utelatelser.</span><span class="sxs-lookup"><span data-stu-id="26757-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="26757-106">ASR-utelatelser bruker samme syntaks som Microsoft Defender Antivirus utelatelser.</span><span class="sxs-lookup"><span data-stu-id="26757-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="26757-107">Hvis du vil ha mer informasjon, kan du se Konfigurere og validere [utelatelser for Microsoft Defender Antivirus skanninger](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="26757-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="26757-108">Hvis du vil unngå problemer, kan du se gjennom Vanlige feil du [bør unngå når du definerer utelatelser.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="26757-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="26757-109">Ikke alle ASR-regler støtter utelatelser.</span><span class="sxs-lookup"><span data-stu-id="26757-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="26757-110">Hvis du vil validere om regelen støtter utelatelser, kan du se tabellen [Angrepsoverflatereduksjonsregler](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="26757-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="26757-111">Regler for reduksjon av angrepsoverflater</span><span class="sxs-lookup"><span data-stu-id="26757-111">Attack surface reduction rules</span></span>

<span data-ttu-id="26757-112">Organisasjonens angrepsoverflate omfatter alle stedene der en angriper kan kompromittere organisasjonsenheter eller -nettverk.</span><span class="sxs-lookup"><span data-stu-id="26757-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="26757-113">Reduksjon av angrepsoverflaten betyr å beskytte organisasjonsenhetene og nettverket, noe som gjør at angripere med færre måter å utføre angrep på.</span><span class="sxs-lookup"><span data-stu-id="26757-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="26757-114">Det kan hjelpe å konfigurere regler for reduksjon av angrepsoverflater i Microsoft Defender for endepunkt.</span><span class="sxs-lookup"><span data-stu-id="26757-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="26757-115">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="26757-115">For more information, see:</span></span>

- [<span data-ttu-id="26757-116">Tilordne GUID for ASR-regel til navn</span><span class="sxs-lookup"><span data-stu-id="26757-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="26757-117">ASR-regler:</span><span class="sxs-lookup"><span data-stu-id="26757-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="26757-118">Windows 10 Pro, versjon 1709 eller nyere</span><span class="sxs-lookup"><span data-stu-id="26757-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="26757-119">Windows 10 Enterprise, versjon 1709 eller nyere</span><span class="sxs-lookup"><span data-stu-id="26757-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="26757-120">Windows Server, versjon 1803 (halvårskanal) eller nyere</span><span class="sxs-lookup"><span data-stu-id="26757-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="26757-121">Identifiser riktig utelatelse som skal brukes</span><span class="sxs-lookup"><span data-stu-id="26757-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="26757-122">Se etter hendelses-ID 1121 eller 1122 i Microsoft-Windows-Windows Defender/Operativ logg.</span><span class="sxs-lookup"><span data-stu-id="26757-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="26757-123">Evaluer blokkscenarioet og konteksten, og bekreft at dette scenarioet må oppheves.</span><span class="sxs-lookup"><span data-stu-id="26757-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="26757-124">Les Bane-verdien i hendelsesdetaljene, som er verdien som definerer utelatelsen.</span><span class="sxs-lookup"><span data-stu-id="26757-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="26757-125">Gjør utelukkelsen så streng som mulig.</span><span class="sxs-lookup"><span data-stu-id="26757-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="26757-126">Bruk et jokertegn der det er nødvendig (for eksempel erstatt brukervariabel).</span><span class="sxs-lookup"><span data-stu-id="26757-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="26757-127">Bruk utelukkelsen i henhold til distribusjonsbehovene dine.</span><span class="sxs-lookup"><span data-stu-id="26757-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="26757-128">Hvis du vil ha mer informasjon, kan du [se Tilpasse regler for reduksjon av angrepsoverflater](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="26757-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="26757-129">Utelukkelse er ikke innfridd</span><span class="sxs-lookup"><span data-stu-id="26757-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="26757-130">Bestem om regelen støtter utelatelser.</span><span class="sxs-lookup"><span data-stu-id="26757-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="26757-131">Hvis du vil ha mer informasjon, [kan du se Regler for reduksjon av angrepsoverflater](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="26757-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="26757-132">Se gjennom utelatelsene som er brukt, og bekreft med hendelsesdataene for skrivefeil eller feiltoolerte jokertegn.</span><span class="sxs-lookup"><span data-stu-id="26757-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="26757-133">Hvis du vil ha mer informasjon, kan du [se Utelukkelsestyper som støttes](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="26757-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="26757-134">Hvis regelen påvirkes for høyt, bør du vurdere å flytte regelen (tilbake) til overvåkingsmodus for å utføre ytterligere validering.</span><span class="sxs-lookup"><span data-stu-id="26757-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="26757-135">Hvis du vil ha mer informasjon, kan du se [Teste hvordan Microsoft Defender for endepunktfunksjoner fungerer i overvåkingsmodus](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="26757-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="26757-136">Samle inn støttedata for å åpne en støttesak ved hjelp av denne kommandoen:</span><span class="sxs-lookup"><span data-stu-id="26757-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="26757-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="26757-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="26757-138">Hvis du vil ha mer informasjon, kan du se [Problemer med introduksjonsmaskiner til Microsoft Defender for endepunkter](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="26757-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
