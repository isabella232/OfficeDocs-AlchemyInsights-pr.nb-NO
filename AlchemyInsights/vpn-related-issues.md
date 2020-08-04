---
title: VPN-relaterte problemer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555232"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="3c564-102">VPN-relaterte problemer</span><span class="sxs-lookup"><span data-stu-id="3c564-102">VPN related issues</span></span>

<span data-ttu-id="3c564-103">Vellykket implementering av VPN-tilkobling for MDM-klienter avhenger av en distribuert profil som gjenspeiler kravene til VPN-infrastrukturen på riktig måte.</span><span class="sxs-lookup"><span data-stu-id="3c564-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="3c564-104">Hvis du vil ha de riktige innstillingene for klientplattformene du undersøker, kan du se:</span><span class="sxs-lookup"><span data-stu-id="3c564-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="3c564-105">Windows 10 og Windows Holografiske enhetsinnstillinger for å legge til VPN-tilkoblinger ved hjelp av Intune</span><span class="sxs-lookup"><span data-stu-id="3c564-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="3c564-106">Legge til VPN-innstillinger på iOS- og iPadOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3c564-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="3c564-107">Innstillinger for Android-enheter for å konfigurere VPN i Intune</span><span class="sxs-lookup"><span data-stu-id="3c564-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="3c564-108">Legge til VPN-innstillinger på macOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3c564-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="3c564-109">Hvis VPN-profilen din bruker sertifikatbasert godkjenning, må du kontrollere at rotsertifikat- og klientgodkjenningssertifikatprofilene som er koblet til VPN-profilen, distribueres.</span><span class="sxs-lookup"><span data-stu-id="3c564-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="3c564-110">**Vanlige problemer**</span><span class="sxs-lookup"><span data-stu-id="3c564-110">**Common Issues**</span></span>

<span data-ttu-id="3c564-111">**Jeg distribuerte en VPN-profil til en enhet. Intune viser at det var vellykket, men enheten kobler ikke til VPN.**</span><span class="sxs-lookup"><span data-stu-id="3c564-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="3c564-112">En vellykket status betyr at Intune har distribuert profilen som konfigurert.</span><span class="sxs-lookup"><span data-stu-id="3c564-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="3c564-113">Disse konfigurasjonene samsvarer imidlertid kanskje ikke med kravene til nettverket og/eller godkjenningen.</span><span class="sxs-lookup"><span data-stu-id="3c564-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="3c564-114">Se gjennom logger i infrastruktur- og godkjenningstjenesten (på VPN-serveren og NPS/Radius-serveren) hvis du vil ha mer informasjon om den forsøkte tilkoblingen.</span><span class="sxs-lookup"><span data-stu-id="3c564-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="3c564-115">Du må kanskje samarbeide med nettverksinfrastrukturteamet ditt, eller tredjeparts VPN-leverandøren, for å samle inn og gjennomgå logger.</span><span class="sxs-lookup"><span data-stu-id="3c564-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="3c564-116">**Når jeg konfigurerer et egendefinert VPN for iOS, er ikke VPN-funksjonen per app gjort tilgjengelig.**</span><span class="sxs-lookup"><span data-stu-id="3c564-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="3c564-117">VPN per app for iOS-enheter i Intune er for øyeblikket tilgjengelig for en bestemt liste over leverandører og partnere, som også må oppfylle sertifikatforutsetninger før du konfigurerer et VPN per app.</span><span class="sxs-lookup"><span data-stu-id="3c564-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="3c564-118">Hvis du vil ha mer informasjon, kan du se [Konfigurere VPN (Virtual Private Network) per app for iOS/iPadOS-enheter i Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="3c564-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="3c564-119">Hvis du vil ha mer informasjon om alle VPN-tilkoblingstyper i Intune, kan du se [Opprette VPN-profiler for å koble til VPN-servere i Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="3c564-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="3c564-120">**iOS On-Demand VPN utløses ikke når et konfigurert domene er tilgjengelig**</span><span class="sxs-lookup"><span data-stu-id="3c564-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="3c564-121">Hvis du vil teste automatiske VPN-innstillinger, angir du følgende verdier:</span><span class="sxs-lookup"><span data-stu-id="3c564-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="3c564-122">Jeg vil gjøre følgende: **Evaluere hvert tilkoblingsforsøk**</span><span class="sxs-lookup"><span data-stu-id="3c564-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="3c564-123">Velg om du vil koble til: **Koble til om nødvendig**</span><span class="sxs-lookup"><span data-stu-id="3c564-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="3c564-124">Når brukere får tilgang til disse domenene: **mål** *domenenavn*</span><span class="sxs-lookup"><span data-stu-id="3c564-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="3c564-125">Hvis konfigurasjonen ovenfor ikke er vellykket, legger du til følgende element:</span><span class="sxs-lookup"><span data-stu-id="3c564-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="3c564-126">Når denne URL-adressen ikke kan nås, kan du koble til VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="3c564-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>