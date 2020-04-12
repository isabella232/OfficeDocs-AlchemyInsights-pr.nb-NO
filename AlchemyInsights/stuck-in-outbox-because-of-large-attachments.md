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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232639"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="c2c3e-102">Løse meldinger som sitter fast i utboksen</span><span class="sxs-lookup"><span data-stu-id="c2c3e-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="c2c3e-103">Vi anbefaler at du starter med å kjøre scenariet ["Jeg har problemer med å sende, motta eller finne e-postmeldinger"](https://aka.ms/SaRA-OutlookSendReceive) fra [verktøyet Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) på den berørte maskinen.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="c2c3e-104">Når en melding sitter fast i utboksen, er den mest sannsynlige årsaken et stort vedlegg eller alternativet "Send umiddelbart når den er tilkoblet" er ikke aktivert.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="c2c3e-105">**Fjern det store tilbehøret**</span><span class="sxs-lookup"><span data-stu-id="c2c3e-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="c2c3e-106">Klikk **Send / motta** > **arbeid frakoblet**.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="c2c3e-107">Klikk **Utboks**i navigasjonsruten.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="c2c3e-108">Herfra kan du:</span><span class="sxs-lookup"><span data-stu-id="c2c3e-108">From here, you can:</span></span> 
    - <span data-ttu-id="c2c3e-109">Slett meldingen.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-109">Delete the message.</span></span> <span data-ttu-id="c2c3e-110">Bare velg det og klikk **Slett**.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="c2c3e-111">Dra meldingen til **kladdemappen,** dobbeltklikk for å åpne meldingen, og slett vedlegget (klikk det og klikk **Slett**).</span><span class="sxs-lookup"><span data-stu-id="c2c3e-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="c2c3e-112">Hvis det oppstår en feil i Outlook som prøver å overføre meldingen, lukker du Outlook.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="c2c3e-113">Det kan ta litt tid å avslutte.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-113">It may take a few moments to exit.</span></span> <span data-ttu-id="c2c3e-114">Hvis Outlook ikke lukkes, trykker du **CTRL+ALT+Slett** og klikker **Start Oppgavebehandling**.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="c2c3e-115">I Oppgavebehandling velger du **kategorien Prosesser,** blar ned til outlook.exe, og klikker **Avslutt prosess**.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="c2c3e-116">Når Outlook lukkes, starter du Outlook på nytt og gjentar trinn 2-3.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="c2c3e-117">Når du har fjernet vedlegget, klikker du **Send / motta** > **arbeid frakoblet** for å fjerne merket for knappen og for å fortsette å jobbe på nettet.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="c2c3e-118">Meldinger blir også sittende fast i utboksen når du klikker **Send**, men du er ikke tilkoblet.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="c2c3e-119">Klikk **Send / motta** og se på Arbeid **frakoblet-knappen.**</span><span class="sxs-lookup"><span data-stu-id="c2c3e-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="c2c3e-120">Hvis den er blå, kobles du fra.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="c2c3e-121">Klikk den for å koble til (knappen blir hvit) og klikk **Send alle**.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="c2c3e-122">**Aktiver Send umiddelbart når du er tilkoblet**</span><span class="sxs-lookup"><span data-stu-id="c2c3e-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="c2c3e-123">Klikk **Alternativer**i kategorien Fil .</span><span class="sxs-lookup"><span data-stu-id="c2c3e-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="c2c3e-124">Klikk **Avansert**i dialogboksen Alternativer for Outlook .</span><span class="sxs-lookup"><span data-stu-id="c2c3e-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="c2c3e-125">Klikk for å aktivere Send **umiddelbart når du er tilkoblet,** i delen Send og motta .</span><span class="sxs-lookup"><span data-stu-id="c2c3e-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="c2c3e-126">Klikk på **OK**.</span><span class="sxs-lookup"><span data-stu-id="c2c3e-126">Click **OK**.</span></span>
 
<span data-ttu-id="c2c3e-127">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="c2c3e-127">For full details, see:</span></span>
- [<span data-ttu-id="c2c3e-128">Video: Sende eller slette en fast e-post</span><span class="sxs-lookup"><span data-stu-id="c2c3e-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="c2c3e-129">E-post forblir i utboksmappen til du manuelt starter en send/motta-operasjon i Outlook</span><span class="sxs-lookup"><span data-stu-id="c2c3e-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
