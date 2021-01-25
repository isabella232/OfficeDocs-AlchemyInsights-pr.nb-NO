---
title: Spørre etter Microsoft Graph API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974424"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="271cf-102">Spørre etter Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="271cf-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="271cf-103">Dette emnet kan også gjelde for utviklere som fremdeles bruker Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="271cf-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="271cf-104">Det anbefales imidlertid på det **sterkeste** at du bruker Microsoft Graph for alle dine katalog-, identitets-og tilgangs behandlings scenarioer.</span><span class="sxs-lookup"><span data-stu-id="271cf-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="271cf-105">**Problemer med godkjenning eller autorisasjon**</span><span class="sxs-lookup"><span data-stu-id="271cf-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="271cf-106">Hvis appen **ikke kan hente tokener** for å ringe Microsoft Graph, velger du **problem med å få en tilgangs kode (Authentication)** Microsoft Graph-kategori for å få mer spesifikk hjelp og støtte på dette emnet.</span><span class="sxs-lookup"><span data-stu-id="271cf-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="271cf-107">Hvis appen **mottar godkjennings feil for 401 eller 403** når du ringer til Microsoft Graph, velger du avmerkings boksen få tilgang til å få **tilgangen nektes (godkjenning)** Microsoft Graph API-kategori for å få mer spesifikk hjelp og støtte på dette emnet.</span><span class="sxs-lookup"><span data-stu-id="271cf-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="271cf-108">**Jeg vil bruke Microsoft Graph, men ikke sikker på hvor du skal begynne**</span><span class="sxs-lookup"><span data-stu-id="271cf-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="271cf-109">Hvis du vil lære mer om Microsoft Graph, kan du se:</span><span class="sxs-lookup"><span data-stu-id="271cf-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="271cf-110">Oversikt over Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="271cf-111">Oversikt over identitets-og tilgangs behandling i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="271cf-112">Komme i gang med å bygge Microsoft Graph-apper</span><span class="sxs-lookup"><span data-stu-id="271cf-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="271cf-113">**Microsoft Graph Explorer** – test Microsoft Graph-APIer i leieren eller en demonstrasjons leier</span><span class="sxs-lookup"><span data-stu-id="271cf-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="271cf-114">**Jeg vil bruke Microsoft Graph, men har den støtte for v 1.0-katalog-APIene jeg trenger?**</span><span class="sxs-lookup"><span data-stu-id="271cf-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="271cf-115">Microsoft Graph er den anbefalte APIEN for katalog, identitet og tilgangs behandling.</span><span class="sxs-lookup"><span data-stu-id="271cf-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="271cf-116">Det finnes imidlertid fremdeles noen tomrom mellom hva som er mulig i Azure AD Graph og Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="271cf-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="271cf-117">Se gjennom følgende artikler, som uthever de mest oppdaterte forskjellene for å hjelpe deg med det du velger:</span><span class="sxs-lookup"><span data-stu-id="271cf-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="271cf-118">Ressurs type forskjeller mellom Azure AD Graph og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="271cf-119">Egenskaps forskjeller mellom Azure AD Graph og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="271cf-120">Metode forskjeller mellom Azure AD og Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="271cf-121">**Når jeg spør etter *bruker* objektet, mangler mange av egenskapene**</span><span class="sxs-lookup"><span data-stu-id="271cf-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="271cf-122">`GET https://graph.microsoft.com/v1.0/users` returnerer bare 11 egenskaper, som Microsoft Graph automatisk velger et standard sett med *bruker* egenskaper som skal returneres.</span><span class="sxs-lookup"><span data-stu-id="271cf-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="271cf-123">Hvis du trenger andre *bruker* egenskaper, kan du bruke $SELECT til å velge hvilke egenskaper programmet trenger.</span><span class="sxs-lookup"><span data-stu-id="271cf-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="271cf-124">Prøv det i **Microsoft Graph Explorer** først.</span><span class="sxs-lookup"><span data-stu-id="271cf-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="271cf-125">**Noen bruker egenskaps verdier er *null* selv om at de er angitt**</span><span class="sxs-lookup"><span data-stu-id="271cf-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="271cf-126">Den mest sannsynlige forklaringen er at programmet har fått tillatelsen *User. ReadBasic. all* -tillatelse.</span><span class="sxs-lookup"><span data-stu-id="271cf-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="271cf-127">Dette gjør at programmet kan lese et begrenset sett med bruker egenskaper, og returnere alle andre egenskaper som null selv om de er angitt tidligere.</span><span class="sxs-lookup"><span data-stu-id="271cf-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="271cf-128">Prøv å gi program *brukeren. read. all* -tilgang i stedet.</span><span class="sxs-lookup"><span data-stu-id="271cf-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="271cf-129">Hvis du vil ha mer informasjon, kan du se [bruker tillatelser for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="271cf-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="271cf-130">**Jeg har problemer med å bruke spørrings parametere for OData til å filtrere data i mine forespørsler**</span><span class="sxs-lookup"><span data-stu-id="271cf-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="271cf-131">Selv om Microsoft Graph støtter en rekke spørrings parametere for OData, støttes ikke mange av disse parameterne fullt ut av katalog tjenester (ressurser som arver fra *directoryObject*) i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="271cf-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="271cf-132">De samme begrensningene som fantes i Azure AD Graph, vedvarer for den meste parten i Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="271cf-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="271cf-133">**Støttes ikke**: $count, $search og $filter på *null* eller *not null* -verdier</span><span class="sxs-lookup"><span data-stu-id="271cf-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="271cf-134">**Støttes ikke**: $filter på bestemte egenskaper (se ressurs emner som kan filtreres på)</span><span class="sxs-lookup"><span data-stu-id="271cf-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="271cf-135">**Støttes ikke**: side veksling, filtrering og sortering på samme tid</span><span class="sxs-lookup"><span data-stu-id="271cf-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="271cf-136">**Støttes ikke**: filtrere på en relasjon.</span><span class="sxs-lookup"><span data-stu-id="271cf-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="271cf-137">For eksempel finner du alle medlemmer av gruppen ingeniør som er i Storbritannia.</span><span class="sxs-lookup"><span data-stu-id="271cf-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="271cf-138">**Delvis støtte**: $OrderBy på *bruker* (bare DisplayName og userPrincipalName) og *gruppe*</span><span class="sxs-lookup"><span data-stu-id="271cf-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="271cf-139">**Del støtte**: $filter (støtter bare *EQ*, *startswith* *eller* *, og* *begrenset)* støtte, $Expand (utvidelse av ett objekts relasjoner returnerer alle relasjoner, men å utvide en samling av objekt relasjoner er begrenset)</span><span class="sxs-lookup"><span data-stu-id="271cf-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="271cf-140">Hvis du vil ha mer informasjon, kan du se [tilpasse svar med spørrings parametere](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="271cf-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="271cf-141">**APIEN jeg ringer til, fungerer ikke – hvor kan jeg gjøre flere tester?**</span><span class="sxs-lookup"><span data-stu-id="271cf-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="271cf-142">**Microsoft Graph Explorer** – test Microsoft Graph-APIene i leieren eller en demonstrasjons leier, og sjekk ut **utvalgs spørringene** i Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="271cf-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="271cf-143">**Når jeg spør etter data det ser ut til at jeg får et ufullstendig data sett tilbake**</span><span class="sxs-lookup"><span data-stu-id="271cf-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="271cf-144">Hvis du spør på en samling (for eksempel *brukere*), bruker Microsoft Graph side grenser for serverside, slik at resultatene alltid returneres med en standard side størrelse.</span><span class="sxs-lookup"><span data-stu-id="271cf-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="271cf-145">Appen skal alltid vente på å bla gjennom samlinger som returneres fra tjenesten.</span><span class="sxs-lookup"><span data-stu-id="271cf-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="271cf-146">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="271cf-146">For more information, see:</span></span>

- [<span data-ttu-id="271cf-147">Beste Fremgangs måter i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="271cf-148">Bla etter Microsoft Graph-data i appen</span><span class="sxs-lookup"><span data-stu-id="271cf-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="271cf-149">**Appen min er for langsomt og blir også begrenset. Hvilke forbedringer kan jeg gjøre?**</span><span class="sxs-lookup"><span data-stu-id="271cf-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="271cf-150">Avhengig av scenariet, er det en rekke forskjellige alternativer for avhending for å gjøre programmet mer utført, og i noen tilfeller mindre utsatt for at du blir begrenset av tjenesten (når du foretar for mange samtaler).</span><span class="sxs-lookup"><span data-stu-id="271cf-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="271cf-151">Hvis du vil lære mer, kan du se:</span><span class="sxs-lookup"><span data-stu-id="271cf-151">To learn more, see:</span></span>

- [<span data-ttu-id="271cf-152">Beste Fremgangs måter i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="271cf-153">Satsvise forespørsler</span><span class="sxs-lookup"><span data-stu-id="271cf-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="271cf-154">Spore endringer gjennom en delta-spørring</span><span class="sxs-lookup"><span data-stu-id="271cf-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="271cf-155">Få beskjed om endringer via webhooks</span><span class="sxs-lookup"><span data-stu-id="271cf-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="271cf-156">Begrensende veiledning</span><span class="sxs-lookup"><span data-stu-id="271cf-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="271cf-157">**Hvor kan jeg finne mer informasjon om feil og kjente problemer?**</span><span class="sxs-lookup"><span data-stu-id="271cf-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="271cf-158">Feil svar informasjon for Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="271cf-159">Kjente problemer med Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="271cf-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="271cf-160">**Hvor kan jeg sjekke status for tjeneste tilgjengelighet og tilkobling?**</span><span class="sxs-lookup"><span data-stu-id="271cf-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="271cf-161">Tjeneste tilgjengeligheten og tilkoblingen til de underliggende tjenestene som du kan få tilgang til gjennom Microsoft Graph, kan påvirke den generelle tilgjengeligheten og ytelsen til Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="271cf-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="271cf-162">For tjeneste tilstanden Azure Active Directory kan du kontrollere statusen for **sikkerhets-og identitets** tjenester som er oppført på [status siden for Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="271cf-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="271cf-163">For Office-tjenester som bidrar til Microsoft Graph, må du kontrollere statusen for tjenestene som er oppført i [instrument bordet for tilstands tilstand for Office Service](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="271cf-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
