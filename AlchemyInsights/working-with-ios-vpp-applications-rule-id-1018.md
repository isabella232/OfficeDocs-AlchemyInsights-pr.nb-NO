---
title: Arbeide med iOS VPP-programmer Regel-ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719966"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="5b3d3-102">Arbeide med iOS VPP-programmer</span><span class="sxs-lookup"><span data-stu-id="5b3d3-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="5b3d3-103">Les [Slik administrerer du iOS-apper som er kjøpt gjennom et program for volumkjøp, med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) for å lære om funksjoner, begrensninger og trinn for å gjøre bruk av Apples volumkjøpsprogram og støtte for det i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="5b3d3-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="5b3d3-104">**Vanlige problemer:** "Jeg tilordnet en iOS VPP-app til brukerne mine, men installasjonen mislyktes."</span><span class="sxs-lookup"><span data-stu-id="5b3d3-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="5b3d3-105">Dette kan skje hvis ett enkelt VPP-token brukes på tvers av flere leverandører av administrasjon av mobilenheter.</span><span class="sxs-lookup"><span data-stu-id="5b3d3-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="5b3d3-106">VPP-tokener fra Apple kan bare brukes med én leverandør.</span><span class="sxs-lookup"><span data-stu-id="5b3d3-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="5b3d3-107">Hvis du brukte et VPP-token med flere leverandører, må du laste opp tokenet på nytt til Intune.</span><span class="sxs-lookup"><span data-stu-id="5b3d3-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="5b3d3-108">Installasjonen kan også mislykkes hvis det totale antallet installasjoner overskrider antall lisenser.</span><span class="sxs-lookup"><span data-stu-id="5b3d3-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="5b3d3-109">Hvis du vil vise en bruksrapport for lisensene dine, går du til siden Lisenser for **Intune-apper-appen.** \> **App licenses**</span><span class="sxs-lookup"><span data-stu-id="5b3d3-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="5b3d3-110">Hvis du vil lære hvordan du tar tilbake lisenser i bruk, kan du se [denne artikkelen.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="5b3d3-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
