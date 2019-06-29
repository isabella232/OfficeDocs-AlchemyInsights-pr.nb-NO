---
title: Arbeide med iOS VPP programmer regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364869"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="fc193-102">Arbeide med iOS VPP-programmer</span><span class="sxs-lookup"><span data-stu-id="fc193-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="fc193-103">Les [hvordan du administrerer iOS apps kjøpt via et volum Kjøpsprogram med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) å lære om funksjoner, betingelser og trinn for å gjøre bruk av Apple volum kjøpe programmet og støtte for den i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="fc193-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="fc193-104">**Vanlige problemer:** "Jeg har tilordnet en iOS VPP app til brukerne, men installasjonen mislyktes".</span><span class="sxs-lookup"><span data-stu-id="fc193-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="fc193-105">Dette kan skje hvis et enkelt VPP-token brukes på tvers av flere leverandører av mobil enhet management.</span><span class="sxs-lookup"><span data-stu-id="fc193-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="fc193-106">VPP-tokener fra Apple kan bare brukes med én leverandør.</span><span class="sxs-lookup"><span data-stu-id="fc193-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="fc193-107">Hvis du brukte et VPP-token med flere leverandører, må du laste opp token til Intune på nytt.</span><span class="sxs-lookup"><span data-stu-id="fc193-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="fc193-108">Installasjonen kan også mislykkes hvis det totale antallet installasjoner overstiger antall lisenser.</span><span class="sxs-lookup"><span data-stu-id="fc193-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="fc193-109">Hvis du vil vise en Bruksrapport for lisensene, går du til **Intune Mobile apps** \> **App lisenser** -siden.</span><span class="sxs-lookup"><span data-stu-id="fc193-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="fc193-110">Hvis du vil lære å gjenvinne lisenser i bruk, kan du se [denne artikkelen.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="fc193-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
