---
title: Endre Microsoft Edge ved å bruke data katalog variabler i stedet for hardkodete baner
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679158"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="46e23-102">Endre Microsoft Edge ved å bruke data katalog variabler i stedet for hardkodete baner</span><span class="sxs-lookup"><span data-stu-id="46e23-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="46e23-103">I Windows kan du for eksempel lagre profil dataene under en brukers lokale program data i stedet for i standard plasseringen, ved å angi **UserDataDir** -policyen til **$ {local_app_data} \Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="46e23-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="46e23-104">Hvis du vil ha mer informasjon, kan du se [opprette Microsoft Edge user data Directory-variabler](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span><span class="sxs-lookup"><span data-stu-id="46e23-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>