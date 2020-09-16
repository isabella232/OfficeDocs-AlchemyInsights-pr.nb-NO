---
title: Logge på Windows 10 uten å bruke et passord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719962"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="27fb3-102">Logge på Windows 10 uten å bruke et passord</span><span class="sxs-lookup"><span data-stu-id="27fb3-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="27fb3-103">Vi anbefaler at du bruker et av alternativene for sikker pålogging for Windows Hello, for eksempel en PIN-kode, et ansikts gjenkjenning eller finger avtrykk, hvis det er tilgjengelig for å unngå å måtte skrive inn et passord på Windows-oppstart.</span><span class="sxs-lookup"><span data-stu-id="27fb3-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="27fb3-104">Hvis du virkelig vil deaktivere sikker pålogging, kan du se instruksjonene automatisk Logg på Windows 10 nedenfor.</span><span class="sxs-lookup"><span data-stu-id="27fb3-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="27fb3-105">**Sikre Windows Hello-alternativer til konto passordet**</span><span class="sxs-lookup"><span data-stu-id="27fb3-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="27fb3-106">Gå til **innstillinger > kontoer > påloggings alternativer** (eller klikk [her](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="27fb3-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="27fb3-107">Tilgjengelige påloggings alternativer vil være oppført.</span><span class="sxs-lookup"><span data-stu-id="27fb3-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="27fb3-108">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="27fb3-108">For example:</span></span>

![Påloggings alternativer.](media/sign-in-options.png)

<span data-ttu-id="27fb3-110">Klikk eller trykk et av alternativene for å konfigurere det.</span><span class="sxs-lookup"><span data-stu-id="27fb3-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="27fb3-111">Neste gang du starter eller låser opp Windows, vil du kunne bruke det nye alternativet i stedet for et passord.</span><span class="sxs-lookup"><span data-stu-id="27fb3-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="27fb3-112">**Logge på Windows 10 automatisk**</span><span class="sxs-lookup"><span data-stu-id="27fb3-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="27fb3-113">**Obs**! automatisk pålogging er praktisk, men introduserer en sikkerhets risiko, spesielt hvis PC-en er tilgjengelig for flere personer.</span><span class="sxs-lookup"><span data-stu-id="27fb3-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="27fb3-114">Klikk eller trykk **Start** -knappen på oppgave linjen.</span><span class="sxs-lookup"><span data-stu-id="27fb3-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="27fb3-115">Skriv inn **NETPLWIZ** , og trykk Enter-tasten for å åpne Brukerkontoer-vinduet.</span><span class="sxs-lookup"><span data-stu-id="27fb3-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="27fb3-116">Klikk kontoen du vil logge på automatisk når Windows starter, i **bruker kontoer**.</span><span class="sxs-lookup"><span data-stu-id="27fb3-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="27fb3-117">Fjern merket i avmerkings boksen brukere må angi et bruker navn og passord for å bruke denne data maskinen.</span><span class="sxs-lookup"><span data-stu-id="27fb3-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Brukere må angi et bruker navn og et passord alternativ.](media/users-must-enter-username.png)

5. <span data-ttu-id="27fb3-119">Klikk **OK**.</span><span class="sxs-lookup"><span data-stu-id="27fb3-119">Click **OK**.</span></span> <span data-ttu-id="27fb3-120">Du blir bedt om å skrive inn og bekrefte passordet for kontoen du valgte.</span><span class="sxs-lookup"><span data-stu-id="27fb3-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="27fb3-121">Klikk **OK** for å fullføre.</span><span class="sxs-lookup"><span data-stu-id="27fb3-121">Click **OK** to finish.</span></span> <span data-ttu-id="27fb3-122">Neste gang Windows 10 starter, vil den automatisk logge på kontoen du valgte.</span><span class="sxs-lookup"><span data-stu-id="27fb3-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
