---
title: Feilsøke problemer med registrering av Android-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655892"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="17302-102">Feilsøke problemer med registrering av Android-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="17302-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="17302-103">Se gjennom ressursene som vises nedenfor for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="17302-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="17302-104">Noen vanlige problemer og Løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="17302-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="17302-p101">**Enhet ikke kryptert feil i Company Portal:** Nyere versjoner av Android, spesielt fra og med v7.0, krever et passord for oppstart å forsikre deg om at enheten er fullstendig kryptert. Vanlige løsninger er å aktivere en PIN-kode for oppstart eller kryptere fullstendig enheten. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="17302-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="17302-p102">**Enheter kan ikke være på tjenesten Intune eller vise som "Unhealthy" i admin-konsollen Intune:** Noen Samsung 4.4 og 5.5 enheter kan ikke sjekke inn i tjenesten. Det er 3 mulige løsninger på dette problemet:</span><span class="sxs-lookup"><span data-stu-id="17302-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="17302-110">Åpne Intune Company Portal-app, som automatisk starter en enhetssynkronisering manuelt.</span><span class="sxs-lookup"><span data-stu-id="17302-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="17302-111">Oppdatere enheten til Android 6.0 eller høyere.</span><span class="sxs-lookup"><span data-stu-id="17302-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="17302-p103">Deaktiver Samsung Smart Manager fra å behandle Intune Company Portal. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for ytterligere informasjon om disse problemer og løsninger.</span><span class="sxs-lookup"><span data-stu-id="17302-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="17302-p104">**Brukeren lisens Type ugyldig** eller **bruker navnet ikke gjenkjennes feil:** brukeren må tilordnes en Intune eller EMS-lisens. Se gjennom disse dokumentene for å tilordne en lisens via: Office Admin Center eller Azure portal.</span><span class="sxs-lookup"><span data-stu-id="17302-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="17302-116">Ytterligere ressurser til å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="17302-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="17302-p105">Bruke [Intune feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrering-feil. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="17302-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="17302-119">Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for en liste over vanlige feil som hindrer registrering og løsninger for hver.</span><span class="sxs-lookup"><span data-stu-id="17302-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="17302-120">[Lær hvordan du kan registrere Android-enheter i Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="17302-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

