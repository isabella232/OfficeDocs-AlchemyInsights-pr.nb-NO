---
title: Single-Sign på for Azure Active Directory-sammenføyde enheter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405051"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="ac961-102">Enkel pålogging for Azure Active Directory-sammenføyde enheter</span><span class="sxs-lookup"><span data-stu-id="ac961-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="ac961-103">Hvis du har et lokalt Active Directory-miljø (AD)-miljø og vil bli med i AD-domeneaktiverte datamaskiner til Azure AD, kan du oppnå dette ved å gjøre hybrid Azure AD-sammenføyning.</span><span class="sxs-lookup"><span data-stu-id="ac961-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="ac961-104">[Slik gjør du det: Planlegg implementeringen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) av hybrid Azure Active Directory-sammenføyning gir deg de relaterte trinnene for å implementere en hybrid Azure AD-sammenføyning i miljøet.</span><span class="sxs-lookup"><span data-stu-id="ac961-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="ac961-105">Konfigurere Azure AD-sammenføyde enheter for lokale Single-Sign På ved hjelp av Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="ac961-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="ac961-106">**Problemer med primær oppdateringstoken (PRT)** Et primært oppdateringstoken (PRT) er en viktig artefakt av Azure AD-godkjenning på Windows 10-, Windows Server 2016- og nyere versjoner, iOS- og Android-enheter.</span><span class="sxs-lookup"><span data-stu-id="ac961-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="ac961-107">Det er et JSON Web Token (JWT) spesielt utstedt til Microsofts førsteparts tokenmeglere for å aktivere enkel pålogging (SSO) på tvers av programmene som brukes på disse enhetene.</span><span class="sxs-lookup"><span data-stu-id="ac961-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="ac961-108">[I Hva er et primært oppdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)gir vi detaljer om hvordan en PRT utstedes, brukes og beskyttes på Windows 10-enheter.</span><span class="sxs-lookup"><span data-stu-id="ac961-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="ac961-109">**WamDefaultSet: JA og AzureADPrt: JA** Disse feltene angir om brukeren har godkjent Azure AD ved pålogging på enheten.</span><span class="sxs-lookup"><span data-stu-id="ac961-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="ac961-110">Hvis verdiene er **NEI,** kan det forfalle:</span><span class="sxs-lookup"><span data-stu-id="ac961-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="ac961-111">Ugyldig lagringsnøkkel i TPM som er knyttet til enheten ved registrering (kontroller KeySignTest mens den kjører forhøyet).</span><span class="sxs-lookup"><span data-stu-id="ac961-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="ac961-112">Alternativ påloggings-ID</span><span class="sxs-lookup"><span data-stu-id="ac961-112">Alternate Login ID</span></span>
- <span data-ttu-id="ac961-113">Finner ikke HTTP-proxy</span><span class="sxs-lookup"><span data-stu-id="ac961-113">HTTP Proxy not found</span></span>

<span data-ttu-id="ac961-114">Feilsøke enheter ved hjelp av kommandoen dsregcmd – [SSO-tilstand](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="ac961-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
