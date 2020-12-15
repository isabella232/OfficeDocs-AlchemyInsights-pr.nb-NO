---
title: Bruke Microsoft Intune til å administrere Internett-tilgang i Microsoft Edge for iOS og Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679614"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="798d0-102">Bruke Microsoft Intune til å administrere Internett-tilgang i Microsoft Edge for iOS og Android</span><span class="sxs-lookup"><span data-stu-id="798d0-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="798d0-103">Microsoft Edge for iOS og Android lar en bruker bla gjennom nettet fra flere, helt atskilte profiler.</span><span class="sxs-lookup"><span data-stu-id="798d0-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="798d0-104">De brede beskyttelses funksjonene for Microsoft 365-data blir tilgjengelige når du abonnerer på Enterprise Mobility + Security Suite, som inkluderer Microsoft Intune og Azure Active Directory Premium-funksjoner, for eksempel betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="798d0-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="798d0-105">Du vil i det minste ønske å distribuere en policy for betinget tilgang som (1) lar brukere koble fra mobile enheter til Microsoft Edge for iOS og Android, og at (2) implementerer en Microsoft Intune-app – beskyttelses policy som gir en beskyttet nett leser opplevelse.</span><span class="sxs-lookup"><span data-stu-id="798d0-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="798d0-106">Hvis du vil forstå hvordan du kan bruke betinget tilgang og policyer, kan du se:</span><span class="sxs-lookup"><span data-stu-id="798d0-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="798d0-107">Bruke Azure Active Directory-policyer for betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="798d0-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="798d0-108">Opprette policyer for Microsoft Intune app Protection</span><span class="sxs-lookup"><span data-stu-id="798d0-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="798d0-109">Bruke enkel pålogging for Azure Active Directory – tilkoblede nett programmer i policy-beskyttede nett lesere</span><span class="sxs-lookup"><span data-stu-id="798d0-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="798d0-110">Bruke app-konfigurasjon til å administrere nett lesings opplevelsen</span><span class="sxs-lookup"><span data-stu-id="798d0-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="798d0-111">Tillat bruk av bare jobb-og skole kontoer</span><span class="sxs-lookup"><span data-stu-id="798d0-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="798d0-112">Distribuere generelle konfigurasjons policyer for apper</span><span class="sxs-lookup"><span data-stu-id="798d0-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="798d0-113">Distribuere policyer for program konfigurasjon for data beskyttelse</span><span class="sxs-lookup"><span data-stu-id="798d0-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="798d0-114">Bruke Microsoft Endpoint Manager til å distribuere policyer for program konfigurasjon</span><span class="sxs-lookup"><span data-stu-id="798d0-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="798d0-115">Hvis du vil lære hvordan du får tilgang til behandlede program logger, kan du se [bruke Microsoft Edge for IOS og Android til å få tilgang til behandlede app](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="798d0-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
