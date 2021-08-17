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
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116737"
---
# <a name="get-a-list-of-enterprise-applications"></a>Få en liste over enterprise-programmer

1. Hvis **du** vil ha en liste over bedriftsprogrammer (alle programmer eller filtrert etter visningsnavn, ID, identifikator-URIer og så videre) via Powershell-kommandoen, kan du se [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Hvis du vil ha en liste over tjenesteprinsippobjekter (alle objekter eller filtrert etter ID) via Powershell-kommandoen, kan du se [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Hvis du vil ha **en liste over SAML-konfigurerte apper, kan følgende PowerShell-skript** hjelpe deg:

    Hvert program er en OAuth-app eller SAML-app (både galleri- og ikke-galleriapper) vil ha to objekter opprettet i AAD når registreringen skjer. Det ene kalles programobjektet, og det andre er tjenesteprinsippobjektet. Når du dumper egenskapene for et tjenesteprinsippobjekt ved hjelp av PowerShell, vil du se at hvert program har et bestemt antall tilknyttede koder:

    - OAuth-apper har en kode kalt **WindowsAzureActiveDirectoryIntegratedApp**
    - Galleri SAML-apper har en kode kalt **WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**
    - SAML-apper uten galleri har en kode kalt **WindowsAzureActiveDirectoryCustomSingleSignOnApplication**

    Derfor kan du bruke disse kodene og finne ut hva slags app det er. Koden **WindowsAzureActiveDirectoryIntegratedApp** er vanlig for alle typer apper. Du kan bruke følgende kodesnutt til å liste opp alle SAML-appene (både galleri og ikke-galleri):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Hvis du vil ha mer informasjon, kan du [se Identifisere SAML-aktiverte apper i Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Finn og vis bare nettprogrammer:** Bruk kommandoen nedenfor til å få alle Azure AD-programmer med programtypen «Nettapp/API»

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Finn og vis opprinnelige programmer alene:** Kjør følgende kommando for å få alle opprinnelige klientprogrammer (stasjonære/mobile enheter).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Eksporter alle registrerte Azure AD-programdetaljer til CSV:** Kommandoen nedenfor eksporterer alle Azure AD-appene med nødvendige detaljer til CSV-filen:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Trenger du å eksportere en liste over ubrukte Azure-apper** – overvåkingsrapport

    Azure AD kan vise programlogger i opptil 30 dager forutsatt at du har Azure AD Premium lisens.
    Du har to alternativer for å beholde dataene i mer enn 30 dager. Du kan bruke [AZURE AD Reporting API-ene](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) til å hente dataene programmatisk og lagre dem i en database. Alternativt kan du integrere overvåkingslogger i et tredjeparts SIEM-system.

    Du kan også laste ned applisten for alle programmer og eide programmer under Azure Active Directory>Appregistreringer>Last ned>Alle programmer/Eide programmer.

    Hvis du vil ha en liste over programmer gjennom MS Graph, kan du se Listeprogrammer [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) og programressurstype [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
