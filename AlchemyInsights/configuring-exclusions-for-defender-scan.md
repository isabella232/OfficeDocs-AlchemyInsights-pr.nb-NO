---
title: Konfigurere utelatelser for ATP-skanning for Microsoft Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713900"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="a68b0-102">Konfigurere utelatelser for ATP-skanning for Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="a68b0-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="a68b0-103">Generelt sett kan du utelate bestemte filtyper og mappeplasseringer fra ATP-skanninger med Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="a68b0-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="a68b0-104">Du kan også konfigurere utelatelser for filer som åpnes av bestemte prosesser.</span><span class="sxs-lookup"><span data-stu-id="a68b0-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="a68b0-105">Hvis du vil ha mer [informasjon,](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) kan du se konfigurere og validere utelatelser basert på filtype og mappeplassering og konfigurere utelatelser for filer som åpnes [av prosesser.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="a68b0-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="a68b0-106">Hvis du vil konfigurere utelatelser for **Windows Server 2016 og 2019,** kan du se Konfigurere [microsoft Defender Antivirus-utelatelser på Windows Server.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="a68b0-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="a68b0-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="a68b0-107">**Mac**</span></span>

<span data-ttu-id="a68b0-108">Hvis du vil ha mer informasjon om støttede utelatelsestyper [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) og konfigurering av en liste over utelatelser for Mac, kan du se støttede utelatelsestyper og hvordan du konfigurerer listen over [utelatelser.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="a68b0-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="a68b0-109">**Obs!** Du kan også validere utelatelseslister ved hjelp av EICAR-testfilen.</span><span class="sxs-lookup"><span data-stu-id="a68b0-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="a68b0-110">Hvis du vil ha mer informasjon, kan du se Validere lister over utelatelser [med EICAR-testfilen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="a68b0-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="a68b0-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="a68b0-111">**Linux**</span></span>

<span data-ttu-id="a68b0-112">Hvis du vil ha mer informasjon om støttede utelatelsestyper [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) og konfigurering av en liste over utelatelser for Linux, kan du se støttede utelatelsestyper og konfigurere og validere utelatelser [for Microsoft Defender ATP for Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="a68b0-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="a68b0-113">**Obs!** Du kan også validere utelatelseslister ved hjelp av EICAR-testfilen.</span><span class="sxs-lookup"><span data-stu-id="a68b0-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="a68b0-114">Hvis du vil ha mer informasjon, kan du se Validere lister over utelatelser [med EICAR-testfilen.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="a68b0-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 