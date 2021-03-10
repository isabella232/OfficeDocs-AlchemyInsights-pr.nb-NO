---
title: Problem med tilbakestilling av passord
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696272"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="e3cd6-102">Problemer med å tilbakestille passord</span><span class="sxs-lookup"><span data-stu-id="e3cd6-102">Problems resetting password</span></span>

<span data-ttu-id="e3cd6-103">Nedenfor finner du noen av problemene du kan møte på når du tilbakestiller passord og mulige løsninger:</span><span class="sxs-lookup"><span data-stu-id="e3cd6-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="e3cd6-104">**Jeg har et problem med tilbakestilling av passord, som ikke dekkes i de andre kategoriene**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="e3cd6-105">Kontroller at du er autorisert til å tilbakestille passord.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="e3cd6-106">Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="e3cd6-107">Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="e3cd6-108">Kontroller at du forstår lisensieringskravene:</span><span class="sxs-lookup"><span data-stu-id="e3cd6-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="e3cd6-109">Du må ha minst én lisens tilordnet i organisasjonen</span><span class="sxs-lookup"><span data-stu-id="e3cd6-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="e3cd6-110">Bare skybrukere – alle Office 365 (O365) betalte SKU-er, eller Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="e3cd6-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="e3cd6-111">Skybrukere og/eller lokale brukere – Azure AD Premium P1 eller P2, Enterprise Mobility + Security (EMS) eller Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="e3cd6-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="e3cd6-112">Hvis du vil lese mer om lisensieringskrav, kan du se artikkelen Lisensieringskrav [for selvbetjent tilbakestilling av](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)passord for Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="e3cd6-113">**Jeg har problemer med å teste policyen for tilbakestilling av passord jeg har angitt**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="e3cd6-114">Det kan ta flere minutter å replikere nylig brukte policyer på tvers av alle datasentre og sluttpunkter.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="e3cd6-115">Fysisk avstand fra datasenteret påvirker også hvor raskt endringer brukes.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="e3cd6-116">Test med en sluttbruker, ikke en administrator, og pilot med et lite sett med brukere.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="e3cd6-117">Policyene som er konfigurert i Azure Portal, gjelder BARE for sluttbrukere, ikke administratorer.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="e3cd6-118">Microsoft håndhever en sterk policy for tilbakestilling av passord med to porter for en hvilken som helst Azure-administratorrolle (eksempel: Global administrator, Brukerstøtteadministrator, passordadministrator osv.)</span><span class="sxs-lookup"><span data-stu-id="e3cd6-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="e3cd6-119">Lær mer om [policyer for administratorer.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="e3cd6-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="e3cd6-120">**Jeg ønsker å distribuere tilbakestilling av passord, men jeg ønsker ikke at brukerne mine skal registrere mer sikkerhetsinformasjon**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="e3cd6-121">Forhåndsutmuler data for brukerne, slik at de ikke trenger å gjøre det!</span><span class="sxs-lookup"><span data-stu-id="e3cd6-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="e3cd6-122">– Som administrator kan du angi telefon- og e-postegenskaper for brukerne før du ruller ut tilbakestilling av passord til organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="e3cd6-123">Du kan gjøre dette ved hjelp av en API, PowerShell eller Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="e3cd6-124">Mer informasjon her:</span><span class="sxs-lookup"><span data-stu-id="e3cd6-124">More information here:</span></span>
- [<span data-ttu-id="e3cd6-125">Distribuere tilbakestilling av passord uten at brukere må registrere seg</span><span class="sxs-lookup"><span data-stu-id="e3cd6-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="e3cd6-126">Hvilke data som brukes av tilbakestilling av passord</span><span class="sxs-lookup"><span data-stu-id="e3cd6-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="e3cd6-127">**Knappen for tilbakestilling av passord er nedtonet**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="e3cd6-128">Du har ikke tillatelse til å tilbakestille denne brukerens passord.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="e3cd6-129">Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="e3cd6-130">Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="e3cd6-131">**Jeg ser ikke blad for tilbakestilling av passord**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="e3cd6-132">Du har ikke tillatelse til å tilbakestille passord.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="e3cd6-133">Bare globale passord og brukeradministratorer kan tilbakestille brukerpassord.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="e3cd6-134">Globale administratorer kan også tilbakestille passordene til andre privilegerte administratorer.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="e3cd6-135">**Jeg ser ikke det lokale integrasjonsbladet i tilbakestilling av passord**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="e3cd6-136">Det lokale integreringsbladet vises bare i hybridmiljøer, det vil si at du bruker tilbakeskriving av passord til å manipulere lokale brukerpassord.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="e3cd6-137">Du ser ikke dette bladet hvis:</span><span class="sxs-lookup"><span data-stu-id="e3cd6-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="e3cd6-138">Du bruker ikke tilbakeskriving av passord</span><span class="sxs-lookup"><span data-stu-id="e3cd6-138">You are not using password writeback</span></span>
    - <span data-ttu-id="e3cd6-139">Det er et problem med installasjon/tilkobling av passord-writeback</span><span class="sxs-lookup"><span data-stu-id="e3cd6-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="e3cd6-140">Det er et problem med installasjonen/tilkoblingen til Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e3cd6-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="e3cd6-141">Hvis du vil ha flere feilsøkingstrinn for problemer med tilbakeskriving av passord, kan du se delen [Feilsøke passordskriving](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="e3cd6-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="e3cd6-142">**Jeg vet ikke hvordan jeg tilbakestiller passordet til en bruker**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="e3cd6-143">Logg på Azure Portal som en passende administrator.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="e3cd6-144">Gå til bladbladet Brukere og grupper, og velg **Alle brukere.**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="e3cd6-145">Velg en bruker fra listen.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-145">Select a user from the list.</span></span>
1. <span data-ttu-id="e3cd6-146">Velg Oversikt for den valgte **brukeren,** og klikk deretter Tilbakestill passord på **kommandolinjen.**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="e3cd6-147">Følg instruksjonene på skjermen.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="e3cd6-148">Bare tilbakestillinger utført gjennom Azure Portal støtter tilbakeskriving av passord.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="e3cd6-149">**Jeg tilbakestiller passordet til en lokal bruker fra administrasjonsportalen for Office 365 eller mobilappen for Office 365, men brukeren kan fremdeles ikke logge på**</span><span class="sxs-lookup"><span data-stu-id="e3cd6-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="e3cd6-150">Tilbakeskriving av passord støttes ikke i denne portalen.</span><span class="sxs-lookup"><span data-stu-id="e3cd6-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="e3cd6-151">Tilbakestill brukerens passord på nytt i Azure Portal – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="e3cd6-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

