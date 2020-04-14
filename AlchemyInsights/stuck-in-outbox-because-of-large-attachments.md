---
title: Sitter fast i utboksen på grunn av store vedlegg
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241261"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="28835-102">Løse meldinger som sitter fast i utboksen</span><span class="sxs-lookup"><span data-stu-id="28835-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="28835-103">Vi anbefaler at du starter med å kjøre scenariet ["Jeg har problemer med å sende, motta eller finne e-postmeldinger"](https://aka.ms/SaRA-OutlookSendReceive) fra [verktøyet Microsoft Support and Recovery Assistant.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="28835-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="28835-104">Når en melding sitter fast i utboksen, er den mest sannsynlige årsaken et stort vedlegg eller alternativet "Send umiddelbart når den er tilkoblet" er ikke aktivert.</span><span class="sxs-lookup"><span data-stu-id="28835-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="28835-105">**Fjern det store tilbehøret**</span><span class="sxs-lookup"><span data-stu-id="28835-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="28835-106">I Outlook velger du **Send / motta** > **arbeid frakoblet**.</span><span class="sxs-lookup"><span data-stu-id="28835-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="28835-107">Velg **Utboks**i navigasjonsruten.</span><span class="sxs-lookup"><span data-stu-id="28835-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="28835-108">Herfra kan du:</span><span class="sxs-lookup"><span data-stu-id="28835-108">From here, you can:</span></span> 
    - <span data-ttu-id="28835-109">Slett meldingen (velg den, og velg deretter **Slett**).</span><span class="sxs-lookup"><span data-stu-id="28835-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="28835-110">Dra meldingen til Kladd-mappen, dobbeltklikk for å åpne den, og fjern vedlegget, velg den og velg deretter **Slett**).</span><span class="sxs-lookup"><span data-stu-id="28835-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="28835-111">Hvis du får en feilmelding som sier at Outlook prøver å overføre meldingen, lukker du Outlook.</span><span class="sxs-lookup"><span data-stu-id="28835-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="28835-112">Det kan ta litt tid å avslutte.</span><span class="sxs-lookup"><span data-stu-id="28835-112">It may take a few moments to exit.</span></span> <span data-ttu-id="28835-113">Hvis Outlook ikke lukkes, trykker du CTRL+ALT+Slett og velger **Start Oppgavebehandling**.</span><span class="sxs-lookup"><span data-stu-id="28835-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="28835-114">I Oppgavebehandling velger du **kategorien Prosesser,** blar ned til outlook.exe, og velger **Avslutt prosess**.</span><span class="sxs-lookup"><span data-stu-id="28835-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="28835-115">Når Outlook lukkes, starter du den på nytt og gjentar trinn 2 og 3.</span><span class="sxs-lookup"><span data-stu-id="28835-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="28835-116">Når du har fjernet vedlegget, klikker du **Send / motta** > **arbeid frakoblet** for å fortsette arbeidet på nettet.</span><span class="sxs-lookup"><span data-stu-id="28835-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="28835-117">Meldinger blir også sittende fast i utboksen når du klikker **Send**, men du er ikke tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="28835-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="28835-118">Klikk **Send / motta** og se på Arbeid **frakoblet-knappen.**</span><span class="sxs-lookup"><span data-stu-id="28835-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="28835-119">Hvis den er blå, kobles du fra.</span><span class="sxs-lookup"><span data-stu-id="28835-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="28835-120">Klikk den for å koble til (knappen blir hvit) og klikk **Send alle**.</span><span class="sxs-lookup"><span data-stu-id="28835-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="28835-121">**Aktiver Send umiddelbart når du er tilkoblet**</span><span class="sxs-lookup"><span data-stu-id="28835-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="28835-122">Klikk **Alternativer**i kategorien Fil .</span><span class="sxs-lookup"><span data-stu-id="28835-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="28835-123">Klikk **Avansert**i dialogboksen Alternativer for Outlook .</span><span class="sxs-lookup"><span data-stu-id="28835-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="28835-124">Klikk for å aktivere Send **umiddelbart når du er tilkoblet,** i delen Send og motta .</span><span class="sxs-lookup"><span data-stu-id="28835-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="28835-125">Klikk på **OK**.</span><span class="sxs-lookup"><span data-stu-id="28835-125">Click **OK**.</span></span>
 
<span data-ttu-id="28835-126">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="28835-126">For full details, see:</span></span>
- [<span data-ttu-id="28835-127">Video: Sende eller slette en fast e-post</span><span class="sxs-lookup"><span data-stu-id="28835-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="28835-128">E-post forblir i utboksmappen til du manuelt starter en send/motta-operasjon i Outlook</span><span class="sxs-lookup"><span data-stu-id="28835-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
