---
title: Vilkår mangler fra SharePoint Online term store
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762077"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="df186-102">Aktivere BitLocker-kryptering med Intune</span><span class="sxs-lookup"><span data-stu-id="df186-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="df186-103">Policyen for beskyttelse mot endepunkter for Intune kan brukes til å konfigurere Boitlocker krypteringsinnstillinger for Windows-enheter som beskrevet i: Windows10 (og senere) innstillinger for å beskytte enheter ved hjelp av Intune</span><span class="sxs-lookup"><span data-stu-id="df186-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="df186-104">Du bør være oppmerksom på at mange nyere enheter som kjører Windows 10 støtter automatisk BitLocker-kryptering som utløses uten bruk av MDM-policy.</span><span class="sxs-lookup"><span data-stu-id="df186-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="df186-105">Dette kan påvirke bruken av policy hvis ikke standardinnstillingene er konfigurert.</span><span class="sxs-lookup"><span data-stu-id="df186-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="df186-106">Se vanlige spørsmål for flere detaljer.</span><span class="sxs-lookup"><span data-stu-id="df186-106">See FAQ for more detail.</span></span>


<span data-ttu-id="df186-107">Vanlige  spørsmål: hvilke versjoner av Windows støtter Enhetskryptering ved å bruke policyen for sluttpunktbeskyttelse?</span><span class="sxs-lookup"><span data-stu-id="df186-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="df186-108"> A: innstillingene i Intune Endpoint Protection policy implementeres ved hjelp av BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="df186-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="df186-109">Ikke alle utgaver eller versjoner av Windows støtter BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="df186-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="df186-110">På dette tidspunktet Windows Editions: Enterprise; Utdanning, Mobile, mobile Enterprise og Professional (fra bygge 1809 og framover) støttes.</span><span class="sxs-lookup"><span data-stu-id="df186-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="df186-111">Q: Hvis en enhet er allerede kryptert med BitLocker bruker OS standardinnstillingene for krypteringsmetode og Cipher styrke (XTS-AES-128) vil bruke en policy med ulike innstillinger automatisk utløse re-kryptering av stasjonen med de nye innstillingene?</span><span class="sxs-lookup"><span data-stu-id="df186-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="df186-112">A: Nei.</span><span class="sxs-lookup"><span data-stu-id="df186-112">A: No.</span></span> <span data-ttu-id="df186-113">For å bruke de nye Cipher innstillingene stasjonen må først dekrypteres.</span><span class="sxs-lookup"><span data-stu-id="df186-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="df186-114">For enheter som blir registrert med autopilot, utløses automatisk kryptering som vil oppstå under OOBE ikke før Intune-policy evalueres som tillater policy-baserte innstillinger som skal brukes i stedet for OS-standarder</span><span class="sxs-lookup"><span data-stu-id="df186-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="df186-115">Q hvis en enhet krypteres som et resultat av bruken av Intune-policyen, blir den dekryptert når denne policyen fjernes?</span><span class="sxs-lookup"><span data-stu-id="df186-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="df186-116">A: fjerning av kryptering relatert policy fører ikke til dekryptering av stasjonene som ble konfigurert.</span><span class="sxs-lookup"><span data-stu-id="df186-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="df186-117">Spørsmål: Hvorfor viser Intune Compliance policy at enheten ikke har "BitLocker Enabled", men det er?</span><span class="sxs-lookup"><span data-stu-id="df186-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="df186-118">A: "BitLocker aktivert"-innstillingen i samsvars policyen for Intune bruker Windows Device Health-klienten (DHA).</span><span class="sxs-lookup"><span data-stu-id="df186-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="df186-119">Denne klienten måler bare Enhetsstatus ved oppstart.</span><span class="sxs-lookup"><span data-stu-id="df186-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="df186-120">Så hvis en enhet ikke har blitt startet på nytt siden BitLocker-krypteringen ble fullført, vil ikke DHA-klienttjenesten rapportere BitLocker som aktiv.</span><span class="sxs-lookup"><span data-stu-id="df186-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>