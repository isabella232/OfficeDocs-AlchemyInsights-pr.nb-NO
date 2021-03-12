---
title: Kan ikke sende/motta e-post til/fra Office 365 på grunn av TLS 1.0- og TLS 1.1-deaktiveringen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747122"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="677cd-102">Kan ikke sende/motta e-post til/fra Office 365 på grunn av TLS 1.0- og TLS 1.1-deaktiveringen</span><span class="sxs-lookup"><span data-stu-id="677cd-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="677cd-103">Som bekreftet av meldingssenteret ble MC229914, TLS 1.0 og TLS 1.1-avviklingen startet å håndheve for Exchange Online-endepunkter for e-postflyt.</span><span class="sxs-lookup"><span data-stu-id="677cd-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="677cd-104">Snart godtar ikke Office 365 TLS 1.0- og TLS 1.1-e-posttilkoblinger fra eksterne kilder.</span><span class="sxs-lookup"><span data-stu-id="677cd-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="677cd-105">Exchange Online bruker heller aldri TLS 1.0 eller 1.1 til å sende utgående e-post.</span><span class="sxs-lookup"><span data-stu-id="677cd-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="677cd-106">Hvis du har problemer på grunn av TLS 1.0- eller 1.1-deaktivering, kan du oppleve en av følgende feil:</span><span class="sxs-lookup"><span data-stu-id="677cd-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="677cd-107">Avsenderen får NDR-retur - '421 4.4.2 Tilkobling ble brutt på grunn av SocketError'</span><span class="sxs-lookup"><span data-stu-id="677cd-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="677cd-108">Feil i køvisningsprogrammet for lokal server som sender e-post til Officer 365- '421 4.4.2-tilkobling droppet på grunn av SocketError'</span><span class="sxs-lookup"><span data-stu-id="677cd-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="677cd-109">Feil i Logg for Send [koblingsprotokoll](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) på serveren som sender e-post til Office 365– TLS-forhandling mislyktes med feilen SocketError</span><span class="sxs-lookup"><span data-stu-id="677cd-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="677cd-110">Feil i protokollloggen for Send eller motta kobling – '451 5.7.3 Må utstede en STARTTLS-kommando først'</span><span class="sxs-lookup"><span data-stu-id="677cd-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="677cd-111">Hvis du opplever noen av feilene ovenfor, må du kontrollere at serveren som sender eller mottar e-post, har TLS 1.2 aktivert ved å kontrollere følgende registernøkler:</span><span class="sxs-lookup"><span data-stu-id="677cd-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="677cd-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:0000000 "Enabled"=dword:0000001**</span><span class="sxs-lookup"><span data-stu-id="677cd-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="677cd-113">Hvis du gjør endringer i registernøklene ovenfor for å aktivere TLS 1.2, starter du serveren på nytt for at endringene skal tre i kraft.</span><span class="sxs-lookup"><span data-stu-id="677cd-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="677cd-114">Kontroller også at du har de nyeste Windows- og Exchange-oppdateringene installert.</span><span class="sxs-lookup"><span data-stu-id="677cd-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="677cd-115">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="677cd-115">For more information, see:</span></span>

- [<span data-ttu-id="677cd-116">Veiledning for Exchange Server TLS, del 1: Gjør deg klar for TLS 1.2 – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="677cd-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="677cd-117">Veiledning for Exchange Server TLS Del 2: Aktivere TLS 1.2 og identifisere klienter som ikke bruker det – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="677cd-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="677cd-118">Forstå e-postscenarioer hvis TLS-versjoner ikke kan avtales med Exchange Online – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="677cd-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
