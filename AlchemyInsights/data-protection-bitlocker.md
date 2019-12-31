---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908718"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="917cc-102">Aktivere BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="917cc-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="917cc-103">Policyen for sluttpunktbeskyttelse for Intune kan brukes til å konfigurere BitLocker-krypteringsinnstillinger for Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="917cc-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="917cc-104">Hvis du vil ha mer informasjon, kan [du se Windows 10 (og senere) innstillinger for å beskytte enheter ved hjelp av Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="917cc-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="917cc-105">Du bør være oppmerksom på at mange nyere enheter som kjører Windows 10 støtter automatisk BitLocker-kryptering, som utløses uten bruk av MDM-policy.</span><span class="sxs-lookup"><span data-stu-id="917cc-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="917cc-106">Dette kan påvirke bruken av policy hvis ikke-standardinnstillinger er konfigurert.</span><span class="sxs-lookup"><span data-stu-id="917cc-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="917cc-107">Se følgende vanlige spørsmål for flere detaljer.</span><span class="sxs-lookup"><span data-stu-id="917cc-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="917cc-108">Hvis du vil ha informasjon om feilsøking av BitLocker-problemer, kan du se [Feilsøke BitLocker policyer i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="917cc-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="917cc-109">**Vanlige spørsmål**</span><span class="sxs-lookup"><span data-stu-id="917cc-109">**FAQ**</span></span>

 <span data-ttu-id="917cc-110">Spørsmål: hvilke versjoner av Windows støtter Enhetskryptering ved å bruke policyen for sluttpunktbeskyttelse?</span><span class="sxs-lookup"><span data-stu-id="917cc-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="917cc-111">A: innstillingene i Intune Endpoint Protection policy implementeres ved hjelp av [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="917cc-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="917cc-112">Ikke alle utgaver eller versjoner av Windows støtter BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="917cc-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="917cc-113">På dette tidspunktet støttes følgende Windows-utgaver: Enterprise, Education, Mobile, mobile Enterprise og Professional (Build 1809 og senere).</span><span class="sxs-lookup"><span data-stu-id="917cc-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="917cc-114">Q: Hvis en enhet er allerede kryptert med BitLocker bruker OS standardinnstillingene for krypteringsmetode og Cipher styrke (XTS-AES-128), vil bruke en policy med ulike innstillinger automatisk utløse re-kryptering av stasjonen med de nye innstillingene?</span><span class="sxs-lookup"><span data-stu-id="917cc-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="917cc-115">A: Nei.</span><span class="sxs-lookup"><span data-stu-id="917cc-115">A: No.</span></span> <span data-ttu-id="917cc-116">Hvis du vil bruke de nye Cipher innstillingene, må stasjonen først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="917cc-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="917cc-117">**Merk:** For enheter som registreres med autopilot, utløses ikke den automatiske krypteringen som oppstår under OOBE, før Intune-policyen evalueres, noe som gjør at policy-baserte-innstillingene kan brukes i stedet for operativsystem standardene.</span><span class="sxs-lookup"><span data-stu-id="917cc-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="917cc-118">Spørsmål: Hvis en enhet er kryptert som et resultat av bruken av Intune-policy, vil den bli dekryptert når denne policyen fjernes?</span><span class="sxs-lookup"><span data-stu-id="917cc-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="917cc-119">A: fjerning av krypterings relatert policy fører ikke til dekryptering av stasjonene som ble konfigurert.</span><span class="sxs-lookup"><span data-stu-id="917cc-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="917cc-120">Spørsmål: Hvorfor viser Samsvars policyen for Intune at enheten ikke har BitLocker aktivert, selv om den er det?</span><span class="sxs-lookup"><span data-stu-id="917cc-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="917cc-121">A: "BitLocker aktivert"-innstillingen i retningslinjene for overholdelse av Intune bruker Windows Device Health-klienten (DHA).</span><span class="sxs-lookup"><span data-stu-id="917cc-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="917cc-122">Denne klienten måler bare Enhetsstatus ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="917cc-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="917cc-123">Så hvis en enhet ikke er startet på nytt siden BitLocker-krypteringen ble fullført, vil ikke DHA-klienttjenesten rapportere BitLocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="917cc-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 