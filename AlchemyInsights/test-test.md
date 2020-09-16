---
title: Termer mangler i term lageret i SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750460"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="f7af6-102">Aktivere BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="f7af6-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="f7af6-103">Policyen for Intune Endpoint Protection kan brukes til å konfigurere Boitlocker krypterings innstillinger for Windows-enheter som beskrevet i: Windows10 (og nyere) innstillinger for å beskytte enheter ved hjelp av Intune</span><span class="sxs-lookup"><span data-stu-id="f7af6-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="f7af6-104">Du bør være klar over at mange nyere enheter som kjører Windows 10 støtter automatisk BitLocker-kryptering som utløses uten program for MDM-policy.</span><span class="sxs-lookup"><span data-stu-id="f7af6-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="f7af6-105">Dette kan påvirke bruk av policy hvis det ikke er konfigurerte standard innstillinger.</span><span class="sxs-lookup"><span data-stu-id="f7af6-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="f7af6-106">Se vanlige spørsmål for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="f7af6-106">See FAQ for more detail.</span></span>


<span data-ttu-id="f7af6-107">Vanlige spørsmål   : hvilke utgaver av Windows støtter enhets kryptering ved hjelp av policyen for ende punkt beskyttelse?</span><span class="sxs-lookup"><span data-stu-id="f7af6-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="f7af6-108"> Svar: innstillingene i policyer for Intune Endpoint Protection implementeres ved hjelp av BitLocker-CSPEN.</span><span class="sxs-lookup"><span data-stu-id="f7af6-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="f7af6-109">Ikke alle utgaver eller versjoner av Windows støtter BitLocker-CSPEN. 
     </span><span class="sxs-lookup"><span data-stu-id="f7af6-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="f7af6-110">På dette tidspunktet Windows-utgaver: Enterprise; Education, mobil, mobil Enterprise og Professional (fra Bygg 1809 fremover) støttes.</span><span class="sxs-lookup"><span data-stu-id="f7af6-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="f7af6-111">Spørsmål: Hvis en enhet allerede er kryptert med BitLocker ved hjelp av standard innstillingene for OS for krypterings metode og chifferkodestyrke (XTS-AES-128), vil bruk av en policy med ulike innstillinger automatisk utløse rekryptering av stasjonen med de nye innstillingene?</span><span class="sxs-lookup"><span data-stu-id="f7af6-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="f7af6-112">Sv.: Nei.</span><span class="sxs-lookup"><span data-stu-id="f7af6-112">A: No.</span></span> <span data-ttu-id="f7af6-113">Hvis du vil bruke de nye Cipher innstillingene, må stasjonen først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="f7af6-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="f7af6-114">Obs! for enheter som blir registrert med automatisk pilot, blir ikke den automatiske krypteringen som ville skje under OOBE, utløst før Intune-policyen blir evaluert, noe som gjør at policy innstillingene kan brukes i stedet for operativ system standardene</span><span class="sxs-lookup"><span data-stu-id="f7af6-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="f7af6-115">Hvis en enhet krypteres som et resultat av appen for Intune-policyen, dekrypteres den når policyen fjernes?</span><span class="sxs-lookup"><span data-stu-id="f7af6-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="f7af6-116">Svar: fjerning av krypterings relatert policy fører ikke til dekryptering av stasjonene som ble konfigurert.</span><span class="sxs-lookup"><span data-stu-id="f7af6-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="f7af6-117">Spørsmål: Hvorfor viser Samsvars policyen for Intune at enheten ikke har BitLocker aktivert, men det er?</span><span class="sxs-lookup"><span data-stu-id="f7af6-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="f7af6-118">A: innstillingen «BitLocker aktivert» i henhold til samsvars policyen for Intune bruker Windows Device Health Attestation-klienten (DHA).</span><span class="sxs-lookup"><span data-stu-id="f7af6-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="f7af6-119">Denne klienten måler bare enhets tilstanden ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="f7af6-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="f7af6-120">Hvis en enhet ikke har blitt startet på nytt etter at BitLocker-kryptering ble fullført, vil ikke tjeneste tjenesten for DHA rapportere at BitLocker skal være aktiv.</span><span class="sxs-lookup"><span data-stu-id="f7af6-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>