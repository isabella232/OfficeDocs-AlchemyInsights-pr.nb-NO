---
title: Kjøre Windows-minnediagnostikk i Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357787"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="2fe51-102">Kjøre Windows-minnediagnostikk i Windows 10</span><span class="sxs-lookup"><span data-stu-id="2fe51-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="2fe51-103">Hvis Windows og apper på PCen krasjer, fryser eller opptrer på en ustabil måte, kan du ha et problem med PCens minne (RAM).</span><span class="sxs-lookup"><span data-stu-id="2fe51-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="2fe51-104">Du kan kjøre Windows Memory Diagnostic for å se etter problemer med PCens RAM.</span><span class="sxs-lookup"><span data-stu-id="2fe51-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="2fe51-105">Skriv inn diagnose av **minne**i søkeboksen på oppgavelinjen, og velg deretter **Windows Memory Diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="2fe51-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="2fe51-106">For å kjøre diagnose, må PCen starte på nytt.</span><span class="sxs-lookup"><span data-stu-id="2fe51-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="2fe51-107">Du har muligheten til å starte på nytt umiddelbart (vennligst lagre arbeidet og lukk åpne dokumenter og e-post først), eller planlegge at diagnoseenheten skal kjøres automatisk neste gang PCen starter på nytt:</span><span class="sxs-lookup"><span data-stu-id="2fe51-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnose av Windows-minne](media/windows-memory-diagnostic.png)

<span data-ttu-id="2fe51-109">Når PCen starter på nytt, **kjøres Diagnoseverktøyet for Windows-minne** automatisk.</span><span class="sxs-lookup"><span data-stu-id="2fe51-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="2fe51-110">Status og fremdrift vises når diagnostikken kjøres, og du har muligheten til å avbryte diagnostikken ved å trykke **ESC-tasten** på tastaturet.</span><span class="sxs-lookup"><span data-stu-id="2fe51-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="2fe51-111">Når diagnostikken er fullført, starter Windows normalt.</span><span class="sxs-lookup"><span data-stu-id="2fe51-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="2fe51-112">Umiddelbart etter omstart, når skrivebordet vises, vises et varsel (ved siden av **Handlingssenter-ikonet** på oppgavelinjen), for å angi om det ble funnet minnefeil.</span><span class="sxs-lookup"><span data-stu-id="2fe51-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="2fe51-113">For eksempel,</span><span class="sxs-lookup"><span data-stu-id="2fe51-113">For example:</span></span>

<span data-ttu-id="2fe51-114">Her er Handlingssenter-ikonet:</span><span class="sxs-lookup"><span data-stu-id="2fe51-114">Here's the Action Center icon:</span></span> ![Handlingssenter-ikon](media/action-center-icon.png) 

<span data-ttu-id="2fe51-116">Og et eksempelvarsel:</span><span class="sxs-lookup"><span data-stu-id="2fe51-116">And a sample notification:</span></span> ![Ingen minnefeil](media/no-memory-errors.png)

<span data-ttu-id="2fe51-118">Hvis du har gått glipp av varselet, kan du velge **Handlingssenter-ikonet** på oppgavelinjen for å vise **handlingssenteret** og se en rullbar liste over varsler.</span><span class="sxs-lookup"><span data-stu-id="2fe51-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="2fe51-119">Hvis du vil se gjennom detaljert informasjon, skriver du inn **hendelse** i søkeboksen på oppgavelinjen, og deretter velger du **Hendelsesliste**.</span><span class="sxs-lookup"><span data-stu-id="2fe51-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="2fe51-120">I ruten til venstre for **Hendelsesliste** **navigerer**du til Windows Logger > System .</span><span class="sxs-lookup"><span data-stu-id="2fe51-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="2fe51-121">I ruten til høyre skanner du ned listen **Source** mens du ser på Kilde-kolonnen, til du ser hendelser med **minnediagnoseresultater**for kildeverdi .</span><span class="sxs-lookup"><span data-stu-id="2fe51-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="2fe51-122">Merk hver slik hendelse, og se resultatinformasjonen i boksen under **Kategorien Generelt** under listen.</span><span class="sxs-lookup"><span data-stu-id="2fe51-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
