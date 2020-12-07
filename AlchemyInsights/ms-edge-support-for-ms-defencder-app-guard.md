---
title: Microsoft Edges støtte for Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584016"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="52a1e-102">Microsoft Edges støtte for Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="52a1e-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="52a1e-103">Utformet for Windows 10 og Microsoft Edge bruker Application Guard en metode for maskin vare isolasjon som lar en bruker navigere i et uklarert nettsted fra en isolert, Hyper-V-aktivert beholder, atskilt fra verts operativ systemet.</span><span class="sxs-lookup"><span data-stu-id="52a1e-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="52a1e-104">En organisasjons administrator definerer en liste over klarerte nett steder, Sky ressurser og interne nettverk.</span><span class="sxs-lookup"><span data-stu-id="52a1e-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="52a1e-105">Når en bruker besøker et nettsted som ikke er i listen, vil Microsoft Edge åpne området i beholderen.</span><span class="sxs-lookup"><span data-stu-id="52a1e-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="52a1e-106">Dette betyr at hvis området blir skadelig, forblir Verts-PCen beskyttet, og angriperen vil ikke få tilgang til virksomhets dataene.</span><span class="sxs-lookup"><span data-stu-id="52a1e-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="52a1e-107">Installasjon av utvidelser i beholderen støttes på Microsoft Edge versjon 81, og den kan kontrolleres via en policy.</span><span class="sxs-lookup"><span data-stu-id="52a1e-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="52a1e-108">UpdateURL-adressen som brukes i ExtensionInstallForcelist-policyen, skal legges til som en nøytral ressurs i policyene for nettverks isolasjon som brukes av Application Guard.</span><span class="sxs-lookup"><span data-stu-id="52a1e-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="52a1e-109">Hvis du vil ha mer informasjon, kan du se [Microsoft Edge-støtte for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="52a1e-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
