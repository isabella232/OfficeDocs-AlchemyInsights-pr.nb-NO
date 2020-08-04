---
title: Intune Wi-Fi-profiler
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555315"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="228a6-102">Intune Wi-Fi-profiler</span><span class="sxs-lookup"><span data-stu-id="228a6-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="228a6-103">Vellykket implementering av Wi-Fi-tilkobling for MDM-klienter avhenger av en riktig distribuert profil som gjenspeiler kravene til bedriftens Wi-Fi-infrastruktur.</span><span class="sxs-lookup"><span data-stu-id="228a6-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="228a6-104">Hvis du vil se gjennom de riktige innstillingene for klientplattformene du undersøker, kan du se:</span><span class="sxs-lookup"><span data-stu-id="228a6-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="228a6-105">Legge til Wi-Fi-innstillinger for enheter som kjører Android i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="228a6-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="228a6-106">Legge til Wi-Fi-innstillinger for Android Enterprise dedikerte og fullstendig administrerte enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="228a6-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="228a6-107">Legge til Wi-Fi-innstillinger for iOS- og iPadOS-enheter i Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="228a6-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="228a6-108">Legge til Wi-Fi-innstillinger for Windows 10 og senere enheter i Intune</span><span class="sxs-lookup"><span data-stu-id="228a6-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="228a6-109">Importere Wi-Fi-innstillinger for Windows-enheter i Intune</span><span class="sxs-lookup"><span data-stu-id="228a6-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="228a6-110">**Vanlige problemer**</span><span class="sxs-lookup"><span data-stu-id="228a6-110">**Common Issues**</span></span>

<span data-ttu-id="228a6-111">**Jeg distribuerer en Wi-Fi-profil som er avhengig av et distribuert sertifikat som er angitt i Wi-Fi-profilen. Konfigurasjonsprofilene viser imidlertid en feilstatus.**</span><span class="sxs-lookup"><span data-stu-id="228a6-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="228a6-112">Kontroller at enheten mottok sertifikatet.</span><span class="sxs-lookup"><span data-stu-id="228a6-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="228a6-113">Gå til **Alle enheter i** Intune, og velg enheten > **Enhetskonfigurasjon**.</span><span class="sxs-lookup"><span data-stu-id="228a6-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="228a6-114">Kontroller at alle forventede profiler er oppført og i en vellykket tilstand.</span><span class="sxs-lookup"><span data-stu-id="228a6-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="228a6-115">For en Android-profil, hvis du har mellomliggende sertifikater i sertifikatkjeden, må du kontrollere at de distribueres til Android-enheter.</span><span class="sxs-lookup"><span data-stu-id="228a6-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="228a6-116">Hvis du vil kontrollere sertifikatstatusen, går du til **Enhetskonfigurasjonsprofiler**  >  **Profiles**  >  **Android mellomliggende CA**  >  **Properties**  >  **Trusted Certificate**.</span><span class="sxs-lookup"><span data-stu-id="228a6-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="228a6-117">Hvis du fortsatt ser feil, kan du se gjennom avsnittene for prosedyrer og feilsøking.</span><span class="sxs-lookup"><span data-stu-id="228a6-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="228a6-118">Hvis du vil ha mer informasjon, kan du se [Oversikt for feilsøking av SCEP-sertifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="228a6-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="228a6-119">**Jeg distribuerte en Wi-Fi-profil til en enhet. Intune viser at det var vellykket, men enheten kobler ikke til Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="228a6-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="228a6-120">En vellykket status betyr at Intune har distribuert profilen som konfigurert.</span><span class="sxs-lookup"><span data-stu-id="228a6-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="228a6-121">Disse konfigurasjonene samsvarer imidlertid kanskje ikke med kravene til nettverket og/eller godkjenningen.</span><span class="sxs-lookup"><span data-stu-id="228a6-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="228a6-122">Hvis du vil ha mer informasjon om den forsøkte tilkoblingen, kan du se gjennom logger i infrastruktur- og godkjenningstjenesten (på Wi-Fi Access Point controller og NPS/Radius-serveren).</span><span class="sxs-lookup"><span data-stu-id="228a6-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="228a6-123">Du må kanskje samarbeide med nettverksinfrastrukturteamet, eller tredjeparts Wi-Fi-leverandøren, for å samle inn og se gjennom logger.</span><span class="sxs-lookup"><span data-stu-id="228a6-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>