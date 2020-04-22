---
title: Vilkår som mangler fra SharePoint Online Term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766862"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="3a4c0-102">Aktivere Bitlocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="3a4c0-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="3a4c0-103">Intune Endpoint Protection Policy kan brukes til å konfigurere Boitlocker krypteringsinnstillinger for Windows-enheter som beskrevet i : Windows10 (og senere) innstillinger for å beskytte enheter som bruker Intune</span><span class="sxs-lookup"><span data-stu-id="3a4c0-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="3a4c0-104">Du bør være oppmerksom på at mange nyere enheter som kjører Windows 10, støtter automatisk bitlocker-kryptering som utløses uten bruk av MDM-policy.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="3a4c0-105">Dette kan påvirke programmet for policy hvis ikke-standardinnstillinger er konfigurert.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="3a4c0-106">Se Vanlige spørsmål for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-106">See FAQ for more detail.</span></span>


<span data-ttu-id="3a4c0-107">Vanlige  spørsmål: Hvilke versjoner av Windows støtter enhetskryptering ved hjelp av policyen for beskyttelse av endepunkt?</span><span class="sxs-lookup"><span data-stu-id="3a4c0-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="3a4c0-108"> Svar: Innstillingene i Intune Endpoint Protection Policy implementeres ved hjelp av Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="3a4c0-109">Ikke alle utgaver eller versjoner av Windows støtter Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="3a4c0-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="3a4c0-110">På dette tidspunktet Windows Editions: Enterprise; Utdanning, Mobil, Mobil bedrift og Professional (fra bygge 1809 og utover) støttes.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="3a4c0-111">Spørsmål: Hvis en enhet allerede er kryptert med Bitlocker ved hjelp av OS-standardinnstillingene for krypteringsmetode og chifferstyrke (XTS-AES-128), vil bruk av en policy med forskjellige innstillinger automatisk utløse rekryptering av stasjonen med de nye innstillingene?</span><span class="sxs-lookup"><span data-stu-id="3a4c0-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="3a4c0-112">A: Nei.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-112">A: No.</span></span> <span data-ttu-id="3a4c0-113">For å kunne bruke de nye chifferinnstillingene må stasjonen først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="3a4c0-114">For enheter som registreres med Autopilot, utløses ikke den automatiske krypteringen som oppstår under OOBE før Intune-policyen evalueres, noe som gjør at policybaserte innstillinger kan brukes i stedet for OS-standardene</span><span class="sxs-lookup"><span data-stu-id="3a4c0-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="3a4c0-115">Q Hvis en enhet er kryptert som følge av anvendelsen av Intune-policyen, dekrypteres den når denne policyen fjernes?</span><span class="sxs-lookup"><span data-stu-id="3a4c0-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="3a4c0-116">A: Fjerning av krypteringsrelatert policy resulterer IKKE i dekryptering av stasjonene som ble konfigurert.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="3a4c0-117">Spørsmål: Hvorfor viser intune Compliance policy at enheten min ikke har "Bitlocker Aktivert", men det er det?</span><span class="sxs-lookup"><span data-stu-id="3a4c0-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="3a4c0-118">Svar: Innstillingen "Bitlocker aktivert" i intune compliance policy bruker Windows Device Health Attestation (DHA)-klienten.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="3a4c0-119">Denne klienten måler bare enhetstilstand ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="3a4c0-120">Så hvis en enhet ikke har blitt startet på nytt siden bitlocker kryptering ble fullført DHA-klienttjenesten vil ikke rapportere bitlocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="3a4c0-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>