---
title: Feilsøke enkel pålogging for Azure AD-sammenføyde enheter
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036175"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="32c87-102">Feilsøke enkel pålogging for Azure AD-sammenføyde enheter</span><span class="sxs-lookup"><span data-stu-id="32c87-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="32c87-103">Hvis du har et lokalt Active Directory-miljø (AD)-miljø og vil bli med i AD-domeneaktiverte datamaskiner til Azure AD, kan du oppnå dette ved å gjøre hybrid Azure AD-sammenføyning.</span><span class="sxs-lookup"><span data-stu-id="32c87-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="32c87-104">[Slik gjør du det: Planlegg implementeringen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) av hybrid Azure Active Directory-sammenføyning gir deg de relaterte trinnene for å implementere en hybrid Azure AD-sammenføyning i miljøet.</span><span class="sxs-lookup"><span data-stu-id="32c87-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="32c87-105">Hvis du vil ha mer informasjon, kan du [se Konfigurere Azure AD-sammenføyde](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)enheter for lokale Single-Sign På ved hjelp av Windows Hello for Business.</span><span class="sxs-lookup"><span data-stu-id="32c87-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="32c87-106">**Problemer med primær oppdateringstoken (PRT)**</span><span class="sxs-lookup"><span data-stu-id="32c87-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="32c87-107">Et primært oppdateringstoken (PRT) er en viktig artefakt av Azure AD-godkjenning på Windows 10-, Windows Server 2016- og nyere versjoner, iOS- og Android-enheter.</span><span class="sxs-lookup"><span data-stu-id="32c87-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="32c87-108">Det er et JSON Web Token (JWT) spesielt utstedt til Microsofts førsteparts tokenmeglere for å aktivere enkel pålogging (SSO) på tvers av programmene som brukes på disse enhetene.</span><span class="sxs-lookup"><span data-stu-id="32c87-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="32c87-109">Hvis du vil ha mer informasjon om hvordan en PRT utstedes, brukes og beskyttes på Windows 10-enheter, kan du se Hva er et [primært oppdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="32c87-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="32c87-110">**WamDefaultSet: JA og AzureADPrt: JA**</span><span class="sxs-lookup"><span data-stu-id="32c87-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="32c87-111">Disse feltene angir om brukeren har godkjent Azure AD ved pålogging på enheten.</span><span class="sxs-lookup"><span data-stu-id="32c87-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="32c87-112">Hvis verdiene er **NEI,** kan det skyldes følgende:</span><span class="sxs-lookup"><span data-stu-id="32c87-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="32c87-113">Ugyldig lagringsnøkkel i TPM som er knyttet til enheten ved registrering (kontroller KeySignTest mens den kjører forhøyet)</span><span class="sxs-lookup"><span data-stu-id="32c87-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="32c87-114">Alternativ påloggings-ID</span><span class="sxs-lookup"><span data-stu-id="32c87-114">Alternate Login ID</span></span>
- <span data-ttu-id="32c87-115">Finner ikke HTTP-proxy</span><span class="sxs-lookup"><span data-stu-id="32c87-115">HTTP Proxy not found</span></span>

<span data-ttu-id="32c87-116">Hvis du vil feilsøke enheter ved hjelp av dsregcmd-kommandoen, kan du [se SSO-tilstand](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="32c87-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
