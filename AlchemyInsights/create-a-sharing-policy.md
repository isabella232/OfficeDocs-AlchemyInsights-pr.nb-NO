---
title: Opprette en delingspolicy for å tillate brukerne å dele kalenderen med personer utenfor organisasjonen
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
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816281"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="14a8a-102">Opprette en delingspolicy for å tillate brukerne å dele kalenderen med personer utenfor organisasjonen</span><span class="sxs-lookup"><span data-stu-id="14a8a-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="14a8a-103">Gå til **Administrator** > **Exchange** fra instrumentbordet i administrasjonssenteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="14a8a-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="14a8a-104">Gå til **organisasjon** > **deling**.</span><span class="sxs-lookup"><span data-stu-id="14a8a-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="14a8a-105">Klikk på **Ny** i listevisning under **Individuell deling**.</span><span class="sxs-lookup"><span data-stu-id="14a8a-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="14a8a-106">Skriv inn et egendefinert navn for delingspolicyen i **policynavn**-boksen i **ny delingspolicy**.</span><span class="sxs-lookup"><span data-stu-id="14a8a-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="14a8a-107">Klikk på **Legg til** for å definere delingsregler for policyen.</span><span class="sxs-lookup"><span data-stu-id="14a8a-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="14a8a-108">Velg ett av følgende alternativer i **delingsregel**, for å angi domenene du vil dele med:</span><span class="sxs-lookup"><span data-stu-id="14a8a-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="14a8a-109">**Dele med alle domener**</span><span class="sxs-lookup"><span data-stu-id="14a8a-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="14a8a-110">**Dele med et bestemt domene**</span><span class="sxs-lookup"><span data-stu-id="14a8a-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="14a8a-111">Hvis du velger **Dele med et bestemt domene**, skriver du inn navnet på domenet du vil dele med.</span><span class="sxs-lookup"><span data-stu-id="14a8a-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="14a8a-112">Hvis du trenger å skrive inn mer enn ett domene for denne delingspolicyen, lagrer du innstillingene for det første domenet, og redigerer deretter delingsreglene for å legge til flere domener.</span><span class="sxs-lookup"><span data-stu-id="14a8a-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="14a8a-113">Hvis du vil angi informasjonen som kan deles, merker du av for **Del kalendermappe**, og velger deretter ett av følgende alternativer:</span><span class="sxs-lookup"><span data-stu-id="14a8a-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="14a8a-114">**Informasjon om ledig/opptatt i kalenderen bare med tidspunkt**</span><span class="sxs-lookup"><span data-stu-id="14a8a-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="14a8a-115">**Informasjon om ledig/opptatt i kalenderen med tidspunkt, emne og sted**</span><span class="sxs-lookup"><span data-stu-id="14a8a-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="14a8a-116">**All avtaleinformasjon i kalenderen, inkludert tidspunkt, emne, sted og tittel**</span><span class="sxs-lookup"><span data-stu-id="14a8a-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="14a8a-117">Klikk på **lagre** for å angi reglene i delingspolicyen.</span><span class="sxs-lookup"><span data-stu-id="14a8a-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="14a8a-118">Hvis du vil angi denne delingspolicyen som den nye standard delingspolicyen for alle brukerne i organisasjonen, merker du av for **Gjør denne policyen til standard delingspolicy**.</span><span class="sxs-lookup"><span data-stu-id="14a8a-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="14a8a-119">Klikk på **lagre** for å opprette delingspolicyen.</span><span class="sxs-lookup"><span data-stu-id="14a8a-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="14a8a-120">**For full forståelse av dette emnet kan du lese:**</span><span class="sxs-lookup"><span data-stu-id="14a8a-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="14a8a-121">Opprette en delingspolicy i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="14a8a-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="14a8a-122">Bruke en delingspolicy på postbokser i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="14a8a-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="14a8a-123">Endre, deaktivere eller fjerne en delingspolicy i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="14a8a-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)