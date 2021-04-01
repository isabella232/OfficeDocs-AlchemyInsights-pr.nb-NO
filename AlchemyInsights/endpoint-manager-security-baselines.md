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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440893"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="3842e-102">EndPoint Manager – sikkerhetsgrunnlinjer</span><span class="sxs-lookup"><span data-stu-id="3842e-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="3842e-103">Sikkerhetsgrunnlinjer er forhåndskonfigurerte grupper med Windows-innstillinger som hjelper deg med å bruke sikkerhetsinnstillingene som anbefales av de relevante sikkerhetsteamene.</span><span class="sxs-lookup"><span data-stu-id="3842e-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="3842e-104">Disse referanseverdiene kan tilpasses for bare å levere de innstillingene og verdiene du ønsker.</span><span class="sxs-lookup"><span data-stu-id="3842e-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="3842e-105">Hvis du vil ha mer informasjon om sikkerhetsmessige grunnlinjer, kan du se [Bruk sikkerhetsmessige grunnlinjer til å konfigurere Windows 10-enheter i Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="3842e-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="3842e-106">Det finnes for øyeblikket grunnlinjer for disse produktene:</span><span class="sxs-lookup"><span data-stu-id="3842e-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="3842e-107">Windows MDM-sikkerhetsinnstillinger</span><span class="sxs-lookup"><span data-stu-id="3842e-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="3842e-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="3842e-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="3842e-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3842e-109">Microsoft Edge</span></span>

<span data-ttu-id="3842e-110">Hver av grunnlinjene oppdateres med jevne mellomrom og lanseres i trinnvise versjoner.</span><span class="sxs-lookup"><span data-stu-id="3842e-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="3842e-111">Hver versjon legger til og fjerner innstillinger fra den forrige versjonen for å sikre at grunnlinjen oppfyller gjeldende veiledning.</span><span class="sxs-lookup"><span data-stu-id="3842e-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="3842e-112">Sikkerhetskonsollen for grunnlinjer i Endepunktsikkerhet tillater ulike versjoner å sammenlignes ved å gjøre endringene fra versjon til versjon synlig.</span><span class="sxs-lookup"><span data-stu-id="3842e-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="3842e-113">Hvis du vil ha veiledning i hvordan du mest effektivt endrer hvilken versjon av grunnlinje som distribueres, kan du se [Behandle profiler for sikkerhetsgrunnlinjer i Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="3842e-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="3842e-114">Når du har distribuert en grunnkonfigurasjon for sikkerhet, kan du overvåke tilstanden til distribusjonen og se gjennom innstillingene på enhetsbasis.</span><span class="sxs-lookup"><span data-stu-id="3842e-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="3842e-115">**Merk:** Det kan ta opptil 24 timer før rapporteringsdataene for grunnlinjer vises fra den første distribusjonen til en enhet, og opptil seks timer for ytterligere oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="3842e-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="3842e-116">Den vanligste årsaken til at en grunnlinje-innstilling ikke brukes, er at den samme innstillingen brukes i en annen profil.</span><span class="sxs-lookup"><span data-stu-id="3842e-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="3842e-117">Dette scenarioet kan undersøkes for bestemte enheter ved å velge den aktuelle enheten fra Enhetsstatus-noden i profilen for Grunnkonfigurasjon for sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="3842e-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="3842e-118">Hvis du vil ha mer informasjon, kan du se [Løse konflikter for grunnkonfigurasjoner for sikkerhet](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="3842e-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>