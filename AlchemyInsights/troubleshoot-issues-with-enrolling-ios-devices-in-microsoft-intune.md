---
title: Feilsøk problemer med registrering av iOS-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507012"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="2ff11-102">Feilsøk problemer med registrering av iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2ff11-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="2ff11-103">Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="2ff11-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2ff11-104">Noen vanlige feilmeldinger og løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="2ff11-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="2ff11-105">**Enhet cap nådd** Brukeren har flere enheter registrert enn enhetsgrensen.</span><span class="sxs-lookup"><span data-stu-id="2ff11-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="2ff11-106">Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [endre enhetens grense](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="2ff11-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="2ff11-107">**Denne tjenesten støttes ikke. Ingen registrerings policy:** Apple Push Notification Service (APNS) må konfigureres eller fornyes.</span><span class="sxs-lookup"><span data-stu-id="2ff11-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="2ff11-108">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette.</span><span class="sxs-lookup"><span data-stu-id="2ff11-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="2ff11-109">**Brukerlisens type ugyldig eller brukernavn gjenkjennes ikke:** Brukeren må tilordnes en Intune-eller EMS-lisens.</span><span class="sxs-lookup"><span data-stu-id="2ff11-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="2ff11-110">Se gjennom disse dokumentene for å tilordne en lisens via: [Office Administrasjonssenter](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="2ff11-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="2ff11-111">Flere ressurser som kan hjelpe deg med å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="2ff11-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2ff11-112">Bruk [feilsøkings portalen for Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registreringsfeil.</span><span class="sxs-lookup"><span data-stu-id="2ff11-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="2ff11-113">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="2ff11-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2ff11-114">Se gjennom disse dokumentene for en liste over vanlige feil som forhindrer registrering og løsninger for hver: [feilsøkingsveiledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [feilsøking av dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="2ff11-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="2ff11-115">[Finn ut hvordan du registrerer IOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="2ff11-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

