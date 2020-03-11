---
title: Logge på Windows 10 uten å bruke et passord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588289"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="73c7a-102">Logge på Windows 10 uten å bruke et passord</span><span class="sxs-lookup"><span data-stu-id="73c7a-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="73c7a-103">Hvis du vil unngå å måtte skrive inn et passord ved oppstart av Windows, anbefaler vi at du bruker et av windows Hello-sikre påloggingsalternativene, for eksempel en PIN-kode, ansiktsgjenkjenning eller fingeravtrykk, hvis tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="73c7a-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="73c7a-104">Hvis du virkelig vil deaktivere sikker pålogging, kan du se instruksjonene "Logg på Windows 10 automatisk" nedenfor.</span><span class="sxs-lookup"><span data-stu-id="73c7a-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="73c7a-105">**Sikre Windows Hello-alternativer til kontopassordet**</span><span class="sxs-lookup"><span data-stu-id="73c7a-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="73c7a-106">Gå til **Innstillinger > Kontoer > Påloggingsalternativer** (eller klikk [her).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="73c7a-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="73c7a-107">Tilgjengelige påloggingsalternativer vises.</span><span class="sxs-lookup"><span data-stu-id="73c7a-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="73c7a-108">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="73c7a-108">For example:</span></span>

![Påloggingsalternativer.](media/sign-in-options.png)

<span data-ttu-id="73c7a-110">Klikk eller trykk på ett av alternativene for å konfigurere det.</span><span class="sxs-lookup"><span data-stu-id="73c7a-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="73c7a-111">Neste gang du starter eller låser opp Windows, kan du bruke det nye alternativet i stedet for et passord.</span><span class="sxs-lookup"><span data-stu-id="73c7a-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="73c7a-112">**Logge på Windows 10 automatisk**</span><span class="sxs-lookup"><span data-stu-id="73c7a-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="73c7a-113">**Merk:** Automatisk pålogging er praktisk, men introduserer en sikkerhetsrisiko, spesielt hvis PCen er tilgjengelig av flere personer.</span><span class="sxs-lookup"><span data-stu-id="73c7a-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="73c7a-114">Klikk eller trykk **startknappen** på oppgavelinjen.</span><span class="sxs-lookup"><span data-stu-id="73c7a-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="73c7a-115">Skriv inn **netplwiz,** og trykk på Enter-tasten for å åpne Brukerkontoer-vinduet.</span><span class="sxs-lookup"><span data-stu-id="73c7a-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="73c7a-116">Klikk kontoen du vil logge på automatisk når Windows starter, i **Brukerkontoer.**</span><span class="sxs-lookup"><span data-stu-id="73c7a-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="73c7a-117">Fjern merket for "Brukere må skrive inn et brukernavn og passord for å bruke denne datamaskinen".</span><span class="sxs-lookup"><span data-stu-id="73c7a-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Brukere må skrive inn et alternativ for brukernavn og passord.](media/users-must-enter-username.png)

5. <span data-ttu-id="73c7a-119">Klikk på **OK**.</span><span class="sxs-lookup"><span data-stu-id="73c7a-119">Click **OK**.</span></span> <span data-ttu-id="73c7a-120">Du vil bli bedt om å skrive inn og bekrefte passordet for kontoen du valgte.</span><span class="sxs-lookup"><span data-stu-id="73c7a-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="73c7a-121">Klikk **OK** for å fullføre.</span><span class="sxs-lookup"><span data-stu-id="73c7a-121">Click **OK** to finish.</span></span> <span data-ttu-id="73c7a-122">Neste gang Windows 10 starter, logger den automatisk på kontoen du valgte.</span><span class="sxs-lookup"><span data-stu-id="73c7a-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
