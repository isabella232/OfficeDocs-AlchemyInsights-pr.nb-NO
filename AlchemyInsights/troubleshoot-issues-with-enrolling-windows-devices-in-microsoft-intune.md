---
title: Feilsøke problemer med registrering av Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661562"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="e40a6-102">Feilsøke problemer med registrering av Windows-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e40a6-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="e40a6-103">Se gjennom ressursene som vises nedenfor for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="e40a6-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e40a6-104">Noen vanlige feilmeldinger og Løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="e40a6-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="e40a6-p101">**Kan ikke installere programvaren, 0x80cf4017:** Konto-sertifikatet er utløpt. Nytt Last ned PC-klient programvaren i Intune Admin-konsollen. Se dokumentasjonen for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="e40a6-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="e40a6-108">**0x801c0003-feilkode:** Feilen kan oppstå i følgende scenarier:</span><span class="sxs-lookup"><span data-stu-id="e40a6-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="e40a6-p102">Brukeren har flere enheter som er registrert enn enhetsgrensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) , eller [Endre begrensningen for enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="e40a6-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="e40a6-p103">"Brukere kan koble enheter til Azure AD" er satt til "ingen". Sett den til alle, eller Velg brukere. Gå gjennom [denne dokumentasjonen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="e40a6-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="e40a6-p104">Enheten er allerede registrert av en annen bruker. Hvis det er tilfellet, fjerner du enheten fra konsollen Azure Intune eller unenroll enheten manuelt før du prøver på nytt.</span><span class="sxs-lookup"><span data-stu-id="e40a6-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="e40a6-p105">Enheten er Windows Home 10. Bare Windows 10 Pro, utdanning og Enterprise SKUer kan delta Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e40a6-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="e40a6-118">Ytterligere ressurser til å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="e40a6-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e40a6-p106">Bruke [Intune feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrering-feil. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="e40a6-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e40a6-121">Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og løsninger for hver: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [feilsøking dok](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e40a6-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="e40a6-122">[Lær hvordan du kan registrere Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="e40a6-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

