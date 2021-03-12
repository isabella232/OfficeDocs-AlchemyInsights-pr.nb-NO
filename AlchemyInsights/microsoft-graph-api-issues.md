---
title: Problemer med Microsoft Graph API
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714154"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="c62dc-102">Problemer med Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="c62dc-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="c62dc-103">Dette emnet kan også gjelde for utviklere som fremdeles bruker Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="c62dc-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="c62dc-104">Det anbefales imidlertid på **det sterkeste** at du bruker Microsoft Graph for alle scenariene for katalog-, identitets- og tilgangsbehandling.</span><span class="sxs-lookup"><span data-stu-id="c62dc-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="c62dc-105">**Godkjennings- eller godkjenningsproblemer**</span><span class="sxs-lookup"><span data-stu-id="c62dc-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="c62dc-106">Hvis appen ikke kan skaffe **tokener** til å ringe Microsoft Graph, kan du velge Problem med å få et tilgangstoken **(godkjenning)** Microsoft Graph-kategori for å få mer spesifikk hjelp og støtte for dette emnet.</span><span class="sxs-lookup"><span data-stu-id="c62dc-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="c62dc-107">Hvis appen mottar **401-** eller 403-godkjenningsfeil når du ringer Microsoft Graph, kan du velge feilmeldingen Får ingen tilgang **(Authorization)** Microsoft Graph API for å få mer spesifikk hjelp og støtte for dette emnet.</span><span class="sxs-lookup"><span data-stu-id="c62dc-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="c62dc-108">**Jeg vil bruke Microsoft Graph, men er ikke sikker på hvor jeg skal begynne**</span><span class="sxs-lookup"><span data-stu-id="c62dc-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="c62dc-109">Oversikt over Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c62dc-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="c62dc-110">Oversikt over identitets- og tilgangsbehandling i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c62dc-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="c62dc-111">Komme i gang med å bygge Microsoft Graph-apper</span><span class="sxs-lookup"><span data-stu-id="c62dc-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="c62dc-112">**Microsoft Graph Explorer** – test Microsoft Graph API-er i tenanten din eller en demo-tenant</span><span class="sxs-lookup"><span data-stu-id="c62dc-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="c62dc-113">**Jeg vil bruke Microsoft Graph, men støtter det API-ene for v1.0-katalogen jeg trenger?**</span><span class="sxs-lookup"><span data-stu-id="c62dc-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="c62dc-114">Microsoft Graph er det anbefalte API-et for katalog-, identitets- og tilgangsbehandling.</span><span class="sxs-lookup"><span data-stu-id="c62dc-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="c62dc-115">Det er imidlertid fortsatt noen hull mellom det som er mulig i Azure AD Graph og Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c62dc-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="c62dc-116">Se gjennom følgende artikler, som fremhever de mest oppdaterte forskjellene som kan hjelpe deg med valget ditt:</span><span class="sxs-lookup"><span data-stu-id="c62dc-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="c62dc-117">Forskjeller på ressurstypen mellom Azure AD Graph og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c62dc-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="c62dc-118">Egenskapsforskjeller mellom Azure AD Graph og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c62dc-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="c62dc-119">Metodeforskjeller mellom Azure AD og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c62dc-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="c62dc-120">**API-en jeg ringer, fungerer ikke – hvor kan jeg teste mer?**</span><span class="sxs-lookup"><span data-stu-id="c62dc-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="c62dc-121">**Microsoft Graph Explorer** – test Microsoft Graph API-er i tenanten din eller en demo-leier, og sjekk også ut eksempelspørringene **i** Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="c62dc-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="c62dc-122">**Appen min er for treg og blir også begrensning. Hvilke forbedringer kan jeg gjøre?**</span><span class="sxs-lookup"><span data-stu-id="c62dc-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="c62dc-123">Avhengig av scenarioet finnes det en rekke alternativer du kan velge mellom for å gjøre programmet mer velfellerende, og i noen tilfeller mindre utsatt for å bli begrensning av tjenesten (når du foretar for mange anrop).</span><span class="sxs-lookup"><span data-stu-id="c62dc-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="c62dc-124">Anbefalte fremgangsmåter for Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c62dc-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="c62dc-125">Grupperingsforespørsler</span><span class="sxs-lookup"><span data-stu-id="c62dc-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="c62dc-126">Spore endringer gjennom delta-spørring</span><span class="sxs-lookup"><span data-stu-id="c62dc-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="c62dc-127">Bli varslet om endringer via webhooks</span><span class="sxs-lookup"><span data-stu-id="c62dc-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="c62dc-128">Begrensningsveiledning</span><span class="sxs-lookup"><span data-stu-id="c62dc-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="c62dc-129">**Hvor finner jeg mer informasjon om feil og kjente problemer?**</span><span class="sxs-lookup"><span data-stu-id="c62dc-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="c62dc-130">Informasjon om feilsvar i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c62dc-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="c62dc-131">Kjente problemer med Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c62dc-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="c62dc-132">**Hvor kan jeg kontrollere statusen for tjenestetilgjengelighet og tilkobling?**</span><span class="sxs-lookup"><span data-stu-id="c62dc-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="c62dc-133">Tjenestetilgjengeligheten og tilkoblingen til de underliggende tjenestene som kan nås via Microsoft Graph, kan påvirke den generelle tilgjengeligheten og ytelsen til Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c62dc-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="c62dc-134">For tjenestetilstand for Azure Active Directory kontrollerer du statusen for **tjenester for** sikkerhet og identitet som er oppført på [statussiden for Azure.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="c62dc-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="c62dc-135">Når det gjelder Office-tjenester som bidrar til Microsoft Graph, kan du kontrollere statusen for tjenester som er oppført i instrumentbordet for [tjenestetilstand.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="c62dc-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="c62dc-136">Godkjenningsfeil i Microsoft Graph kan skyldes flere forskjellige problemer, og de fleste genererer en 401- eller 403-feil.</span><span class="sxs-lookup"><span data-stu-id="c62dc-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="c62dc-137">Følgende kan for eksempel føre til autorisasjonsfeil:</span><span class="sxs-lookup"><span data-stu-id="c62dc-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="c62dc-138">Feil [innhentingsflyter for tilgangstoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="c62dc-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="c62dc-139">Dårlig konfigurerte [tillatelsesområder](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="c62dc-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="c62dc-140">Mangel på [samtykke](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="c62dc-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="c62dc-141">\**_Avvikling av kundestøtte for godkjenningsbiblioteket for Azure Active Directory (ADAL) og Azure AD Graph-API-en (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="c62dc-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="c62dc-142">_\*Fra og med 30. juni 2020\*\*, vil vi ikke lenger legge til nye funksjoner i ADAL og Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="c62dc-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="c62dc-143">Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.</span><span class="sxs-lookup"><span data-stu-id="c62dc-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="c62dc-144">**Fra og med 30. juni 2022** avslutter vi støtten for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.</span><span class="sxs-lookup"><span data-stu-id="c62dc-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="c62dc-145">Apper som bruker ADAL på eksisterende OS-versjoner, vil fortsette å fungere etter dette tid, men vil ikke få noen teknisk støtte *eller sikkerhetsoppdateringer.*</span><span class="sxs-lookup"><span data-stu-id="c62dc-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="c62dc-146">Apper som bruker Azure AD Graph etter dette tid, kan ikke lenger motta svar fra Azure AD Graph-endepunktet.</span><span class="sxs-lookup"><span data-stu-id="c62dc-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="c62dc-147">**ADAL-overføring**</span><span class="sxs-lookup"><span data-stu-id="c62dc-147">**ADAL Migration**</span></span>

<span data-ttu-id="c62dc-148">Vi anbefaler at du oppdaterer til [Microsofts godkjenningbibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhetsoppdateringene.</span><span class="sxs-lookup"><span data-stu-id="c62dc-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="c62dc-149">Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre programmene til MSAL innen tidsfristen for slutten av støtten, slik at de vil dra nytte av MSALs pågående sikkerhets- og funksjonsforbedringer.</span><span class="sxs-lookup"><span data-stu-id="c62dc-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="c62dc-150">Les Vanlige spørsmål om ADAL</span><span class="sxs-lookup"><span data-stu-id="c62dc-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="c62dc-151">Finn ut hvordan du overfører apper per plattform</span><span class="sxs-lookup"><span data-stu-id="c62dc-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="c62dc-152">Hvis du trenger hjelp til å forstå hvilke apper som bruker ADAL, anbefaler vi at du går gjennom alle appenes kildekode, og hvis aktuelt, kan du ta kontakt med eventuelle ISV-er eller appleverandører.</span><span class="sxs-lookup"><span data-stu-id="c62dc-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="c62dc-153">Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c62dc-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="c62dc-154">**AAD Graph-overføring**</span><span class="sxs-lookup"><span data-stu-id="c62dc-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="c62dc-155">For programmer som bruker Azure AD Graph, følger du veiledningen vår for [å overføre Azure AD Graph-apper til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="c62dc-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="c62dc-156">[Sjekklisten for overføring gir et utgangspunkt for å komme i gang](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="c62dc-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="c62dc-157">Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="c62dc-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="c62dc-158">Vi anbefaler at du ser gjennom kildekoden for alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør.</span><span class="sxs-lookup"><span data-stu-id="c62dc-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="c62dc-159">Microsoft Kundestøtte kan også gi deg en liste over all AAD Graph-bruk i tenanten din.</span><span class="sxs-lookup"><span data-stu-id="c62dc-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="c62dc-160">Brukeren eller administratoren må gi appen de riktige tillatelsene via en samtykkeprosess for at appen skal få tilgang til data i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c62dc-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="c62dc-161">[Tillatelsesreferansen for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) viser tillatelsene som er knyttet til hvert hovedsett av Microsoft Graph API-er.</span><span class="sxs-lookup"><span data-stu-id="c62dc-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="c62dc-162">Den gir også veiledning om hvordan du bruker tillatelsene.</span><span class="sxs-lookup"><span data-stu-id="c62dc-162">It also provides guidance about how to use the permissions.</span></span>
