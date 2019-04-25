---
title: Feilsøke problemer med registrering av Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390652"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="0ccd8-102">Feilsøke problemer med registrering av Windows-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0ccd8-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="0ccd8-103">Se gjennom ressursene som vises nedenfor for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="0ccd8-104">Noen vanlige feilmeldinger og Løsningstrinn:</span><span class="sxs-lookup"><span data-stu-id="0ccd8-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="0ccd8-105">**Kan ikke installere programvaren, 0x80cf4017:** Konto-sertifikatet er utløpt.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="0ccd8-106">Nytt Last ned PC-klient programvaren i Intune Admin-konsollen.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="0ccd8-107">Se dokumentasjonen for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-107">Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="0ccd8-108">**0x801c0003-feilkode:** Feilen kan oppstå i følgende scenarier:</span><span class="sxs-lookup"><span data-stu-id="0ccd8-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="0ccd8-109">Brukeren har flere enheter som er registrert enn enhetsgrensen.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0ccd8-110">Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) , eller [Endre begrensningen for enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="0ccd8-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="0ccd8-111">"Brukere kan koble enheter til Azure AD" er satt til "ingen".</span><span class="sxs-lookup"><span data-stu-id="0ccd8-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="0ccd8-112">Sett den til alle, eller Velg brukere.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-112">Set it to all or select users.</span></span> <span data-ttu-id="0ccd8-113">Gå gjennom [denne dokumentasjonen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="0ccd8-114">Enheten er allerede registrert av en annen bruker.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="0ccd8-115">Hvis det er tilfellet, fjerner du enheten fra konsollen Azure Intune eller unenroll enheten manuelt før du prøver på nytt.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="0ccd8-116">Enheten er Windows Home 10.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="0ccd8-117">Bare Windows 10 Pro, utdanning og Enterprise SKUer kan delta Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="0ccd8-118">Ytterligere ressurser til å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="0ccd8-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0ccd8-119">Bruke [Intune feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrering-feil.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0ccd8-120">Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="0ccd8-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="0ccd8-121">Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og løsninger for hver: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [feilsøking dok](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="0ccd8-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="0ccd8-122">[Lær hvordan du kan registrere Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="0ccd8-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

