---
title: Problemer med legitimasjon
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063682"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="ab763-102">Problemer med legitimasjon</span><span class="sxs-lookup"><span data-stu-id="ab763-102">Issues with credentials</span></span>

<span data-ttu-id="ab763-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow describes](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) how to program directly against the OAuth 2.0 client credentials grant flow.</span><span class="sxs-lookup"><span data-stu-id="ab763-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="ab763-104">**Hvordan behandler jeg passord eller sertifikatlegitimasjon for et program?**</span><span class="sxs-lookup"><span data-stu-id="ab763-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="ab763-105">I Azure CLI kan du bruke [az ad-app-legitimasjon](https://docs.microsoft.com/cli/azure/ad/app/credential) til å slette, liste opp eller tilbakestille passordet eller sertifikatlegitimasjonen til et program.</span><span class="sxs-lookup"><span data-stu-id="ab763-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="ab763-106">**Hvordan tilbakestiller brukerne passordene sine?**</span><span class="sxs-lookup"><span data-stu-id="ab763-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="ab763-107">Brukere må registrere [seg for selvbetjent tilbakestilling](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) av passord før de kan tilbakestille passordene sine.</span><span class="sxs-lookup"><span data-stu-id="ab763-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="ab763-108">Når en bruker har registrert seg, kan de følge instruksjonene i denne artikkelen for å tilbakestille passordet: Tilbakestill [jobb- eller skolepassordet.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="ab763-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="ab763-109">**Hvordan endrer brukerne passordene sine?**</span><span class="sxs-lookup"><span data-stu-id="ab763-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="ab763-110">Brukere kan følge fremgangsmåten i denne artikkelen for å endre passordene sine: [Slik endrer du passordet.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="ab763-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="ab763-111">De kan også [administrere app-passord for totrinnskontroll.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="ab763-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="ab763-112">**Brukeren får en feilmelding når jeg endrer eller tilbakestiller passordet**</span><span class="sxs-lookup"><span data-stu-id="ab763-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="ab763-113">Denne koblingen gir informasjon om vanlige problemer som kan oppstå når en bruker prøver å tilbakestille passordet sitt: [Vanlige problemer og deres løsninger](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="ab763-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="ab763-114">**Jeg har problemer med å tilbakestille passordet til en bruker**</span><span class="sxs-lookup"><span data-stu-id="ab763-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="ab763-115">Kontroller at du er autorisert til å tilbakestille passord.</span><span class="sxs-lookup"><span data-stu-id="ab763-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="ab763-116">*Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.*</span><span class="sxs-lookup"><span data-stu-id="ab763-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ab763-117">Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.</span><span class="sxs-lookup"><span data-stu-id="ab763-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="ab763-118">Kontroller at du forstår lisensieringskravene:</span><span class="sxs-lookup"><span data-stu-id="ab763-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="ab763-119">Du må ha minst én lisens tilordnet i organisasjonen:</span><span class="sxs-lookup"><span data-stu-id="ab763-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="ab763-120">**Bare skybrukere** – alle Office 365 (O365) betalte SKU-er, eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="ab763-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="ab763-121">**Skybrukere og/eller** lokale brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="ab763-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="ab763-122">Hvis du vil lære mer om lisensieringskrav, kan du se Lisensieringskrav [for selvbetjent tilbakestilling av passord for Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="ab763-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="ab763-123">Hvis du vil tilbakestille passordet til en bruker, kan du finne brukeren i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ab763-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="ab763-124">Klikk deretter Tilbakestill passord-knappen på oversiktsbladet for denne brukeren.</span><span class="sxs-lookup"><span data-stu-id="ab763-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="ab763-125">**Knappen for tilbakestilling av passord er nedtonet**</span><span class="sxs-lookup"><span data-stu-id="ab763-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="ab763-126">Du har ikke tillatelse til **å** tilbakestille denne brukerens passord.</span><span class="sxs-lookup"><span data-stu-id="ab763-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="ab763-127">*Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.*</span><span class="sxs-lookup"><span data-stu-id="ab763-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ab763-128">Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.</span><span class="sxs-lookup"><span data-stu-id="ab763-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="ab763-129">**Jeg ser ikke blad for tilbakestilling av passord**</span><span class="sxs-lookup"><span data-stu-id="ab763-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="ab763-130">Du har ikke tillatelse til å tilbakestille passord.</span><span class="sxs-lookup"><span data-stu-id="ab763-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="ab763-131">*Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.*</span><span class="sxs-lookup"><span data-stu-id="ab763-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ab763-132">Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.</span><span class="sxs-lookup"><span data-stu-id="ab763-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="ab763-133">**Jeg ser ikke det lokale integrasjonsbladet i tilbakestilling av passord**</span><span class="sxs-lookup"><span data-stu-id="ab763-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="ab763-134">Det lokale integreringsbladet vises bare i hybridmiljøer, det vil si at du bruker tilbakeskriving av passord til å manipulere lokale brukerpassord.</span><span class="sxs-lookup"><span data-stu-id="ab763-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="ab763-135">Du ser ikke dette bladet hvis:</span><span class="sxs-lookup"><span data-stu-id="ab763-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="ab763-136">Du bruker ikke tilbakeskriving av passord</span><span class="sxs-lookup"><span data-stu-id="ab763-136">You are not using password writeback</span></span>
  - <span data-ttu-id="ab763-137">Det er et problem med installasjon/tilkobling av passord-writeback</span><span class="sxs-lookup"><span data-stu-id="ab763-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="ab763-138">Det er et problem med installasjonen/tilkoblingen til Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="ab763-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="ab763-139">Hvis du vil ha flere feilsøkingstrinn for problemer med tilbakeskriving av passord, kan du se [Feilsøke tilbakeskriving av passord](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="ab763-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="ab763-140">**Jeg vet ikke hvordan jeg tilbakestiller passordet til en bruker**</span><span class="sxs-lookup"><span data-stu-id="ab763-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="ab763-141">Logg på Azure Portal som en passende administrator.</span><span class="sxs-lookup"><span data-stu-id="ab763-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="ab763-142">Gå til **bladbladet Brukere og** grupper, og velg Alle **brukere.**</span><span class="sxs-lookup"><span data-stu-id="ab763-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="ab763-143">Velg en bruker fra listen.</span><span class="sxs-lookup"><span data-stu-id="ab763-143">Select a user from the list.</span></span>
4. <span data-ttu-id="ab763-144">Velg Oversikt for den valgte **brukeren,** og velg deretter Tilbakestill passord på **kommandolinjen.**</span><span class="sxs-lookup"><span data-stu-id="ab763-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="ab763-145">Velg Tilbakestill **passord-knappen,** og følg instruksjonene på skjermen.</span><span class="sxs-lookup"><span data-stu-id="ab763-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="ab763-146">Bare tilbakestillinger utført gjennom **Azure Portal støtter** tilbakeskriving av passord.</span><span class="sxs-lookup"><span data-stu-id="ab763-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="ab763-147">**Jeg tilbakestiller passordet til en lokal bruker fra administrasjonsportalen for Office 365 eller mobilappen for Office 365, men brukeren kan fremdeles ikke logge på**</span><span class="sxs-lookup"><span data-stu-id="ab763-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="ab763-148">Tilbakeskriving av passord støttes ikke i denne portalen.</span><span class="sxs-lookup"><span data-stu-id="ab763-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="ab763-149">Tilbakestill brukerens passord på nytt i Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ab763-149">Reset the user's password again in the Azure portal.</span></span>
