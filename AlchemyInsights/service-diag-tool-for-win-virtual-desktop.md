---
title: Tjeneste diagnose verktøy for Windows virtuelt skrive bord
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680238"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="02c49-102">Tjeneste diagnose verktøy for Windows virtuelt skrive bord</span><span class="sxs-lookup"><span data-stu-id="02c49-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="02c49-103">Windows Virtual Desktop (WVD) har et diagnose verktøy som lar administratorer identifisere feil via ett enkelt grensesnitt.</span><span class="sxs-lookup"><span data-stu-id="02c49-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="02c49-104">Dette verktøyet logger diagnose relatert informasjon når WVD brukes av noen som er tilordnet en WVD-rolle.</span><span class="sxs-lookup"><span data-stu-id="02c49-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="02c49-105">Hver Logg inneholder informasjon om WVD-rollen som er involvert i aktiviteten, feil meldingene som vises under økten og informasjon om leieren og brukeren.</span><span class="sxs-lookup"><span data-stu-id="02c49-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="02c49-106">Azure log Analytics kan konfigureres til å registrere aktivitets loggen som er opprettet av diagnose verktøyet.</span><span class="sxs-lookup"><span data-stu-id="02c49-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="02c49-107">Slik gjør du det:</span><span class="sxs-lookup"><span data-stu-id="02c49-107">Here's how:</span></span>

1. <span data-ttu-id="02c49-108">Opprett et Logg analyse arbeidsom råde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="02c49-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="02c49-109">[Koble Windows-datamaskiner til Azure-skjerm](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="02c49-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="02c49-110">Få arbeidsområde-ID-en og primær nøkkelen for arbeidsom rådet.</span><span class="sxs-lookup"><span data-stu-id="02c49-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="02c49-111">Installasjons vei viseren trenger denne informasjonen for å konfigurere agenten på riktig måte og sikre at den kan kommunisere med Azure-skjermen.</span><span class="sxs-lookup"><span data-stu-id="02c49-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="02c49-112">[Push diagnose data til arbeidsom rådet](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="02c49-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="02c49-113">Du kan skyve diagnose data fra WVD-leieren til Logg analysen for arbeidsom rådet.</span><span class="sxs-lookup"><span data-stu-id="02c49-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="02c49-114">[Identifisere og diagnostisere problemer](https://go.microsoft.com/fwlink/?linkid=2128338) som er interne eller eksterne i forhold til WVD.</span><span class="sxs-lookup"><span data-stu-id="02c49-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="02c49-115">Hvis du vil ha mer informasjon om hvordan du konfigurerer tjeneste diagnose verktøyet for WVD, kan du se [bruke Logg analyse for diagnose funksjonen](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="02c49-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
