---
title: Problemer med å utvikle programmer med APIer
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975024"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="9cdf6-102">Problemer med å utvikle programmer med APIer</span><span class="sxs-lookup"><span data-stu-id="9cdf6-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="9cdf6-103">Hvis du vil begynne å bruke Azure Active Directory Graph API, kan du se hurtigst [Art veiledning for Azure ad Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller vise den [interaktive referanse dokumentasjonen for Azure ad Graph API](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="9cdf6-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="9cdf6-104">**Slutten av støtte for Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD-graf)**</span><span class="sxs-lookup"><span data-stu-id="9cdf6-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="9cdf6-105">**Fra og med 30. juni 2020** vil vi ikke lenger legge til nye funksjoner i ADAL og Azure ad Graph.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="9cdf6-106">Vi vil fortsette å gi tekniske støtte og sikkerhets oppdateringer, men vil ikke lenger gi funksjons oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="9cdf6-107">**Fra og med 30. juni 2022** vil vi avslutte støtte for ADAL og Azure ad Graph og vil ikke lenger gi tekniske støtte eller sikkerhets oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="9cdf6-108">Apper som bruker ADAL på eksisterende OS-versjoner vil fortsatt fungere etter denne tiden, men får ingen tekniske støtte eller sikkerhets oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="9cdf6-109">Apper som bruker Azure AD Graph etter dette tidspunktet, vil kanskje ikke lenger motta svar fra Azure AD Graph-endepunktet.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="9cdf6-110">**ADAL overføring**</span><span class="sxs-lookup"><span data-stu-id="9cdf6-110">**ADAL Migration**</span></span>

<span data-ttu-id="9cdf6-111">Vi anbefaler at du oppdaterer til [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhets oppdateringene.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="9cdf6-112">Hvis du bruker Microsoft-apper, vet du at Microsoft er i ferd med å overføre sine programmer til MSAL med tids fristen for slutt på støtte, slik at de kommer til å dra nytte av MSALs kontinuerlige sikkerhets-og funksjons forbedringer.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="9cdf6-113">[Les ADAL vanlige spørsmål](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="9cdf6-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="9cdf6-114">[Lær om hvordan du overfører apper på hver enkelt plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="9cdf6-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="9cdf6-115">Hvis du trenger hjelp til å forstå hvilke av appene som bruker ADAL, anbefaler vi at du ser gjennom alle programmenes kilde kode, og hvis det er aktuelt, kan du nå ut til alle uavhengige program vare leverandører.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9cdf6-116">Microsoft kunde støtte kan også gi deg en liste over alle ikke-Microsoft-ADAL-apper i leieren din.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="9cdf6-117">**Overføring av AAD-graf**</span><span class="sxs-lookup"><span data-stu-id="9cdf6-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="9cdf6-118">For programmer som bruker Azure AD Graph, følger du veiledningen vår for å overføre [apper i Azure ad Graph til Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="9cdf6-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="9cdf6-119">[Overførings sjekk listen vår gir et komme i gang-punkt](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="9cdf6-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="9cdf6-120">Registrerings portalen for Azure-apper viser hvilke programmer som bruker AAD-graf.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="9cdf6-121">Vi anbefaler at du ser gjennom alle appenes kilde kode, og hvis det er aktuelt, kan du nå ut til alle uavhengige program vare leverandører.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9cdf6-122">Microsoft kunde støtte kan også gi deg en liste over all bruk av AAD-graf i leieren din.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="9cdf6-123">Brukeren eller administratoren må gi den riktige tillatelsene via en samtykke prosess for at appen skal få tilgang til data i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="9cdf6-124">[Referansen Microsoft Graph-tillatelser](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) viser tillatelsene som er tilknyttet hvert hoved sett med Microsoft Graph-APIer.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="9cdf6-125">Den gir deg også veiledning om hvordan du bruker tillatelsene.</span><span class="sxs-lookup"><span data-stu-id="9cdf6-125">It also provides guidance about how to use the permissions.</span></span>
