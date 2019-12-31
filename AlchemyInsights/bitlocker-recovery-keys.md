---
title: Gjenopprettingsnøkler for BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908823"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="088e9-102">Tilgang til gjenopprettingsnøkler for BitLocker</span><span class="sxs-lookup"><span data-stu-id="088e9-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="088e9-103">Når du konfigurerer BitLocker-innstillinger Intune Endpoint Protection policy, er det mulig å definere om gjenopprettingsinformasjon for BitLocker skal lagres i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="088e9-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="088e9-104">Hvis denne innstillingen er konfigurert, skal de lagrede Gjenopprettingsdataene være synlige for en Intune-administrator som en del av enhets oppførings dataene i Intune Devices-blad på to måter:</span><span class="sxs-lookup"><span data-stu-id="088e9-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="088e9-105">Enheter-Azure AD-enheter-> "enhet" eller enheter-> alle enheter-> "enhet"-> gjenopprettings taster</span><span class="sxs-lookup"><span data-stu-id="088e9-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="088e9-106">Hvis det er administrativ tilgang til selve enheten, kan du eventuelt se gjenopprettingsnøkkelen (Password) ved å kjøre følgende kommando fra en hevet ledetekst:</span><span class="sxs-lookup"><span data-stu-id="088e9-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="088e9-107">Hvis enheten ble kryptert før registrering i Intune, kan gjenopprettingsnøkkelen være knyttet til "Microsoft Account" (MSA) som brukes til å logge på enheten under OOBE-prosessen.</span><span class="sxs-lookup"><span data-stu-id="088e9-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="088e9-108">Hvis det var tilfelle, tilgang https://onedrive.live.com/recoverykey til og logge på med at MSA skal vise enhetene som gjenopprettingsnøkler ble lagret.</span><span class="sxs-lookup"><span data-stu-id="088e9-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="088e9-109">Hvis enheten ble kryptert som et resultat av konfigurasjon gjennom domenebasert gruppepolicy, kan gjenopprettingsinformasjonen lagres i den lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="088e9-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

