---
title: Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708971"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="61c79-102">Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="61c79-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="61c79-103">Se gjennom ressursene som er oppført nedenfor for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="61c79-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="61c79-104">Noen vanlige feilmeldinger og løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="61c79-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="61c79-105">**Enhetsgrense nådd** Brukeren har flere enheter registrert enn enhetsgrensen.</span><span class="sxs-lookup"><span data-stu-id="61c79-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="61c79-106">Se gjennom disse dokumentene [for å fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller endre [enhetsgrensen.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="61c79-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="61c79-107">**Denne tjenesten støttes ikke. Ingen registreringspolicy:** Apple Push Notification Service (APNS) må konfigureres eller fornyes.</span><span class="sxs-lookup"><span data-stu-id="61c79-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="61c79-108">Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette.</span><span class="sxs-lookup"><span data-stu-id="61c79-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="61c79-109">**Brukerlisenstype ugyldig eller brukernavn gjenkjennes ikke:** Brukeren må tildeles en Intune- eller EMS-lisens.</span><span class="sxs-lookup"><span data-stu-id="61c79-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="61c79-110">Se gjennom disse dokumentene for å tilordne en lisens via [administrasjonssenteret for Office eller](https://docs.microsoft.com/intune/licenses-assign) [Azure Portal.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="61c79-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="61c79-111">Flere ressurser som kan hjelpe deg med å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="61c79-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="61c79-112">Bruk [feilsøkingsportalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil.</span><span class="sxs-lookup"><span data-stu-id="61c79-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="61c79-113">Se [gjennom dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="61c79-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="61c79-114">Se gjennom disse dokumentene for å få en liste over vanlige feil som hindrer registrering og løsninger for hver av [dem:](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) Feilsøkingsveiledning og [Feilsøking av dokumenter.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="61c79-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="61c79-115">[Finn ut hvordan du registrere iOS-enheter i Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="61c79-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

