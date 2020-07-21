---
title: Brukeren får feil AADSTS7000112 Yammer er deaktivert
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198365"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="b7ef1-102">Brukeren får feil AADSTS7000112 Yammer er deaktivert</span><span class="sxs-lookup"><span data-stu-id="b7ef1-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="b7ef1-103">Hvis du får feilmeldingen "AADSTS7000112: Programmet '00000005-0000-0ff1-ce00-00000000000'(Yammer) er deaktivert", finnes det et problem med tjenestehovedstolen i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="b7ef1-104">En administrator kan ha deaktivert tjenestekontohaveren for å blokkere tilgangen til Yammer.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="b7ef1-105">Deaktivering av servicekontohaveren anbefales ikke og kan forårsake flere problemer.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="b7ef1-106">Hvis du vil ha mer informasjon om den støttede tilnærmingen for å blokkere brukertilgang til Yammer, kan du se [Deaktivere Yammer-tilgang for Microsoft 365-brukere](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="b7ef1-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="b7ef1-107">Slik løser du dette problemet i Azure Portal og gjenoppretter brukertilgang til Yammer:</span><span class="sxs-lookup"><span data-stu-id="b7ef1-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="b7ef1-108">Åpne Azure Active Directory-siden, og velg **Enterprise-programmer** under **Behandle** i venstre navigasjonsrute.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="b7ef1-109">Skriv inn **Office 365 Yammer** i søkeboksen, og velg programnavnet for å åpne innstillinger.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="b7ef1-110">Velg **Egenskaper** under **Behandle** i navigasjonsruten til venstre.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="b7ef1-111">Angi verdien for Aktivert for brukere til **Yes**å logge **Save** **på?**</span><span class="sxs-lookup"><span data-stu-id="b7ef1-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="b7ef1-112">Logg på Yammer på nytt.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-112">Sign in to Yammer again.</span></span> <span data-ttu-id="b7ef1-113">Det kan hende du må slette informasjonskapsler.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-113">You might need to clear cookies.</span></span>

<span data-ttu-id="b7ef1-114">Du kan også kjøre PowerShell-kommandoer for å angi verdien.</span><span class="sxs-lookup"><span data-stu-id="b7ef1-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="b7ef1-115">Hvis du vil ha mer informasjon, kan du se ["Beklager, men vi har problemer med å logge deg på" feil når du klikker Yammer-flisen i Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="b7ef1-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 