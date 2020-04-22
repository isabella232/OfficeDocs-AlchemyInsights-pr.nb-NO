---
title: Feilsøke problemer med å registrere Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759629"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="99ce4-102">Feilsøke problemer med å registrere Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="99ce4-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="99ce4-103">Se gjennom ressursene som er oppført nedenfor for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="99ce4-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="99ce4-104">Noen vanlige problemer og løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="99ce4-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="99ce4-105">**Enheten ikke kryptert feil i Firmaportal:** Nyere versjoner av Android, spesielt fra og med v7.0, krever et oppstartspassord for å sikre at enheten din er fullstendig kryptert.</span><span class="sxs-lookup"><span data-stu-id="99ce4-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="99ce4-106">Vanlige løsninger er å aktivere en oppstartspinne eller kryptere enheten helt.</span><span class="sxs-lookup"><span data-stu-id="99ce4-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="99ce4-107">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="99ce4-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="99ce4-108">**Enheter kan ikke sjekke inn med Intune-tjenesten eller vise som "Usunn" i Intune admin-konsollen:** Noen Samsung 4.4- og 5.5-enheter kan ikke sjekke inn i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="99ce4-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="99ce4-109">Det finnes 3 mulige løsninger på dette problemet:</span><span class="sxs-lookup"><span data-stu-id="99ce4-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="99ce4-110">Åpne Intune Company Portal-appen manuelt, som automatisk starter en enhetssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="99ce4-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="99ce4-111">Oppdater enheten til Android 6.0 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="99ce4-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="99ce4-112">Deaktiver Samsung Smart Manager fra å administrere Intune Company Portal.</span><span class="sxs-lookup"><span data-stu-id="99ce4-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="99ce4-113">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for mer informasjon om disse problemene og løsningene.</span><span class="sxs-lookup"><span data-stu-id="99ce4-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="99ce4-114">**Brukerlisenstype Ugyldig** eller **Brukernavn gjenkjennes ikke feil:** Brukeren må tilordnes en Intune- eller EMS-lisens.</span><span class="sxs-lookup"><span data-stu-id="99ce4-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="99ce4-115">Se gjennom disse dokumentene for å tilordne en lisens via: Administrasjonssenter for Office eller Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="99ce4-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="99ce4-116">Flere ressurser som kan løse problemet:</span><span class="sxs-lookup"><span data-stu-id="99ce4-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="99ce4-117">Bruk [Intune Feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil.</span><span class="sxs-lookup"><span data-stu-id="99ce4-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="99ce4-118">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="99ce4-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="99ce4-119">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som hindrer registrering og oppløsning er til hver av dem.</span><span class="sxs-lookup"><span data-stu-id="99ce4-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="99ce4-120">[Finn ut hvordan du registrerer Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="99ce4-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
