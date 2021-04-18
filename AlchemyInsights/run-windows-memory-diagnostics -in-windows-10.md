---
title: Kjøre Windows minnediagnose i Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826676"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="e7c60-102">Kjøre Windows minnediagnose i Windows 10</span><span class="sxs-lookup"><span data-stu-id="e7c60-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="e7c60-103">Hvis Windows og apper på PC-en krasjer, fryser eller oppfører seg ustabilt, kan det hende du har et problem med PC-ens minne (RAM).</span><span class="sxs-lookup"><span data-stu-id="e7c60-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="e7c60-104">Du kan kjøre Windows minnediagnose for å se etter problemer med PC-ens RAM.</span><span class="sxs-lookup"><span data-stu-id="e7c60-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="e7c60-105">Skriv inn **minnediagnose** i søkeboksen på oppgavelinjen, og velg deretter **Windows minnediagnose**.</span><span class="sxs-lookup"><span data-stu-id="e7c60-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="e7c60-106">For å kjøre diagnosen må PC-en startes på nytt.</span><span class="sxs-lookup"><span data-stu-id="e7c60-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="e7c60-107">Du har muligheten til å starte på nytt umiddelbart (lagre arbeidet, og lukk åpne dokumenter og e-postmeldinger først), eller planlegg at diagnosen skal kjøres automatisk neste gang PC-en startes på nytt:</span><span class="sxs-lookup"><span data-stu-id="e7c60-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows minnediagnose](media/windows-memory-diagnostic.png)

<span data-ttu-id="e7c60-109">Når PC-en startes på nytt, kjøres **Windows Diagnoseverktøy for minne** automatisk.</span><span class="sxs-lookup"><span data-stu-id="e7c60-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="e7c60-110">Status og fremdrift vises mens diagnosen kjører, og du har muligheten til å avbryte diagnosen ved å trykke på **ESC**-knappen på tastaturet.</span><span class="sxs-lookup"><span data-stu-id="e7c60-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="e7c60-111">Når diagnosen er fullført, starter Windows normalt.</span><span class="sxs-lookup"><span data-stu-id="e7c60-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="e7c60-112">Rett etter du har startet på nytt, når skrivebordet vises, vises en varsling (ved siden av **Handlingssenter**-ikonet på oppgavelinjen), for å indikere om minnefeil ble funnet.</span><span class="sxs-lookup"><span data-stu-id="e7c60-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="e7c60-113">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="e7c60-113">For example:</span></span>

<span data-ttu-id="e7c60-114">Her er Handlingssenter-ikonet:</span><span class="sxs-lookup"><span data-stu-id="e7c60-114">Here's the Action Center icon:</span></span> ![Handlingssenter-ikon](media/action-center-icon.png) 

<span data-ttu-id="e7c60-116">Og en eksempelvarsling:</span><span class="sxs-lookup"><span data-stu-id="e7c60-116">And a sample notification:</span></span> ![Ingen minnefeil](media/no-memory-errors.png)

<span data-ttu-id="e7c60-118">Hvis du gikk glipp av varslingen, kan du velge **Handlingssenter**-ikonet på oppgavelinjen, for å vise **Handlingssenter** og se en rullbar liste over varslinger.</span><span class="sxs-lookup"><span data-stu-id="e7c60-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="e7c60-119">Hvis du vil gå gjennom detaljert informasjon, skriver du inn **hendelse** i søkeboksen på oppgavelinjen, og velger deretter **Hendelsesliste**.</span><span class="sxs-lookup"><span data-stu-id="e7c60-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="e7c60-120">Gå til **Windows-logger > System** i ruten til venstre i **Hendelsesliste**.</span><span class="sxs-lookup"><span data-stu-id="e7c60-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="e7c60-121">Skann nedover listen i ruten til høyre, mens du ser på **Kilde**-kolonnen, til du ser hendelser med kildeverdien **Minnediagnose-resultater**.</span><span class="sxs-lookup"><span data-stu-id="e7c60-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="e7c60-122">Uthev hver hendelse som dette, og se resultatinformasjonen i boksen under **Generell**-fanen under listen.</span><span class="sxs-lookup"><span data-stu-id="e7c60-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
