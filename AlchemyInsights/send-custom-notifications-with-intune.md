---
title: Sende egendefinerte varslinger med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992321"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="265f7-102">Slik sender du tilpassede varslinger til brukere av administrerte iOS-og Android-enheter</span><span class="sxs-lookup"><span data-stu-id="265f7-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="265f7-103">Tilpassede varslinger for Intune behandles av Company Portal-appen på en brukers enhet.</span><span class="sxs-lookup"><span data-stu-id="265f7-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="265f7-104">Appen oppretter deretter push-varslingen på den enheten.</span><span class="sxs-lookup"><span data-stu-id="265f7-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="265f7-105">Følgende er enhets forutsetninger for å støtte mottak av egendefinerte varslinger, og for appen å deretter opprette push-varsling:</span><span class="sxs-lookup"><span data-stu-id="265f7-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="265f7-106">Enheten må ha Company Portal-appen installert.</span><span class="sxs-lookup"><span data-stu-id="265f7-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="265f7-107">Enheten må tillate at Company Portal-appen sender push-varslinger.</span><span class="sxs-lookup"><span data-stu-id="265f7-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="265f7-108">Når appen er installert eller oppdatert, vil den be brukeren om å tillate varslinger.</span><span class="sxs-lookup"><span data-stu-id="265f7-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="265f7-109">Android-enheter må ha Google Play Services installert.</span><span class="sxs-lookup"><span data-stu-id="265f7-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="265f7-110">Enheten må være registrert i Intune.</span><span class="sxs-lookup"><span data-stu-id="265f7-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="265f7-111">Hvis du vil ha mer informasjon, inkludert hvordan du sender en melding, kan du se [funksjons dokumentasjonen](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="265f7-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
