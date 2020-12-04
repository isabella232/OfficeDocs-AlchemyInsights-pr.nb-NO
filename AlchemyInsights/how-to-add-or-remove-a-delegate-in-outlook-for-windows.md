---
title: Slik legger du til eller fjerner en representant i Outlook for Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573576"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="8cc60-102">Slik legger du til eller fjerner en representant i Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="8cc60-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="8cc60-103">Slik legger du til en representant i Outlook for Windows:</span><span class="sxs-lookup"><span data-stu-id="8cc60-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="8cc60-104">Klikk **fil** -fanen etterfulgt av **konto innstillinger**, og velg deretter **representant tilgang**.</span><span class="sxs-lookup"><span data-stu-id="8cc60-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="8cc60-105">Klikk på **Legg til**.</span><span class="sxs-lookup"><span data-stu-id="8cc60-105">Click on **Add**.</span></span> <span data-ttu-id="8cc60-106">Hvis **Legg til** ikke vises, kan det være at en aktiv tilkobling ikke finnes mellom Outlook og Exchange.</span><span class="sxs-lookup"><span data-stu-id="8cc60-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="8cc60-107">Status linjen i Outlook viser tilkoblings statusen.</span><span class="sxs-lookup"><span data-stu-id="8cc60-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="8cc60-108">Skriv inn navnet på personen du vil angi som representant, eller søk og velg navnet i søke resultat listen.</span><span class="sxs-lookup"><span data-stu-id="8cc60-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="8cc60-109">Representanten må være en person i organisasjonens globale adresse liste (GAL).</span><span class="sxs-lookup"><span data-stu-id="8cc60-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="8cc60-110">Klikk **Legg til** etterfulgt av **OK**.</span><span class="sxs-lookup"><span data-stu-id="8cc60-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="8cc60-111">Godta standard innstillingene for tillatelser i dialog boksen **representant tillatelser** , eller velg egen definerte tilgangs nivåer for Exchange-mapper.</span><span class="sxs-lookup"><span data-stu-id="8cc60-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="8cc60-112">Hvis en representant bare trenger tillatelse til å arbeide med møte innkallelser og svar, er standard tillatelses innstillinger som **representant mottar kopier av møte relaterte meldinger som sendes til meg** , er tilstrekkelig.</span><span class="sxs-lookup"><span data-stu-id="8cc60-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="8cc60-113">Du kan la innstillingen for tillatelse til **innboksen** bli **værende.**</span><span class="sxs-lookup"><span data-stu-id="8cc60-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="8cc60-114">Møte invitasjoner og svar vil gå direkte til representantens innboks.</span><span class="sxs-lookup"><span data-stu-id="8cc60-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="8cc60-115">Som standard er representanten gitt **redaktør (kan lese, opprette og endre elementer)** tillatelse til **Kalender** -mappen.</span><span class="sxs-lookup"><span data-stu-id="8cc60-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="8cc60-116">Når representanten svarer på et møte på vegne av deg, legges det automatisk til i **Kalender** -mappen.</span><span class="sxs-lookup"><span data-stu-id="8cc60-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="8cc60-117">Hvis du vil sende en melding for å varsle representanten om de endrede tillatelsene, merker du av for **Send automatisk melding til representant oppsummering av disse tillatelsene** .</span><span class="sxs-lookup"><span data-stu-id="8cc60-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="8cc60-118">Hvis du vil, merker du av for **Representanten kan se mine private elementer** .</span><span class="sxs-lookup"><span data-stu-id="8cc60-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="8cc60-119">Denne innstillingen påvirker alle Exchange-mapper.</span><span class="sxs-lookup"><span data-stu-id="8cc60-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="8cc60-120">Dette inkluderer alle mapper for e-post, kontakter, kalender, oppgaver, notater og logg.</span><span class="sxs-lookup"><span data-stu-id="8cc60-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="8cc60-121">Det er ikke mulig å gi tilgang til private elementer i bare bestemte mapper.</span><span class="sxs-lookup"><span data-stu-id="8cc60-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="8cc60-122">Velg **OK**.</span><span class="sxs-lookup"><span data-stu-id="8cc60-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="8cc60-123">Meldinger som sendes med Send på vegne av-tillatelser, omfatter både representantens og navnene ditt ved siden av **fra**.</span><span class="sxs-lookup"><span data-stu-id="8cc60-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="8cc60-124">Når en melding sendes med Send som-tillatelser, vises bare navnet ditt.</span><span class="sxs-lookup"><span data-stu-id="8cc60-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="8cc60-125">Når du har lagt til en representant, kan de legge til Exchange-postboksen i Outlook-profilen sin.</span><span class="sxs-lookup"><span data-stu-id="8cc60-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="8cc60-126">Hvis du vil ha instruksjoner, kan du se [administrere en annen persons e-post og kalender elementer](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="8cc60-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="8cc60-127">Slik fjerner du en representant i Outlook for Windows:</span><span class="sxs-lookup"><span data-stu-id="8cc60-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="8cc60-128">Klikk på **fil** -fanen.</span><span class="sxs-lookup"><span data-stu-id="8cc60-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="8cc60-129">Klikk på **konto innstillinger** etterfulgt av **representant tilgang**.</span><span class="sxs-lookup"><span data-stu-id="8cc60-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="8cc60-130">Velg navnet på representanten du vil endre tillatelser for, og klikk deretter på **Fjern** etterfulgt av **OK**.</span><span class="sxs-lookup"><span data-stu-id="8cc60-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
