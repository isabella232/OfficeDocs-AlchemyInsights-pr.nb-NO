---
title: Eier kan ikke opprette undermappe ved hjelp av Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749139"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="8f9d7-102">Eier kan ikke opprette undermappe ved hjelp av Outlook</span><span class="sxs-lookup"><span data-stu-id="8f9d7-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="8f9d7-103">**Det er et pågående problem med fellesmappeeiere som oppretter undermapper ved hjelp av Outlook. Problemet vil bli løst snart.**</span><span class="sxs-lookup"><span data-stu-id="8f9d7-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="8f9d7-104">I mellomtiden bruker du en av følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="8f9d7-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="8f9d7-105">Bruk Outlook for MAC til å opprette undermappen som problemet påvirker bare Outlook for skrivebordsvinduer (alle versjoner)</span><span class="sxs-lookup"><span data-stu-id="8f9d7-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="8f9d7-106">Be admin opprette undermappen ved hjelp av EXO Shell eller EAC</span><span class="sxs-lookup"><span data-stu-id="8f9d7-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="8f9d7-107">Endre DefaultPublicFolderMailbox/EffectivePublicFolderMailbox på brukeren til en annen postboks enn innholdspostboksen for mappen som forårsaker problemet</span><span class="sxs-lookup"><span data-stu-id="8f9d7-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="8f9d7-108">*Angi postboks bruker1 standardPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="8f9d7-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="8f9d7-109">Vent i en time, start Outlook-klienten på nytt</span><span class="sxs-lookup"><span data-stu-id="8f9d7-109">Wait for an hour, restart outlook client</span></span>