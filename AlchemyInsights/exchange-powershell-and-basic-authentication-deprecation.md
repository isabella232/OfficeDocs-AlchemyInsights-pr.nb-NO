---
title: Avvikling av enkel godkjenning i Exchange PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813481"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="2b279-102">Avvikling av enkel godkjenning i Exchange PowerShell</span><span class="sxs-lookup"><span data-stu-id="2b279-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="2b279-103">Hvis du vil ha mer informasjon om hvordan du kobler til Exchange Online PowerShell uten å bruke enkel godkjenning, [kan du gå hit](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="2b279-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="2b279-104">PowerShell V2-modulen bruker ikke enkel godkjenning.</span><span class="sxs-lookup"><span data-stu-id="2b279-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="2b279-105">Vær oppmerksom på at enkel godkjenning fremdeles må aktiveres på klientdatamaskinen.</span><span class="sxs-lookup"><span data-stu-id="2b279-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="2b279-106">Den nye PowerShell V2-modulen bruker moderne godkjenning for å opprette en kobling for å aktivere alle REST-baserte V2-cmdleter.</span><span class="sxs-lookup"><span data-stu-id="2b279-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="2b279-107">I tillegg til V2-cmdlet-er kan du også få tilgang til eldre eksterne PowerShell-cmdleter (RPS) som krever opprettelse av en ekstern PowerShell-økt.</span><span class="sxs-lookup"><span data-stu-id="2b279-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="2b279-108">Hvis du vil opprette en RPS-økt på Windows-maskinen, må WinRM BasicAuth være aktivert på klientmaskinen, selv om modulen bruker moderne godkjenning-mekanisme til å godkjenne til tjenesten.</span><span class="sxs-lookup"><span data-stu-id="2b279-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="2b279-109">Samlebåndet for enkel WinRM-godkjenning brukes til å transportere moderne godkjenningstokener.</span><span class="sxs-lookup"><span data-stu-id="2b279-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="2b279-110">Hvis enkel WinRM-godkjenning deaktiveres på klientdatamaskinen, vil nye V2-cmdlet-er fortsette å fungere (men de eldre RPS-cmdletene vil ikke gjøre det).</span><span class="sxs-lookup"><span data-stu-id="2b279-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
