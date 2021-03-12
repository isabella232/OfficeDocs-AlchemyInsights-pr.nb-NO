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
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709007"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="f03ff-102">Feilsøke problemer med registrering av Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f03ff-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="f03ff-103">Se gjennom ressursene som er oppført nedenfor for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="f03ff-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f03ff-104">Noen vanlige problemer og løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="f03ff-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="f03ff-105">**Enheten er ikke kryptert i firmaportalen:** Nyere versjoner av Android, spesielt fra og med v7.0, krever et oppstartspassord for å sikre at enheten er fullstendig kryptert.</span><span class="sxs-lookup"><span data-stu-id="f03ff-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="f03ff-106">Vanlige løsninger er å aktivere en oppstarts-PIN-kode eller fullstendig kryptere enheten.</span><span class="sxs-lookup"><span data-stu-id="f03ff-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="f03ff-107">Se [gjennom dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="f03ff-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="f03ff-108">Enheter kan ikke sjekke inn med Intune-tjenesten eller vises som «Ugyldige» i **Intune-administrasjonskonsollen:** Enkelte Samsung 4.4- og 5.5-enheter sjekker kanskje ikke inn tjenesten.</span><span class="sxs-lookup"><span data-stu-id="f03ff-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="f03ff-109">Det finnes tre mulige løsninger på dette problemet:</span><span class="sxs-lookup"><span data-stu-id="f03ff-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="f03ff-110">Åpne Firmaportal-appen for Intune manuelt, som automatisk starter en enhetssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="f03ff-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="f03ff-111">Oppdater enheten til Android 6.0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="f03ff-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="f03ff-112">Deaktiver Smart Manager for Samsung fra å administrere firmaportalen for Intune.</span><span class="sxs-lookup"><span data-stu-id="f03ff-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="f03ff-113">Se [gjennom dette dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for mer informasjon om disse problemene og løsningene.</span><span class="sxs-lookup"><span data-stu-id="f03ff-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="f03ff-114">**Feilmelding om ugyldig brukerlisenstype** **eller brukernavn gjenkjennes ikke:** Brukeren må tilordnes en Intune- eller EMS-lisens.</span><span class="sxs-lookup"><span data-stu-id="f03ff-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f03ff-115">Se gjennom disse dokumentene for å tilordne en lisens via administrasjonssenteret for Office eller Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="f03ff-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="f03ff-116">Flere ressurser som kan hjelpe deg med å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="f03ff-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f03ff-117">Bruk [feilsøkingsportalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil.</span><span class="sxs-lookup"><span data-stu-id="f03ff-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f03ff-118">Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="f03ff-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="f03ff-119">Se [gjennom dette dokumentet](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som forhindrer registrering og løsninger for hver av dem.</span><span class="sxs-lookup"><span data-stu-id="f03ff-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="f03ff-120">[Lær hvordan du registrere Android-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="f03ff-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
