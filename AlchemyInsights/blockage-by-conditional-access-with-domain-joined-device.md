---
title: Jeg blir blokkert av betinget tilgang med domene sammenføyd enhet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036703"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="7be5d-102">Jeg blir blokkert av betinget tilgang med domene sammenføyd enhet</span><span class="sxs-lookup"><span data-stu-id="7be5d-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="7be5d-103">**Anbefalte verktøy**</span><span class="sxs-lookup"><span data-stu-id="7be5d-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="7be5d-104">[Feilsøkingsverktøy for enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – verktøyet som hjelper deg med å feilsøke de vanligste registreringsproblemene for enheten.</span><span class="sxs-lookup"><span data-stu-id="7be5d-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="7be5d-105">[Test skript for tilkobling til enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Skriptet som bidrar til å sikre at en enhet får tilgang til endepunktene for enhetsregistrering under systemkontoen.</span><span class="sxs-lookup"><span data-stu-id="7be5d-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="7be5d-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – Skriptet som lar deg søke etter og administrere foreldede enheter i miljøet.</span><span class="sxs-lookup"><span data-stu-id="7be5d-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="7be5d-107">Her er noen vanlige årsaker til at betinget tilgang kan mislykkes på en enhet som har blitt med i et domene (Hybrid Azure AD).</span><span class="sxs-lookup"><span data-stu-id="7be5d-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="7be5d-108">**Det er ingen Azure AD PRT** på enheten – Du må sikre at enheten har Azure AD Primary Refresh Token (PRT).</span><span class="sxs-lookup"><span data-stu-id="7be5d-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="7be5d-109">Hvis du vil ha mer informasjon om PRT, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="7be5d-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="7be5d-110">Hvis du vil bekrefte om du har Azure AD PRT, kan du kjøre kommandoen på enheten og kontrollere om `dsregcmd/status` «AzureAdPrt» er lik JA.</span><span class="sxs-lookup"><span data-stu-id="7be5d-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="7be5d-111">Hvis «AzureAdPrt» er «NEI», kontrollerer du følgende:</span><span class="sxs-lookup"><span data-stu-id="7be5d-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="7be5d-112">Enten du har et forbundsmiljø med **AD FS,** og det ikke kan nås fra brukernes hjemmenettverk: I dette tilfellet må du sørge for at endepunktene «brukernavnmikset» er tilgjengelige fra ekstranettet.</span><span class="sxs-lookup"><span data-stu-id="7be5d-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="7be5d-113">Hvis AD FS er bak et VPN, må du sørge for at brukerne kobler seg til VPN og logger på enheten på nytt.</span><span class="sxs-lookup"><span data-stu-id="7be5d-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="7be5d-114">Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="7be5d-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="7be5d-115">**Om enhetens TPM** er feil og dermed ikke kan godkjenne enheten: Kontroller «tpm.msc» for å se om tilstanden til TPM er klar.</span><span class="sxs-lookup"><span data-stu-id="7be5d-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="7be5d-116">Hvis ikke, kan `dsregcmd/leave` du kjøre og la enheten bli med i Azure AD på nytt.</span><span class="sxs-lookup"><span data-stu-id="7be5d-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="7be5d-117">Prøv deretter på nytt.</span><span class="sxs-lookup"><span data-stu-id="7be5d-117">Then, try again.</span></span> <span data-ttu-id="7be5d-118">Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="7be5d-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="7be5d-119">**Du bruker en tredjeparts identitetsleverandør, som ikke støtter** WS-Trust protokoll .</span><span class="sxs-lookup"><span data-stu-id="7be5d-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="7be5d-120">Som beskrevet i våre dokumenter, kan ikke hybrid Azure AD-sammenføyde enheter fungere i dette tilfellet.</span><span class="sxs-lookup"><span data-stu-id="7be5d-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="7be5d-121">Samarbeid med identitetsleverandøren din for å få støtte.</span><span class="sxs-lookup"><span data-stu-id="7be5d-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="7be5d-122">Brukere bruker Chrome-nettleseren uten **Windows 10-kontoer** eller Office-utvidelse Chrome bruker ikke automatisk PRT på AAD-sammenføyde eller **hybrid-AAD-sammenføyde** enheter: Dette fører til feil i eventuelle enhetsbaserte policyer for betinget tilgang, med feilmeldingen «Uregistrert enhet» vises.</span><span class="sxs-lookup"><span data-stu-id="7be5d-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="7be5d-123">Hvis du vil bruke Chrome-nettleseren på riktig måte, må du installere Windows 10-kontoer eller Office-utvidelsen til brukernes Chrome-nettleser via SCCM eller Intune.</span><span class="sxs-lookup"><span data-stu-id="7be5d-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="7be5d-124">Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="7be5d-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="7be5d-125">Hvis det ikke er mulig å skyve utvidelsen eksternt, må du varsle brukerne om å installere en av utvidelsene ovenfor manuelt for å få tilgang til programmer bak enhetsbasert betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="7be5d-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="7be5d-126">Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="7be5d-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="7be5d-127">Enheten ble koblet til riktig hybrid Azure AD, men det ble utilsiktet slettet eller deaktivert, enten på grunn av synkroniseringsendringer i Azure AD Connect eller fra **Azure-portalen:** Hvis dette skjer, gjenkjennes ikke enhetsobjektet lenger som en fullstendig sammenføyd enhet, selv om statusen «AzureAdJoined» og «PRT» vises som gyldig på enheten.</span><span class="sxs-lookup"><span data-stu-id="7be5d-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="7be5d-128">Du kan løse dette problemet ved å `dsregcmd/leave` kjøre på de berørte enhetene og la dem bli med i Azure AD på nytt.</span><span class="sxs-lookup"><span data-stu-id="7be5d-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="7be5d-129">Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="7be5d-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="7be5d-130">Hvis enhetene er på Windows 10, 1809-oppdateringen, med VPN/Skyproxy og ser problemer med AzureAdPrt-tilstanden eller en app med SSO-problem (outlook kobler ikke til postboksen selv om du hadde PRT), må du kontrollere at du har denne oppdateringen [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) eller april kumulativ oppdatering [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) for å forhindre PRT-feil på disse maskinene.</span><span class="sxs-lookup"><span data-stu-id="7be5d-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















