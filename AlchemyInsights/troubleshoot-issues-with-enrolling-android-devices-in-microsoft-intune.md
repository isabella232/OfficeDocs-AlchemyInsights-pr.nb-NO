---
title: Feilsøke problemer med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689963"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="4a251-102">Feilsøke problemer med registrering av Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="4a251-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="4a251-103">Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="4a251-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="4a251-104">Noen vanlige problemer og løsnings trinn:</span><span class="sxs-lookup"><span data-stu-id="4a251-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="4a251-105">**Enhet ikke kryptert-feil i firma portalen:** Nyere versjoner av Android, spesielt fra og med v 7.0, krever et oppstarts passord for å sikre at enheten er helt kryptert.</span><span class="sxs-lookup"><span data-stu-id="4a251-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="4a251-106">Vanlige løsninger er å aktivere en oppstarts-PIN-kode eller kryptere enheten fullstendig.</span><span class="sxs-lookup"><span data-stu-id="4a251-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="4a251-107">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="4a251-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="4a251-108">**Enheter kan ikke sjekke inn med Intune-tjenesten eller vise som "inhealth" i administrasjons konsollen for Intune:** Enkelte Samsung 4,4-og 5,5-enheter kan kanskje ikke sjekke inn tjenesten.</span><span class="sxs-lookup"><span data-stu-id="4a251-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="4a251-109">Det er tre mulige løsninger på dette problemet:</span><span class="sxs-lookup"><span data-stu-id="4a251-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="4a251-110">Åpne Intune Company Portal-appen manuelt, som automatisk vil starte en enhets synkronisering.</span><span class="sxs-lookup"><span data-stu-id="4a251-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="4a251-111">Oppdater enheten til Android 6,0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="4a251-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="4a251-112">Deaktivere Samsung smart Manager fra administrasjon av Intune Company Portal.</span><span class="sxs-lookup"><span data-stu-id="4a251-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="4a251-113">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for mer informasjon om disse problemene og løsningene.</span><span class="sxs-lookup"><span data-stu-id="4a251-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="4a251-114">**Bruker lisens typen er ugyldig** eller **bruker navnet er ukjent feil:** brukeren må tilordnes en Intune-eller EMS-lisens.</span><span class="sxs-lookup"><span data-stu-id="4a251-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="4a251-115">Se gjennom disse dokumentene for å tilordne en lisens gjennom: Office Admin Center eller Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="4a251-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="4a251-116">Flere ressurser som kan hjelpe deg med å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="4a251-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4a251-117">Bruk [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrerings feil.</span><span class="sxs-lookup"><span data-stu-id="4a251-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4a251-118">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="4a251-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="4a251-119">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som forhindrer registrering og løsninger på hver av dem.</span><span class="sxs-lookup"><span data-stu-id="4a251-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="4a251-120">[Lær hvordan du registrerer Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="4a251-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
