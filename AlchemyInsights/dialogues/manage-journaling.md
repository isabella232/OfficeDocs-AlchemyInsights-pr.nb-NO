---
title: Behandle loggføring
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526140"
---
# <a name="manage-journaling"></a><span data-ttu-id="0d771-102">Behandle loggføring</span><span class="sxs-lookup"><span data-stu-id="0d771-102">Manage journaling</span></span>

<span data-ttu-id="0d771-103">Loggføring kan hjelpe organisasjonen med å svare på juridiske, forskriftsmessige og organisatoriske samsvarskrav ved å registrere inngående og utgående e-postkommunikasjon.</span><span class="sxs-lookup"><span data-stu-id="0d771-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="0d771-104">Husk:</span><span class="sxs-lookup"><span data-stu-id="0d771-104">Keep in mind:</span></span>

* <span data-ttu-id="0d771-105">Du må ha tillatelser [for organisasjonsbehandling](https://go.microsoft.com/fwlink/?linkid=2115259) og [postbehandling](https://go.microsoft.com/fwlink/?linkid=2115469) før du kan behandle loggføring.</span><span class="sxs-lookup"><span data-stu-id="0d771-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="0d771-106">Du må ha en loggpostboks og (valgfritt) en alternativ loggføringspostboks konfigurert.</span><span class="sxs-lookup"><span data-stu-id="0d771-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="0d771-107">Hvis du vil ha mer informasjon, [kan du se Konfigurere loggføring i Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="0d771-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="0d771-108">I Exchange Online er det en grense for hvor mange loggregler du kan opprette.</span><span class="sxs-lookup"><span data-stu-id="0d771-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="0d771-109">Hvis du vil ha mer informasjon, kan du se [regelgrenser for logg, transport og innboks.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="0d771-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="0d771-110">Exchange Online støtter ikke levering av loggrapporter til en Exchange Online-postboks.</span><span class="sxs-lookup"><span data-stu-id="0d771-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="0d771-111">Du må angi e-postadressen til et lokalt arkiveringssystem eller en tredjeparts arkiveringstjeneste som loggføringspostboksen.</span><span class="sxs-lookup"><span data-stu-id="0d771-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
