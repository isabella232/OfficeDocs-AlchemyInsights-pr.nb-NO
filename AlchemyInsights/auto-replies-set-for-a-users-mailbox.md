---
title: Angi automatiske svar for en postboks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509510"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="d65ad-102">Angi automatiske svar for postboksen til en bruker</span><span class="sxs-lookup"><span data-stu-id="d65ad-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="d65ad-103">**Metode 1**</span><span class="sxs-lookup"><span data-stu-id="d65ad-103">**Method 1**</span></span>

1. <span data-ttu-id="d65ad-104">Logg på Office 365-portalen.</span><span class="sxs-lookup"><span data-stu-id="d65ad-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="d65ad-105">Gå til **Brukere > Aktive brukere** (eller **Grupper > Delte postbokser** dersom du angir dette for en delt postboks).</span><span class="sxs-lookup"><span data-stu-id="d65ad-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="d65ad-106">Velg en bruker som har en Microsoft Exchange-postboks.</span><span class="sxs-lookup"><span data-stu-id="d65ad-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="d65ad-107">Gå til **E-postinnstillinger > Automatiske svar**i undermenyen til høyre (hvis det er en delt postboks, klikker du bare **Automatiske svar** i undermenyen).</span><span class="sxs-lookup"><span data-stu-id="d65ad-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="d65ad-108">**Metode 2**</span><span class="sxs-lookup"><span data-stu-id="d65ad-108">**Method 2**</span></span>

1. <span data-ttu-id="d65ad-109">Logg på Office 365-administratorportalen med legitimasjon for administrator. </span><span class="sxs-lookup"><span data-stu-id="d65ad-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="d65ad-110">Utvid **Administrasjonssentre**, og klikk deretter på **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="d65ad-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="d65ad-111">Klikk på bildet oppe i høyre hjørne, klikk **Annen bruker**, og velg deretter den brukerpostboksen som du vil endre.</span><span class="sxs-lookup"><span data-stu-id="d65ad-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="d65ad-112">Velg **Alternativer** på venstre side, klikk på **Organiser e-post**, og klikk deretter på **Automatiske svar.**</span><span class="sxs-lookup"><span data-stu-id="d65ad-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="d65ad-113">**Metode 3**</span><span class="sxs-lookup"><span data-stu-id="d65ad-113">**Method 3**</span></span>

<span data-ttu-id="d65ad-114">Kjør følgende cmdlet i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d65ad-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="d65ad-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="d65ad-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="d65ad-116">Hvis du vil ha mer informasjon om denne cmdleten, kan du se [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="d65ad-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
