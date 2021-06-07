---
title: Ytelsesproblemer for Microsoft Defender for endepunkt på Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794003"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="04a8e-102">Ytelsesproblemer for Microsoft Defender for endepunkt på Linux</span><span class="sxs-lookup"><span data-stu-id="04a8e-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="04a8e-103">Denne artikkelen veileder deg gjennom trinnene for å identifisere ytelsesproblemer for Microsoft Defender for endepunkt på Linux.</span><span class="sxs-lookup"><span data-stu-id="04a8e-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="04a8e-104">Det er viktig å først kontrollere at problemet du opplever, er løst med [den nyeste versjonen.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="04a8e-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="04a8e-105">Hvis du vil starte undersøkelsen, kan du se [Feilsøke ytelsesproblemer for Microsoft Defender for endepunkt på Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="04a8e-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="04a8e-106">Utelatelser</span><span class="sxs-lookup"><span data-stu-id="04a8e-106">Exclusions</span></span>

<span data-ttu-id="04a8e-107">Utelatelser kan bidra til å redusere ytelsesproblemer.</span><span class="sxs-lookup"><span data-stu-id="04a8e-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="04a8e-108">Se gjennom utelatelsene før du begynner, slik at eventuell ekstra risiko er kjent og dokumentert.</span><span class="sxs-lookup"><span data-stu-id="04a8e-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="04a8e-109">Hvis du vil ha mer informasjon, kan du se Konfigurere og validere utelatelser [for Microsoft Defender for endepunkt på Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="04a8e-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="04a8e-110">Når du har flere filer & mapper som skal utelates, og alle er på samme monteringspunkt, kan det være enklere å utelate monteringspunktet.</span><span class="sxs-lookup"><span data-stu-id="04a8e-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="04a8e-111">Fra og med februarutgivelse 101.22.80 kan du utelate et helt monteringspunkt.</span><span class="sxs-lookup"><span data-stu-id="04a8e-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="04a8e-112">Hvis for eksempel /mnt/backup er et monteringspunkt, kan du legge til /mnt/backup i ekskluderingslisten ved å kjøre denne kommandoen:</span><span class="sxs-lookup"><span data-stu-id="04a8e-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="04a8e-113">**Obs!** Hvis du legger til utelatelser, øker risikoen for at skadelig programvare ikke oppdages og bør håndteres og implementeres med forsiktighet.</span><span class="sxs-lookup"><span data-stu-id="04a8e-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="04a8e-114">Trenger du hjelp?</span><span class="sxs-lookup"><span data-stu-id="04a8e-114">Need Help?</span></span>

<span data-ttu-id="04a8e-115">Hvis du vil hjelpe deg på den mest effektive måten, kan du samle inn diagnosedataene før du åpner en støttesak.</span><span class="sxs-lookup"><span data-stu-id="04a8e-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
