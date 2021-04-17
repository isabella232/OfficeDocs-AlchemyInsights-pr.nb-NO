---
title: Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823472"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="ca8c1-102">Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ca8c1-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="ca8c1-103">Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="ca8c1-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="ca8c1-104">Noen vanlige feilmeldinger og løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="ca8c1-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="ca8c1-105">**Enhetsgrense nådd** Brukeren har flere enheter registrert enn enhetsgrensen.</span><span class="sxs-lookup"><span data-stu-id="ca8c1-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="ca8c1-106">Se gjennom disse dokumentene for [å fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller endre [enhetsgrensen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="ca8c1-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="ca8c1-107">**Denne tjenesten støttes ikke. Ingen registreringspolicy:** Apple Push Notification Service (APNS) må konfigureres eller fornyes.</span><span class="sxs-lookup"><span data-stu-id="ca8c1-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="ca8c1-108">Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette.</span><span class="sxs-lookup"><span data-stu-id="ca8c1-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="ca8c1-109">**Brukerlisenstype Ugyldig eller Brukernavn gjenkjennes ikke:** Brukeren må tilordnes en Intune- eller EMS-lisens.</span><span class="sxs-lookup"><span data-stu-id="ca8c1-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="ca8c1-110">Se gjennom disse dokumentene for å tilordne en lisens gjennom: [Administrasjonssenter for Office](https://docs.microsoft.com/intune/licenses-assign) eller [Azure-portalen.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="ca8c1-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="ca8c1-111">Flere ressurser for å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="ca8c1-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="ca8c1-112">Bruk [Feilsøkingsportalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil.</span><span class="sxs-lookup"><span data-stu-id="ca8c1-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ca8c1-113">Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="ca8c1-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="ca8c1-114">Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og løsninger for hver av dem: [Feilsøkingsveiledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [Feilsøking av dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ca8c1-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="ca8c1-115">[Lær hvordan du kan registrere iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="ca8c1-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

