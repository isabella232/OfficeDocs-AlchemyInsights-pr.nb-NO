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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669257"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="1eb40-102">Feilsøke problemer med registrering av iOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1eb40-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="1eb40-103">Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="1eb40-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="1eb40-104">Noen vanlige feil meldinger og løsnings trinn:</span><span class="sxs-lookup"><span data-stu-id="1eb40-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="1eb40-105">**Enhetens ende** punkt er nådd Brukeren har flere enheter som ble registrert enn enhets grensen.</span><span class="sxs-lookup"><span data-stu-id="1eb40-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="1eb40-106">Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [endre enhets grensen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="1eb40-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="1eb40-107">**Denne tjenesten støttes ikke. Ingen registrerings policy:** Apple Push Notification-tjeneste (APNS) må konfigureres eller fornyes.</span><span class="sxs-lookup"><span data-stu-id="1eb40-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="1eb40-108">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instruksjoner om hvordan du gjør dette.</span><span class="sxs-lookup"><span data-stu-id="1eb40-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="1eb40-109">**Bruker lisens typen er ugyldig eller bruker navnet gjenkjennes ikke:** Brukeren må være tilordnet en Intune-eller EMS-lisens.</span><span class="sxs-lookup"><span data-stu-id="1eb40-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="1eb40-110">Se gjennom disse dokumentene for å tilordne en lisens gjennom: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) eller [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="1eb40-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="1eb40-111">Flere ressurser som kan hjelpe deg med å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="1eb40-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1eb40-112">Bruk [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrerings feil.</span><span class="sxs-lookup"><span data-stu-id="1eb40-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1eb40-113">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="1eb40-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="1eb40-114">Se gjennom disse dokumentene for en liste over vanlige feil som forhindrer registrering og løsninger på hver av dem: [feil søkings veiledning](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) og [feil søkings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="1eb40-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="1eb40-115">[Lær hvordan du registrerer IOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="1eb40-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

