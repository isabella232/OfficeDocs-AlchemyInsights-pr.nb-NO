---
title: Opprette en organisasjonsrelasjon for å la brukerne samarbeide med en annen organisasjon
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
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816137"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="04ddf-102">Opprette en organisasjonsrelasjon for å la brukerne samarbeide med en annen organisasjon</span><span class="sxs-lookup"><span data-stu-id="04ddf-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="04ddf-103">Gå til **Administrator** > **Exchange** fra instrumentbordet i administrasjonssenteret for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="04ddf-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="04ddf-104">Gå til **organisasjon** > **deling**.</span><span class="sxs-lookup"><span data-stu-id="04ddf-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="04ddf-105">Klikk på **Ny** under **Organisasjonsdeling**-</span><span class="sxs-lookup"><span data-stu-id="04ddf-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="04ddf-106">Skriv inn et egendefinert navn for organisasjonsrelasjonen i **Relasjonsnavn**-boksen i **ny organisasjonsrelasjon**.</span><span class="sxs-lookup"><span data-stu-id="04ddf-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="04ddf-107">Skriv inn domenet for den eksterne Office 365- eller lokale Exchange-organisasjonen du vil at skal se kalenderne i **Domener å dele med**-boksen.</span><span class="sxs-lookup"><span data-stu-id="04ddf-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="04ddf-108">Hvis du trenger å skrive inn mer enn ett domene, skill domenenavnene med et komma.</span><span class="sxs-lookup"><span data-stu-id="04ddf-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="04ddf-109">For eksempel contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="04ddf-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="04ddf-110">Merk av for **Aktiver deling av informasjon om ledig/opptatt i kalenderen** for å slå på kalenderdeling med domenene du har oppført.</span><span class="sxs-lookup"><span data-stu-id="04ddf-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="04ddf-111">Angi delingsnivå for informasjon om ledig/opptatt i kalenderen, og angi hvilke brukere som kan dele informasjon om ledig/opptatt i kalenderen.</span><span class="sxs-lookup"><span data-stu-id="04ddf-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="04ddf-112">For å angi informasjon om ledig/opptatt velger du ett av følgende:</span><span class="sxs-lookup"><span data-stu-id="04ddf-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="04ddf-113">**Informasjon om ledig/opptatt i kalenderen bare med tidspunkt**</span><span class="sxs-lookup"><span data-stu-id="04ddf-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="04ddf-114">**Ledig/opptatt i kalenderen med tidspunkt, emne og sted**</span><span class="sxs-lookup"><span data-stu-id="04ddf-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="04ddf-115">For å angi hvilke brukere som skal dele informasjon om ledig/opptatt, velger du ett av følgende:</span><span class="sxs-lookup"><span data-stu-id="04ddf-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="04ddf-116">**Alle i organisasjonen**</span><span class="sxs-lookup"><span data-stu-id="04ddf-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="04ddf-117">**En angitt sikkerhetsgruppe**</span><span class="sxs-lookup"><span data-stu-id="04ddf-117">**A specified security group**</span></span>  

<span data-ttu-id="04ddf-118">Klikk på **bla gjennom** for å velge sikkerhetsgruppen fra en liste, og klikk deretter på **ok**.</span><span class="sxs-lookup"><span data-stu-id="04ddf-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="04ddf-119">Klikk på **lagre** for å opprette organisasjonsrelasjonen.</span><span class="sxs-lookup"><span data-stu-id="04ddf-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="04ddf-120">**Obs!** Konfigurasjoner på tvers av leiere støtter ikke personlige kontakter for ledig/oppdatt-oppslag.</span><span class="sxs-lookup"><span data-stu-id="04ddf-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="04ddf-121">Kontakter må inkluderes i den global adresselisten for ledig/opptatt-oppslag for å fungere.</span><span class="sxs-lookup"><span data-stu-id="04ddf-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="04ddf-122">**For full forståelse av dette emnet kan du lese:**</span><span class="sxs-lookup"><span data-stu-id="04ddf-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="04ddf-123">Opprette en organisasjonsrelasjon i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="04ddf-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="04ddf-124">Endre en organisasjonsrelasjon i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="04ddf-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="04ddf-125">Fjerne en organisasjonsrelasjon i Exchange Online</span><span class="sxs-lookup"><span data-stu-id="04ddf-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
