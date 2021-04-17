---
title: Eier kan ikke opprette undermappe ved hjelp av Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836144"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="41ede-102">Eier kan ikke opprette undermappe ved hjelp av Outlook</span><span class="sxs-lookup"><span data-stu-id="41ede-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="41ede-103">**Det er et pågående problem med eiere av fellesmapper som oppretter undermapper ved hjelp av Outlook. Problemet blir løst snart.**</span><span class="sxs-lookup"><span data-stu-id="41ede-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="41ede-104">I mellomtiden kan du bruke en av følgende midlertidige løsninger:</span><span class="sxs-lookup"><span data-stu-id="41ede-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="41ede-105">Bruk Outlook for MAC til å opprette undermappen fordi problemet bare påvirker Outlook for skrivebordsvinduer (alle versjoner)</span><span class="sxs-lookup"><span data-stu-id="41ede-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="41ede-106">Få administrator til å opprette undermappen ved hjelp av EXO Shell eller EAC</span><span class="sxs-lookup"><span data-stu-id="41ede-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="41ede-107">Endre DefaultPublicFolderMailbox/EffectivePublicFolderMailbox for brukeren til en annen postboks enn innholdspostboksen for mappen som forårsaker problemet</span><span class="sxs-lookup"><span data-stu-id="41ede-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="41ede-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="41ede-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="41ede-109">Vent en time, start Outlook-klienten på nytt</span><span class="sxs-lookup"><span data-stu-id="41ede-109">Wait for an hour, restart outlook client</span></span>