---
title: Problemer med å installere Microsoft Defender på Mac eller Linux
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
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539689"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="0b1ec-102">Problemer med å installere Microsoft Defender på Mac eller Linux</span><span class="sxs-lookup"><span data-stu-id="0b1ec-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="0b1ec-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="0b1ec-103">**Mac**</span></span>

- <span data-ttu-id="0b1ec-104">Kontroller at systemkravene er oppfylt før du installerer Microsoft Defender ATP for Mac.</span><span class="sxs-lookup"><span data-stu-id="0b1ec-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="0b1ec-105">Hvis du vil ha mer informasjon, kan du [se Slik installerer du Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="0b1ec-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="0b1ec-106">Se gjennom informasjonen i filen: «/Bibliotek/Logger/Microsoft/mdatp/install.log».</span><span class="sxs-lookup"><span data-stu-id="0b1ec-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="0b1ec-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="0b1ec-107">**Linux**</span></span>

- <span data-ttu-id="0b1ec-108">Kontroller at systemkravene er oppfylt før du installerer Microsoft Defender ATP for Linux.</span><span class="sxs-lookup"><span data-stu-id="0b1ec-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="0b1ec-109">Hvis du vil ha mer informasjon, kan du [se Slik installerer du MDATP for Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="0b1ec-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="0b1ec-110">Hvis du vil MDATP at tjenesten kjører, kan du se [Installasjonen mislyktes](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="0b1ec-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="0b1ec-111">Hvis du vil feilsøke og løse problemer hvis tjenesten ikke kjører, kan du se Fremgangsmåte for å [feilsøke hvis mdatp-tjenesten ikke kjører](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="0b1ec-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="0b1ec-112">Hvis du vil se fremgangsmåten for å kontrollere klientkonfigurasjonen, som bekrefter produktets tilstand og kjører en gjenkjenningstest på EICAR-tekstfilen, kan du se [Klientkonfigurasjon](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="0b1ec-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="0b1ec-113">**Obs!** Hvis du vil ha en liste over støttede filsystemer for on-access-aktivitet, [kan du Microsoft Defender ATP for Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="0b1ec-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>