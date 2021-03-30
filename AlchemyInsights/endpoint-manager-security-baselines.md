---
title: EndPoint Manager – sikkerhetsgrunnlinjer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421085"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="03bdc-102">EndPoint Manager – sikkerhetsgrunnlinjer</span><span class="sxs-lookup"><span data-stu-id="03bdc-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="03bdc-103">Sikkerhetsgrunnlinjer er forhåndskonfigurerte grupper med Windows-innstillinger som hjelper deg med å bruke sikkerhetsinnstillingene som anbefales av de relevante sikkerhetsteamene.</span><span class="sxs-lookup"><span data-stu-id="03bdc-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="03bdc-104">Disse grunnlinjene kan tilpasses slik at de bare leverer de ønskede innstillingene og verdiene.</span><span class="sxs-lookup"><span data-stu-id="03bdc-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="03bdc-105">Hvis du vil ha mer informasjon om sikkerhetsgrunnlinjer, kan du se Bruke [sikkerhetsgrunnlinjer til å konfigurere Windows 10-enheter i Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="03bdc-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="03bdc-106">Det finnes for øyeblikket opprinnelige planer for disse produktene:</span><span class="sxs-lookup"><span data-stu-id="03bdc-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="03bdc-107">Sikkerhetsinnstillinger for Windows MDM</span><span class="sxs-lookup"><span data-stu-id="03bdc-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="03bdc-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="03bdc-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="03bdc-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="03bdc-109">Microsoft Edge</span></span>

<span data-ttu-id="03bdc-110">Hver av grunnlinjene oppdateres med jevne mellomrom og utgis i trinnvise versjoner.</span><span class="sxs-lookup"><span data-stu-id="03bdc-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="03bdc-111">Hver versjon legger til og eller fjerner innstillinger fra den forrige versjonen for å sikre at grunnlinjen oppfyller gjeldende veiledning.</span><span class="sxs-lookup"><span data-stu-id="03bdc-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="03bdc-112">Konsollen For sikkerhetsgrunnlinjer i Endepunktsikkerhet kan ulike versjoner sammenlignes ved å gjøre endringene fra versjon til versjon synlige.</span><span class="sxs-lookup"><span data-stu-id="03bdc-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="03bdc-113">Hvis du vil ha veiledning om hvordan du mest effektivt endrer hvilken versjon av opprinnelig plan som distribueres, kan du se [Behandle sikkerhetsprofiler for grunnlinje i Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="03bdc-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="03bdc-114">Når du har distribuert en sikkerhetsgrunnlinje, kan du overvåke tilstanden til distribusjon og se gjennom innstillingene på enhet-for-enhet-basis.</span><span class="sxs-lookup"><span data-stu-id="03bdc-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="03bdc-115">**Obs!** Rapporteringsdataene for opprinnelige planer kan ta opptil 24 timer fra den første distribusjonen til en enhet og opptil seks timer for ytterligere oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="03bdc-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="03bdc-116">Den vanligste årsaken til at en innstilling for grunnlinje ikke brukes, er at den samme innstillingen brukes i en annen profil.</span><span class="sxs-lookup"><span data-stu-id="03bdc-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="03bdc-117">Dette scenarioet kan undersøkes for en bestemt enhet ved å velge denne enheten fra noden Enhetsstatus for sikkerhetsgrunnlinjeprofilen.</span><span class="sxs-lookup"><span data-stu-id="03bdc-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="03bdc-118">Hvis du vil ha mer informasjon, kan du se Løse [konflikter for sikkerhetsgrunnlinjer](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="03bdc-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>