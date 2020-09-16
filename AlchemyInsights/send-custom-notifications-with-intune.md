---
title: Send egen definerte varsler med Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720655"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="9b9c7-102">Slik sender du egen definerte varsler til brukere av administrerte iOS-og Android-enheter</span><span class="sxs-lookup"><span data-stu-id="9b9c7-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="9b9c7-103">Egen definerte varsler for Intune behandles av Firmaportal-appen på en brukers enhet.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="9b9c7-104">Appen oppretter deretter push-varslingen på enheten.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="9b9c7-105">Følgende er enhets krav for å støtte mottak av egen definerte varsler, og for appen oppretter du push-varslingen:</span><span class="sxs-lookup"><span data-stu-id="9b9c7-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="9b9c7-106">Enheten må ha Firmaportal-appen installert.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="9b9c7-107">Enheten må tillate at Firmaportal-appen kan sende push-varslinger.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="9b9c7-108">Når appen er installert eller oppdatert, blir brukeren bedt om å tillate varslinger.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="9b9c7-109">Android-enheter må ha Google Play Services installert.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="9b9c7-110">Enheten må være registrert hos Intune.</span><span class="sxs-lookup"><span data-stu-id="9b9c7-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="9b9c7-111">Hvis du vil ha mer informasjon, inkludert hvordan du sender en melding, kan du se [funksjons dokumentasjonen](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="9b9c7-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
