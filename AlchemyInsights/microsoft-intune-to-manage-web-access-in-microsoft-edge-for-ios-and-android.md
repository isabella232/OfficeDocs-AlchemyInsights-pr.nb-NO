---
title: Bruke Microsoft Intune til å administrere netttilgang i Microsoft Edge for iOS og Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989683"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="1f634-102">Bruke Microsoft Intune til å administrere netttilgang i Microsoft Edge for iOS og Android</span><span class="sxs-lookup"><span data-stu-id="1f634-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="1f634-103">Microsoft Edge for iOS og Android lar en bruker surfe på nettet fra flere, helt separate profiler.</span><span class="sxs-lookup"><span data-stu-id="1f634-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="1f634-104">De bredeste beskyttelsesfunksjonene for Microsoft 365-data blir tilgjengelige når du abonnerer på Enterprise Mobility + Security-programserien, som inkluderer Microsoft Intune- og Azure Active Directory Premium-funksjoner, for eksempel betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="1f634-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="1f634-105">Som et minimum bør du distribuere en policy for betinget tilgang som (1) lar brukere koble seg fra mobile enheter til Microsoft Edge for iOS og Android, og at (2) implementerer en policy for appbeskyttelse for Microsoft Intune som gir en beskyttet nettleseropplevelse.</span><span class="sxs-lookup"><span data-stu-id="1f634-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="1f634-106">Hvis du vil forstå hvordan du kan bruke betinget tilgang og policyer, kan du se:</span><span class="sxs-lookup"><span data-stu-id="1f634-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="1f634-107">Bruke policyer for betinget tilgang for Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1f634-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="1f634-108">Opprette beskyttelsespolicyer for Microsoft Intune-apper</span><span class="sxs-lookup"><span data-stu-id="1f634-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="1f634-109">Bruke enkel pålogging for Azure Active Directory–tilkoblede nettapper i policybeskyttede nettlesere</span><span class="sxs-lookup"><span data-stu-id="1f634-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="1f634-110">Bruke appkonfigurasjon til å administrere nettleseropplevelsen</span><span class="sxs-lookup"><span data-stu-id="1f634-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="1f634-111">Tillat bruk av bare jobb- og skolekontoer</span><span class="sxs-lookup"><span data-stu-id="1f634-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="1f634-112">Distribuere generelle konfigurasjonspolicyer for apper</span><span class="sxs-lookup"><span data-stu-id="1f634-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="1f634-113">Distribuere policyer for appkonfigurasjon for databeskyttelse</span><span class="sxs-lookup"><span data-stu-id="1f634-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="1f634-114">Bruke Microsoft Endpoint Manager til å distribuere policyer for appkonfigurasjon</span><span class="sxs-lookup"><span data-stu-id="1f634-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="1f634-115">Hvis du vil lære hvordan du får tilgang til administrerte applogger, kan du se Bruke Microsoft Edge for iOS og [Android til å få tilgang til administrerte applogger](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="1f634-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
