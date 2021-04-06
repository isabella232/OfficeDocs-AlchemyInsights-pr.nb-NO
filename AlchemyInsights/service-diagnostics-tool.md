---
title: Tjenestediagnoseverktøy for Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595865"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="7acf4-102">Tjenestediagnoseverktøy for Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="7acf4-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="7acf4-103">Windows Virtual Desktop (WVD) tilbyr et diagnoseverktøy som lar administratorer identifisere feil gjennom ett enkelt grensesnitt.</span><span class="sxs-lookup"><span data-stu-id="7acf4-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="7acf4-104">Dette verktøyet logger diagnoserelatert informasjon når WVD brukes av noen som har tilordnet en WVD-rolle.</span><span class="sxs-lookup"><span data-stu-id="7acf4-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="7acf4-105">Hver logg inneholder informasjon om WVD-rollen som er involvert i aktiviteten, feilmeldingene som vises under økten, og informasjonen om leieren og brukeren.</span><span class="sxs-lookup"><span data-stu-id="7acf4-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="7acf4-106">Azure Log Analytics kan konfigureres til å registrere aktivitetsloggen som er opprettet av diagnoseverktøyet, ved å følge disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="7acf4-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="7acf4-107">Opprett et Log Analytics-arbeidsområde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="7acf4-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="7acf4-108">[Koble Windows-datamaskiner til Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="7acf4-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="7acf4-109">Få arbeidsområde-ID-en og primærnøkkelen for arbeidsområdet.</span><span class="sxs-lookup"><span data-stu-id="7acf4-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="7acf4-110">Konfigurasjonsveiviseren trenger denne informasjonen for å konfigurere agenten på riktig måte, og for å sikre at den kan kommunisere med Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="7acf4-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="7acf4-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="7acf4-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="7acf4-112">Du kan flytte diagnosedata fra WVD-leieren til Logganalyse for arbeidsområdet.</span><span class="sxs-lookup"><span data-stu-id="7acf4-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="7acf4-113">[Identifiser og diagnostiser](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemer som er interne eller eksterne i forhold til WVD.</span><span class="sxs-lookup"><span data-stu-id="7acf4-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="7acf4-114">Hvis du vil lære mer om hvordan du konfigurerer tjenestediagnoseverktøyet for WVD, kan du se Bruke Logganalyse for diagnosefunksjonen.</span><span class="sxs-lookup"><span data-stu-id="7acf4-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>