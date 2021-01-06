---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768826"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="51bb4-102">Aktivere BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="51bb4-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="51bb4-103">Policyen for Intune Endpoint Protection kan brukes til å konfigurere BitLocker-krypteringsnøkkel for Windows-enheter.</span><span class="sxs-lookup"><span data-stu-id="51bb4-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="51bb4-104">Hvis du vil ha mer informasjon, kan du se [Innstillinger for Windows 10 (og nyere) for å beskytte enheter ved hjelp av Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="51bb4-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="51bb4-105">Du bør være klar over at mange nyere enheter som kjører Windows 10 støtter automatisk BitLocker-kryptering, som utløses uten program for MDM-policy.</span><span class="sxs-lookup"><span data-stu-id="51bb4-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="51bb4-106">Dette kan påvirke bruk av policy hvis ikke-standard innstillinger er konfigurert.</span><span class="sxs-lookup"><span data-stu-id="51bb4-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="51bb4-107">Se følgende vanlige spørsmål for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="51bb4-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="51bb4-108">Hvis du vil ha informasjon om å feilsøke BitLocker-problemer, kan du se [Feilsøke BitLocker-policyer i Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="51bb4-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="51bb4-109">**SPØRSMÅL OG SVAR**</span><span class="sxs-lookup"><span data-stu-id="51bb4-109">**FAQ**</span></span>

<span data-ttu-id="51bb4-110">Spørsmål: hvilke utgaver av Windows støtter enhets kryptering ved hjelp av policyen for ende punkt beskyttelse?</span><span class="sxs-lookup"><span data-stu-id="51bb4-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="51bb4-111">Svar: innstillingene i policyer for Intune Endpoint Protection implementeres ved hjelp av [BitLocker-CSPen](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="51bb4-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="51bb4-112">Ikke alle utgaver eller versjoner av Windows støtter BitLocker-CSPEN.</span><span class="sxs-lookup"><span data-stu-id="51bb4-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="51bb4-113">Spørsmål: Hvordan kan BitLocker aktiveres på enheter uten å kreve slutt bruker medvirkning?</span><span class="sxs-lookup"><span data-stu-id="51bb4-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="51bb4-114">A: så lenge de nødvendige forhånds kravene er oppfylt, er det mulig å aktivere BitLocker "stille kryptering" gjennom Intune.</span><span class="sxs-lookup"><span data-stu-id="51bb4-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="51bb4-115">Se detaljene om enhetens krav og eksempler på policy innstillinger for å aktivere stille kryptering i følgende dokument: [aktivere BitLocker-kryptering stille](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="51bb4-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="51bb4-116">Spørsmål: Hvis en enhet allerede er kryptert med BitLocker ved hjelp av standard innstillingene for krypterings metode og chifferkodestyrke (XTS-AES-128), vil bruk av en policy med ulike innstillinger automatisk utløse rekryptering av stasjonen med de nye innstillingene?</span><span class="sxs-lookup"><span data-stu-id="51bb4-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="51bb4-117">Sv.: Nei.</span><span class="sxs-lookup"><span data-stu-id="51bb4-117">A: No.</span></span> <span data-ttu-id="51bb4-118">Hvis du vil bruke de nye Cipher innstillingene, må stasjonen først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="51bb4-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="51bb4-119">**Obs!** For enheter som blir registrert med automatisk pilot, utløses ikke krypteringen som ville oppstå under OOBE, før Intune-policyen evalueres, slik at de policy-baserte innstillingene kan brukes i stedet for OS-standardene.</span><span class="sxs-lookup"><span data-stu-id="51bb4-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="51bb4-120">Spørsmål: Hvis en enhet krypteres som et resultat av appen for Intune-policyen, dekrypteres den når policyen fjernes?</span><span class="sxs-lookup"><span data-stu-id="51bb4-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="51bb4-121">Svar: fjerning av krypterings relatert policy fører ikke til dekryptering av stasjonene som ble konfigurert.</span><span class="sxs-lookup"><span data-stu-id="51bb4-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="51bb4-122">Spørsmål: Hvorfor viser Samsvars policyen for Intune at enheten ikke har BitLocker aktivert, selv om den er?</span><span class="sxs-lookup"><span data-stu-id="51bb4-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="51bb4-123">A: innstillingen BitLocker Enabled i Intune-overholdelses policyen bruker Windows-klienten tilstands attestering (DHA).</span><span class="sxs-lookup"><span data-stu-id="51bb4-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="51bb4-124">Denne klienten måler bare enhets tilstanden ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="51bb4-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="51bb4-125">Hvis en enhet ikke har blitt startet på nytt etter at BitLocker-kryptering ble fullført, vil ikke tjeneste tjenesten DHA rapportere at BitLocker blir aktivert.</span><span class="sxs-lookup"><span data-stu-id="51bb4-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 