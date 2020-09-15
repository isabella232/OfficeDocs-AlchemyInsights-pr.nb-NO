---
title: Feilsøke problemer med å registrere Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658887"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="ddad6-102">Feilsøke problemer med å registrere Windows-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="ddad6-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="ddad6-103">Se gjennom ressursene som er oppført nedenfor, for å løse problemet nå.</span><span class="sxs-lookup"><span data-stu-id="ddad6-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="ddad6-104">Noen vanlige feil meldinger og løsnings trinn:</span><span class="sxs-lookup"><span data-stu-id="ddad6-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="ddad6-105">**Program varen kan ikke installeres, 0x80cf4017:** Konto sertifikatet er utløpt.</span><span class="sxs-lookup"><span data-stu-id="ddad6-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="ddad6-106">Last ned program vare pakken for PC-klienten i administrasjons konsollen for Intune på nytt.</span><span class="sxs-lookup"><span data-stu-id="ddad6-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="ddad6-107">Se gjennom denne dokumentasjonen for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="ddad6-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="ddad6-108">**Feilkode 0x801c0003:** Feilen kan oppstå i følgende scenarioer:</span><span class="sxs-lookup"><span data-stu-id="ddad6-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="ddad6-109">Brukeren har flere enheter som ble registrert enn enhets grensen.</span><span class="sxs-lookup"><span data-stu-id="ddad6-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="ddad6-110">Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) eller [endre enhets grensen](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="ddad6-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="ddad6-111">«Brukere kan bli med i enheter til Azure AD» er satt til ingen.</span><span class="sxs-lookup"><span data-stu-id="ddad6-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="ddad6-112">Angi det til alle eller Velg brukere.</span><span class="sxs-lookup"><span data-stu-id="ddad6-112">Set it to all or select users.</span></span> <span data-ttu-id="ddad6-113">Se gjennom [denne dokumentasjonen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="ddad6-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="ddad6-114">Enheten er allerede registrert av en annen bruker.</span><span class="sxs-lookup"><span data-stu-id="ddad6-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="ddad6-115">Hvis det er tilfelle, fjerner du enheten fra Azure Intune-konsollen eller avregistrerer enheten manuelt før du prøver på nytt.</span><span class="sxs-lookup"><span data-stu-id="ddad6-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="ddad6-116">Enheten er Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="ddad6-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="ddad6-117">Bare Windows 10 Pro, Education og Enterprise SKU-er kan bli med i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ddad6-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="ddad6-118">Flere ressurser som kan hjelpe deg med å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="ddad6-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="ddad6-119">Bruk [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrerings feil.</span><span class="sxs-lookup"><span data-stu-id="ddad6-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="ddad6-120">Se gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="ddad6-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="ddad6-121">Se gjennom disse dokumentene for en liste over vanlige feil som forhindrer registrering og løsninger på hver av dem: [feil søkings veiledning](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [feil søkings dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="ddad6-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="ddad6-122">[Lær hvordan du registrerer Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="ddad6-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
