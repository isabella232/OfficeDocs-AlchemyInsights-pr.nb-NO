---
title: 'Slik konfigurerer du automatisk svar for alle e-postmeldinger som sendes til Microsoft 365-gruppen:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: c3c1d4e6b16b54d92771d7bdecdc9cb12bbf888c
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481864"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a><span data-ttu-id="708c0-102">Slik konfigurerer du automatisk svar for alle e-postmeldinger som sendes til Microsoft 365-gruppen:</span><span class="sxs-lookup"><span data-stu-id="708c0-102">To configure auto reply for all emails sent to Microsoft 365 group:</span></span>

<span data-ttu-id="708c0-103">**Koble til EXO PowerShell ved hjelp av administratorkontoen for leieren, og bruk følgende kommando:**</span><span class="sxs-lookup"><span data-stu-id="708c0-103">**Connect to EXO PowerShell using tenant admin account and use following command**:</span></span>

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> <span data-ttu-id="708c0-104">Endre **gruppepostboksen** til et gruppenavn som du vil konfigurere automatisk svar på.</span><span class="sxs-lookup"><span data-stu-id="708c0-104">Change **groupmailbox** to a group name that you want to configure auto reply on.</span></span>

