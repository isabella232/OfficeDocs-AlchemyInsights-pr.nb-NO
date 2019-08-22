---
title: Feil under sending av e-post blokkert av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527149"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="f4ead-102">Feil under sending av e-post: klient-vert som er blokkert ved hjelp av Spamhaus</span><span class="sxs-lookup"><span data-stu-id="f4ead-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="f4ead-103">IP-adressen som sendte meldingen, er på en blokkeringsliste som eies av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="f4ead-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="f4ead-104">For blir blokkert av Spamhaus årsaker utsatt kontoer utsatt maskiner som deler en offentlig IP-adresse og retningslinjer for Internett-leverandør (ISP).</span><span class="sxs-lookup"><span data-stu-id="f4ead-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="f4ead-105">Det er mulig reparasjoner:</span><span class="sxs-lookup"><span data-stu-id="f4ead-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="f4ead-106">Du må finne årsaken og fjerne blokkeringen fra webområdet Spamhaus for blokkerte innkommende meldinger til Office 365 der du kan kontrollere e-kildeserveren.</span><span class="sxs-lookup"><span data-stu-id="f4ead-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="f4ead-107">For blokkerte innkommende meldinger til Office 365 der kildens IP-adresse tilhører noen andre, må eieren av adressen du kan fjerne blokkeringen fra webområdet Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="f4ead-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="f4ead-108">Hvis IP-adressen på policyen Block liste (PBL), kan eieren tilordner en annen statisk IP-adresse eller fjerne adressen fra PBL.</span><span class="sxs-lookup"><span data-stu-id="f4ead-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="f4ead-109">For blokkerte utgående meldinger fra Office 365-domenet, kan du få denne feilmeldingen hvis meldingene rutes via en 3 part.</span><span class="sxs-lookup"><span data-stu-id="f4ead-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="f4ead-110">Du kan bruke et verktøy for WHOIS-oppslag til å finne den blokkerte IP-adresse eieren.</span><span class="sxs-lookup"><span data-stu-id="f4ead-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
