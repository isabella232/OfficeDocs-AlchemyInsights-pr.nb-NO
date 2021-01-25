---
title: Problemer med å utvikle programmer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974761"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="d144b-102">Problemer med å utvikle programmer</span><span class="sxs-lookup"><span data-stu-id="d144b-102">Issues developing applications</span></span>

<span data-ttu-id="d144b-103">Hvis du vil feilsøke de vanligste problemene ved bygging av Azure Active Directory-apper (AD), kan du se følgende artikler:</span><span class="sxs-lookup"><span data-stu-id="d144b-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="d144b-104">Jeg har problemer med å logge deg på programmet (ene) ved bruk av Chrome-leser</span><span class="sxs-lookup"><span data-stu-id="d144b-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="d144b-105">Jeg vet ikke hvordan du endrer standard verdien for leve tiden for token for programmet</span><span class="sxs-lookup"><span data-stu-id="d144b-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="d144b-106">Jeg er forvirret om hvordan program samtykke fungerer</span><span class="sxs-lookup"><span data-stu-id="d144b-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="d144b-107">Jeg vet ikke hvordan jeg gir tillatelser til programmet mitt</span><span class="sxs-lookup"><span data-stu-id="d144b-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="d144b-108">Jeg forstår ikke forskjellen mellom delegerte og applikasjons tillatelser</span><span class="sxs-lookup"><span data-stu-id="d144b-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="d144b-109">\***Slutten av støtte for Azure Active Directory Authentication Library (ADAL) og Azure ad Graph API (AAD-graf)** _</span><span class="sxs-lookup"><span data-stu-id="d144b-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="d144b-110">Fra og med 30. juni 2020 vil vi ikke lenger legge til nye funksjoner i Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD-graf).</span><span class="sxs-lookup"><span data-stu-id="d144b-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="d144b-111">Vi vil fortsette å gi tekniske støtte og sikkerhets oppdateringer, men vil ikke lenger gi funksjons oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="d144b-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="d144b-112">Fra og med 30. juni 2022 vil vi avslutte støtte for ADAL og AAD-graf og vil ikke lenger gi tekniske støtte eller sikkerhets oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="d144b-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="d144b-113">Som følge av denne situasjonen er følgende implikasjoner:</span><span class="sxs-lookup"><span data-stu-id="d144b-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="d144b-114">Apper som bruker ADAL på eksisterende OS-versjoner vil fortsatt fungere etter denne tiden, men får ingen tekniske støtte eller sikkerhets oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="d144b-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="d144b-115">Apper som bruker AAD Graph etter dette tidspunktet vil kanskje ikke lenger motta svar fra ende punktet til AAD-Graph</span><span class="sxs-lookup"><span data-stu-id="d144b-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="d144b-116">_ *ADAL-overføring*\*</span><span class="sxs-lookup"><span data-stu-id="d144b-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="d144b-117">Hvis du bruker Microsoft-apper, anbefaler vi at du oppdaterer til Microsoft Authentication Library (MSAL), som har de nyeste funksjonene og sikkerhets oppdateringene.</span><span class="sxs-lookup"><span data-stu-id="d144b-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="d144b-118">Denne anbefalingen er i konteksten til Microsoft som starter prosessen med å overføre sine apper til MSAL av tids fristen for slutt på støtte.</span><span class="sxs-lookup"><span data-stu-id="d144b-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="d144b-119">Overføringen av Microsoft-appene til MSAL sikrer at appene drar nytte av MSALs kontinuerlige sikkerhets-og funksjons forbedringer.</span><span class="sxs-lookup"><span data-stu-id="d144b-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="d144b-120">Les ADAL vanlige spørsmål</span><span class="sxs-lookup"><span data-stu-id="d144b-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="d144b-121">Lær om hvordan du overfører apper på en per-plattform-basis</span><span class="sxs-lookup"><span data-stu-id="d144b-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="d144b-122">Hvis du trenger hjelp til å forstå hvilke av appene dine som bruker ADAL, anbefaler vi at du ser gjennom alle appenes kilde kode og, hvis det er aktuelt, nå ut til alle uavhengige program vare leverandører (ISV-er) eller program leverandører.</span><span class="sxs-lookup"><span data-stu-id="d144b-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="d144b-123">Microsoft kunde støtte kan også gi deg en liste over alle ikke-Microsoft-ADAL-apper i leieren din.</span><span class="sxs-lookup"><span data-stu-id="d144b-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="d144b-124">**Overføring av AAD-graf**</span><span class="sxs-lookup"><span data-stu-id="d144b-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="d144b-125">For programmer som bruker AAD-grafen, følger du veiledningen vår for å overføre apper for AAD-graf til Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="d144b-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="d144b-126">[Overførings sjekk listen vår gir et komme i gang-punkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="d144b-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="d144b-127">Registrerings portalen for Azure-apper viser hvilke programmer som bruker AAD-graf.</span><span class="sxs-lookup"><span data-stu-id="d144b-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="d144b-128">Vi anbefaler at du ser gjennom alle appenes kilde kode, og når det er aktuelt, nå til alle uavhengige program vare leverandører (ISV) eller program leverandører.</span><span class="sxs-lookup"><span data-stu-id="d144b-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="d144b-129">Microsoft kunde støtte kan også gi deg informasjon om AAD Graph-bruk i leieren din.</span><span class="sxs-lookup"><span data-stu-id="d144b-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







