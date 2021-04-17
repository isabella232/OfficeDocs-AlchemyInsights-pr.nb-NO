---
title: Bitlocker-gjenopprettingsnøkler
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820295"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="d2f7d-102">Få tilgang til Bitlocker-gjenopprettingsnøkler</span><span class="sxs-lookup"><span data-stu-id="d2f7d-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="d2f7d-103">Når du konfigurerer Bitlocker-innstillinger Intune Endpoint Protection Policy, er det mulig å definere om Bitlocker-gjenopprettingsinformasjon skal lagres i Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d2f7d-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="d2f7d-104">Hvis denne innstillingen er konfigurert, skal de lagrede gjenopprettingsdataene være synlige for en Intune-administrator som en del av datainnspillingen for enheten i Intune Devices-bladet på to måter:</span><span class="sxs-lookup"><span data-stu-id="d2f7d-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="d2f7d-105">Enheter – Azure AD-enheter – > «Enhet» ELLER Enheter – > Alle enheter – > «Enhet» -> Gjenopprettingsnøkler</span><span class="sxs-lookup"><span data-stu-id="d2f7d-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="d2f7d-106">Hvis det er administrativ tilgang til selve enheten, kan du eventuelt se gjenopprettingsnøkkelen (Passord) ved å kjøre følgende kommando fra en hevet ledetekst:</span><span class="sxs-lookup"><span data-stu-id="d2f7d-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="d2f7d-107">Hvis enheten ble kryptert før registreringen i Intune, kan gjenopprettingsnøkkelen ha blitt knyttet til Microsoft-kontoen (MSA) som ble brukt til å logge på enheten under OOBE-prosessen.</span><span class="sxs-lookup"><span data-stu-id="d2f7d-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="d2f7d-108">Hvis dette var tilfellet, skal tilgang til og pålogging med MSA vise enhetene som  https://onedrive.live.com/recoverykey gjenopprettingsnøklene ble lagret for.</span><span class="sxs-lookup"><span data-stu-id="d2f7d-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="d2f7d-109">Hvis enheten ble kryptert som et resultat av konfigurasjonen via domenebasert gruppepolicy, kan gjenopprettingsinformasjonen lagres i den lokale Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d2f7d-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="d2f7d-110">Hvis du har konfigurert policyen for endepunktbeskyttelse til å lagre gjenopprettingsnøkkelen i Azure Active Directory, men nøkkelen for en bestemt enhet ikke er lastet opp, kan du utløse opplastingen ved å rotere gjenopprettingsnøkkelen for denne enheten fra MEM-konsollen.</span><span class="sxs-lookup"><span data-stu-id="d2f7d-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="d2f7d-111">Hvis du vil ha mer informasjon, kan du se [Roter BitLocker-gjenopprettingsnøkler](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="d2f7d-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

