---
title: Få en liste over enterprise-programmer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404926"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="d9334-102">Få en liste over enterprise-programmer</span><span class="sxs-lookup"><span data-stu-id="d9334-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="d9334-103">Hvis **du** vil ha en liste over bedriftsprogrammer (alle programmer eller filtrert etter visningsnavn, ID, identifikator-URIer og så videre) via Powershell-kommandoen, kan du se [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="d9334-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="d9334-104">Hvis du vil ha en liste over tjenesteprinsippobjekter (alle objekter eller filtrert etter ID) via Powershell-kommandoen, kan du se [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="d9334-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="d9334-105">Hvis du vil ha **en liste over SAML-konfigurerte apper, kan følgende PowerShell-skript** hjelpe deg:</span><span class="sxs-lookup"><span data-stu-id="d9334-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="d9334-106">Hvert program er en OAuth-app eller SAML-app (både galleri- og ikke-galleriapper) vil ha to objekter opprettet i AAD når registreringen skjer.</span><span class="sxs-lookup"><span data-stu-id="d9334-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="d9334-107">Det ene kalles programobjektet, og det andre er tjenesteprinsippobjektet.</span><span class="sxs-lookup"><span data-stu-id="d9334-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="d9334-108">Når du dumper egenskapene for et tjenesteprinsippobjekt ved hjelp av PowerShell, vil du se at hvert program har et bestemt antall tilknyttede koder:</span><span class="sxs-lookup"><span data-stu-id="d9334-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="d9334-109">OAuth-apper har en kode kalt **WindowsAzureActiveDirectoryIntegratedApp**</span><span class="sxs-lookup"><span data-stu-id="d9334-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="d9334-110">Galleri SAML-apper har en kode kalt **WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**</span><span class="sxs-lookup"><span data-stu-id="d9334-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="d9334-111">SAML-apper uten galleri har en kode kalt **WindowsAzureActiveDirectoryCustomSingleSignOnApplication**</span><span class="sxs-lookup"><span data-stu-id="d9334-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="d9334-112">Derfor kan du bruke disse kodene og finne ut hva slags app det er.</span><span class="sxs-lookup"><span data-stu-id="d9334-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="d9334-113">Koden **WindowsAzureActiveDirectoryIntegratedApp** er vanlig for alle typer apper.</span><span class="sxs-lookup"><span data-stu-id="d9334-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="d9334-114">Du kan bruke følgende kodesnutt til å liste opp alle SAML-appene (både galleri og ikke-galleri):</span><span class="sxs-lookup"><span data-stu-id="d9334-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="d9334-115">Hvis du vil ha mer informasjon, kan du [se Identifisere SAML-aktiverte apper i Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span><span class="sxs-lookup"><span data-stu-id="d9334-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="d9334-116">**Finn og vis bare nettprogrammer:** Bruk kommandoen nedenfor til å få alle Azure AD-programmer med programtypen «Nettapp/API»</span><span class="sxs-lookup"><span data-stu-id="d9334-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="d9334-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="d9334-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="d9334-118">**Finn og vis opprinnelige programmer alene:** Kjør følgende kommando for å få alle opprinnelige klientprogrammer (stasjonære/mobile enheter).</span><span class="sxs-lookup"><span data-stu-id="d9334-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="d9334-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="d9334-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="d9334-120">**Eksporter alle registrerte Azure AD-programdetaljer til CSV:** Kommandoen nedenfor eksporterer alle Azure AD-appene med nødvendige detaljer til CSV-filen:</span><span class="sxs-lookup"><span data-stu-id="d9334-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="d9334-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="d9334-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="d9334-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="d9334-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="d9334-123">**Trenger du å eksportere en liste over ubrukte Azure-apper** – overvåkingsrapport</span><span class="sxs-lookup"><span data-stu-id="d9334-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="d9334-124">Azure AD kan vise programlogger i opptil 30 dager forutsatt at du har Azure AD Premium-lisens.</span><span class="sxs-lookup"><span data-stu-id="d9334-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="d9334-125">Du har to alternativer for å beholde dataene i mer enn 30 dager.</span><span class="sxs-lookup"><span data-stu-id="d9334-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="d9334-126">Du kan bruke [AZURE AD Reporting API-ene](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) til å hente dataene programmatisk og lagre dem i en database.</span><span class="sxs-lookup"><span data-stu-id="d9334-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="d9334-127">Alternativt kan du integrere overvåkingslogger i et tredjeparts SIEM-system.</span><span class="sxs-lookup"><span data-stu-id="d9334-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="d9334-128">Du kan også laste ned applisten for alle programmer og eide programmer under Azure Active Directory>Appregistreringer>Last ned>Alle programmer/Eide programmer.</span><span class="sxs-lookup"><span data-stu-id="d9334-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="d9334-129">Hvis du vil ha en liste over programmer via MS Graph, kan du se Listeprogrammer [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) og programressurstype [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="d9334-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
