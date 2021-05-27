---
title: Feilsøking av ediscovery inneholder feil
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676277"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="c2f69-102">Feilsøking av ediscovery inneholder feil</span><span class="sxs-lookup"><span data-stu-id="c2f69-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="c2f69-103">Har du problemer med eDiscovery-sperringer?</span><span class="sxs-lookup"><span data-stu-id="c2f69-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="c2f69-104">Her er noen anbefalte fremgangsmåter du bør vurdere:</span><span class="sxs-lookup"><span data-stu-id="c2f69-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="c2f69-105">Kontroller sperredistribusjonsstatusen.</span><span class="sxs-lookup"><span data-stu-id="c2f69-105">Check the hold distribution status.</span></span>  <span data-ttu-id="c2f69-106">Hvis statusen er **På (venter)** eller **Av (venter),** venter du på at sperrefordelingen skal fullføres.</span><span class="sxs-lookup"><span data-stu-id="c2f69-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="c2f69-107">Slå sammen oppdateringer for eDiscovery-sperring til én enkelt masseforespørsel i stedet for å oppdatere policyen gjentatte ganger for hver transaksjon.</span><span class="sxs-lookup"><span data-stu-id="c2f69-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="c2f69-108">Kjør Set-CaseHoldPolicy <policyname> -RetryDistribution i Powershell for sikkerhets- og samsvarssenteret.</span><span class="sxs-lookup"><span data-stu-id="c2f69-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="c2f69-109">Hvis du vil ha mer [informasjon, kan du Koble til sikkerhets-& PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="c2f69-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="c2f69-110">Hvis du vil ha fremgangsmåter for å kontrollere disse innstillingene og flere anbefalte fremgangsmåter for å begrense og løse problemer med eDiscovery-sperringer, kan du se Feilsøke [problemer med sperring av eDiscovery](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="c2f69-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="c2f69-111">Hvis du vil ha informasjon om feilsøking av andre vanlige eDiscovery-problemer, kan du se Undersøke, feilsøke og løse vanlige [eDiscovery-problemer](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="c2f69-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
