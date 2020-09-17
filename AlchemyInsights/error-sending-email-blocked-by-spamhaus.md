---
title: Feil under sending av e-post blokkert av SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783812"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="c5cf3-102">Feil under sending av e-post: klient vert blokkert ved hjelp av Spamhaus</span><span class="sxs-lookup"><span data-stu-id="c5cf3-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="c5cf3-103">IP-adressen som sendte meldingen, er i en blokkerings liste som eies av [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="c5cf3-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="c5cf3-104">Årsaker til at du blir blokkert av Spamhaus inkluderer kompromitterte kontoer, som har brutte maskiner som deler en offentlig IP-adresse og retnings linjer for Internett-leverandør (ISP).</span><span class="sxs-lookup"><span data-stu-id="c5cf3-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="c5cf3-105">Mulige løsninger er:</span><span class="sxs-lookup"><span data-stu-id="c5cf3-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="c5cf3-106">For blokkerte inn kommende meldinger der du styrer kilde-e-postserveren, må du finne årsaken og fjerne blokken fra Spamhaus-nettstedet.</span><span class="sxs-lookup"><span data-stu-id="c5cf3-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="c5cf3-107">For blokkerte inn kommende meldinger der kilde-IP-adressen tilhører noen andre, må adresse eieren fjerne blokken fra Spamhaus-nettstedet.</span><span class="sxs-lookup"><span data-stu-id="c5cf3-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="c5cf3-108">Hvis IP-adressen er i policyen for policy blokkering (PBL), kan eieren tilordne en annen statisk IP-adresse eller fjerne adressen fra PBL.</span><span class="sxs-lookup"><span data-stu-id="c5cf3-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="c5cf3-109">For blokkerte utgående meldinger fra domenet som er koblet til Microsoft, kan du få denne feilen hvis meldingene er rutet gjennom en tredje parts tjeneste.</span><span class="sxs-lookup"><span data-stu-id="c5cf3-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="c5cf3-110">Du kan bruke et WHOIS-oppslags verktøy til å finne den blokkerte IP-adressen som eier.</span><span class="sxs-lookup"><span data-stu-id="c5cf3-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
