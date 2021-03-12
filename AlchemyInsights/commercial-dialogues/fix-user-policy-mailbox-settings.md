---
title: Løse innstillinger for brukerpolicy/postboks
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750557"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="db453-102">Løse innstillinger for brukerpolicy/postboks</span><span class="sxs-lookup"><span data-stu-id="db453-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="db453-103">Innstillingene for søppelpost i postboksen påvirket denne meldingen.</span><span class="sxs-lookup"><span data-stu-id="db453-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="db453-104">Gjør følgende for å se gjennom innstillingene:</span><span class="sxs-lookup"><span data-stu-id="db453-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="db453-105">Start Skallet for Exchange-administrasjon.</span><span class="sxs-lookup"><span data-stu-id="db453-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="db453-106">Hvis du vil ha mer informasjon, [kan du se Åpne Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="db453-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="db453-107">Kjør denne kommandoen (ved hjelp av brukerens  **e-postadresse): get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="db453-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="db453-108">Kontroller om avsenderens e-postadresse er en del av **TrustedSendersAndDomains** eller **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="db453-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="db453-109">Hvis e-postadressen er i en av listene, må du kanskje fjerne den.</span><span class="sxs-lookup"><span data-stu-id="db453-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="db453-110">Hvis du vil ha mer informasjon, [kan du se Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="db453-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
