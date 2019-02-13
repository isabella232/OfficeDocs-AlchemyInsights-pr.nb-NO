---
title: Feilsøke problemer med registrering av iOS enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924777"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="b0260-102">Feilsøke problemer med registrering av iOS enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b0260-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="b0260-103">Se gjennom ressursene som vises nedenfor for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="b0260-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="b0260-104">Noen vanlige feilmeldinger og Løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="b0260-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="b0260-p101">**Enheten Cap nådd** Brukeren har flere enheter som er registrert enn enhetsgrensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) , eller [Endre begrensningen for enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="b0260-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="b0260-p102">**Denne tjenesten støttes ikke. Ingen registreringspolicyen:** Apple Push Notification Service (APNER) må konfigureres eller fornyes. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette.</span><span class="sxs-lookup"><span data-stu-id="b0260-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="b0260-p103">**Ugyldig bruker-lisens eller brukernavnet gjenkjennes ikke:** Brukeren må være tilordnet en Intune eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="b0260-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="b0260-111">Ytterligere ressurser til å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="b0260-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="b0260-p104">Bruke [Intune feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrering-feil. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="b0260-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="b0260-114">Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og løsninger for hver: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [feilsøking dok](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="b0260-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="b0260-115">[Lær hvordan du kan registrere iOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="b0260-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

