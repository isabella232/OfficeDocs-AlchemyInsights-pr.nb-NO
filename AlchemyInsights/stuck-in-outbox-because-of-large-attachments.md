---
title: Stakk i utboksen på grunn av store vedlegg
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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441314"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="1b053-102">Rette opp meldinger som sitter fast i utboksen</span><span class="sxs-lookup"><span data-stu-id="1b053-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="1b053-103">Vi anbefaler at du starter ved å kjøre scenariet ["Jeg har problemer med å sende, motta eller finne e-postmeldinger"](https://aka.ms/SaRA-OutlookSendReceive) fra [Microsoft Kundestøtte og gjenoppretting Assistant](https://diagnostics.office.com/#/) verktøyet.</span><span class="sxs-lookup"><span data-stu-id="1b053-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="1b053-104">Når en melding blir værende i utboksen, er de mest sannsynlige årsakene:</span><span class="sxs-lookup"><span data-stu-id="1b053-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="1b053-105">Store vedlegg.</span><span class="sxs-lookup"><span data-stu-id="1b053-105">Large attachments.</span></span>
- <span data-ttu-id="1b053-106">Alternativet **Send umiddelbart når tilkoblet** er ikke aktivert.</span><span class="sxs-lookup"><span data-stu-id="1b053-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="1b053-107">Slik fjerner du store vedlegg:</span><span class="sxs-lookup"><span data-stu-id="1b053-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="1b053-108">Velg **Send/motta** > **arbeid frakoblet**i Outlook.</span><span class="sxs-lookup"><span data-stu-id="1b053-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="1b053-109">Velg **Utboks**i navigasjonsruten.</span><span class="sxs-lookup"><span data-stu-id="1b053-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="1b053-110">Herfra kan du gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="1b053-110">From here, you can:</span></span> 
    - <span data-ttu-id="1b053-111">Slett meldingen (Merk den, og velg deretter **Slett**).</span><span class="sxs-lookup"><span data-stu-id="1b053-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="1b053-112">Dra meldingen til Kladd-mappen, dobbeltklikk for å åpne den, og fjern vedlegget, Velg den, og velg deretter **Slett**).</span><span class="sxs-lookup"><span data-stu-id="1b053-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="1b053-113">Hvis du får en feilmelding som sier at Outlook prøver å overføre meldingen, lukker du Outlook.</span><span class="sxs-lookup"><span data-stu-id="1b053-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="1b053-114">Det kan ta litt tid å avslutte.</span><span class="sxs-lookup"><span data-stu-id="1b053-114">It may take a few moments to exit.</span></span> <span data-ttu-id="1b053-115">Hvis Outlook ikke lukkes, trykker du Ctrl + Alt + Delete og velger **Start Oppgavebehandling**.</span><span class="sxs-lookup"><span data-stu-id="1b053-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="1b053-116">I Oppgavebehandling velger du kategorien **prosesser** , blar ned til Outlook. exe og velger **Avslutt prosess**.</span><span class="sxs-lookup"><span data-stu-id="1b053-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="1b053-117">Når Outlook lukkes, starter du det på nytt og gjentar trinn 2 og 3.</span><span class="sxs-lookup"><span data-stu-id="1b053-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="1b053-118">Når du har fjernet vedlegget, klikker du **Send/motta** > **arbeid frakoblet** for å gjenoppta arbeidet online.</span><span class="sxs-lookup"><span data-stu-id="1b053-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="1b053-119">Meldinger blir også værende i utboksen når du klikker **Send**, men du er ikke tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="1b053-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="1b053-120">Klikk **Send og motta** , og se på **arbeid frakoblet** -knappen.</span><span class="sxs-lookup"><span data-stu-id="1b053-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="1b053-121">Hvis den er blå, er du frakoblet.</span><span class="sxs-lookup"><span data-stu-id="1b053-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="1b053-122">Velg den for å koble til (knappen blir hvit) og klikk på **Send alle**.</span><span class="sxs-lookup"><span data-stu-id="1b053-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="1b053-123">Slik aktiverer du **sending umiddelbart når**du er tilkoblet:</span><span class="sxs-lookup"><span data-stu-id="1b053-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="1b053-124">Velg **fil** > **Alternativer** >  **Avansert**.</span><span class="sxs-lookup"><span data-stu-id="1b053-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="1b053-125">I delen **Send og motta** velger du **Send umiddelbart når**du er tilkoblet, og deretter velger du **OK**.</span><span class="sxs-lookup"><span data-stu-id="1b053-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="1b053-126">For alle detaljer, se:</span><span class="sxs-lookup"><span data-stu-id="1b053-126">For full details see:</span></span>
- [<span data-ttu-id="1b053-127">Video: sende eller slette en fastlåst e-post</span><span class="sxs-lookup"><span data-stu-id="1b053-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="1b053-128">E-post blir værende i Utboks-mappen til du manuelt starter en operasjon for sending/mottak i Outlook</span><span class="sxs-lookup"><span data-stu-id="1b053-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
