---
title: Arbeide med iOS VPP programmer regel-Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303605"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="81f8c-102">Arbeide med iOS VPP-programmer</span><span class="sxs-lookup"><span data-stu-id="81f8c-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="81f8c-103">Les [hvordan du administrerer iOS apps kjøpt via et volum Kjøpsprogram med Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) å lære om funksjoner, betingelser og trinn for å gjøre bruk av Apple volum kjøpe programmet og støtte for den i Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="81f8c-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="81f8c-104">**Vanlige problemer:** "Jeg har tilordnet en iOS VPP app til brukerne, men installasjonen mislyktes".</span><span class="sxs-lookup"><span data-stu-id="81f8c-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="81f8c-p101">Dette kan skje hvis et enkelt VPP-token brukes på tvers av flere leverandører av mobil enhet management. VPP-tokener fra Apple kan bare brukes med én leverandør. Hvis du brukte et VPP-token med flere leverandører, må du laste opp token til Intune på nytt.</span><span class="sxs-lookup"><span data-stu-id="81f8c-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="81f8c-p102">Installasjonen kan også mislykkes hvis det totale antallet installasjoner overstiger antall lisenser. Hvis du vil vise en Bruksrapport for lisensene, går du til **Intune Mobile apps** \> **App lisenser** -siden. Hvis du vil lære å gjenvinne lisenser i bruk, kan du se [denne artikkelen.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="81f8c-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

