---
title: Finne manglende programmer på blad for appregistrering
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
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057111"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Finne manglende programmer på blad for appregistrering

1. Finner ikke programmer i portalen for appregistrering.

    Hvis et program er et program med flere leiere og det ble registrert i en annen leier, vises det ikke under blad for appregistrering. Det kan imidlertid hende at du finner det under Enterprise Applications-blad når du har fått tilgang til det (etter å ha blitt samtykket) og tjenesteprinsippet er opprettet i leieren. Hvis du vil ha mer informasjon, [kan du se &-tjenesteprinsipper i Azure AD – Microsofts identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Kan ikke vise apper i blad for appregistrering selv om du er administrator.

    Kontroller at du er i riktig katalog på Azure-portalen.
3. Programmet mitt er ikke oppført under Enterprise Applications-blad, men det vises når jeg spør etter PowerShell-kommandoen.

    Noen ganger, etter at du har slettet programmet fra Azure-portalen, vises det ikke i portalen, men det har kanskje ikke blitt slettet fullstendig. Hvis du vil ha mer informasjon, kan du se:
    - Du kan hente listen over tidligere slettede programmer og se om programmet vises i listen ved hjelp av Powershell-kommandoen: **Get-AzureADDeletedApplication**. Hvis du vil ha mer informasjon, kan du se [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Hvis du vil fjerne programmet fullstendig, kan du prøve følgende i PowerShell: **Remove-AzureADApplication -ObjectId**. Hvis du vil ha mer informasjon, [kan du se Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Du kan også prøve å gjenopprette det slettede programmet ved hjelp av følgende Powershell-kommando: **Gjenopprett AzureADDeletedApplication -ObjectId**. Hvis du vil ha mer informasjon, kan du se [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Finner ikke listen over alle forhåndsinstallerte bedriftsprogrammer i den nye Azure-tenanten.

    Det finnes ingen forhåndsinstallerte bedriftsprogrammer i Azure AD som standard. Du må legge det til manuelt fra «Nytt program»-alternativet ved å bla gjennom det fra Azure AD-galleriet eller legge til et program som ikke er galleri. Hvis du vil ha mer informasjon, kan du se Hurtigstart: Legge til et program i Azure Active Directory [(Azure AD) tenant.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Hvis du er global administrator, kan du enkelt få tilgang til appene ved hjelp [av Microsoft 365 startprogrammet](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)for apper .
5. Finner ikke appene mine fra Mine apper-portalen.

    Kontroller at apper ikke er skjult på mine apper-samlingssiden. Hvis du vil ha mer informasjon, kan du [se Samlinger (forhåndsvisning) i Mine apper-portalen – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Hvis du vil starte apper fra Mine apper-portalen, kan du se Finne & bruke apper i Mine [apper-portalen – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 Mover-appen vises ikke på Enterprise Applications-bladet etter installasjonen.

    «Office 365 Mover»-programmet er en app med flere hengsler som ikke trenger å legges til i AAD ved hjelp av Galleriprogrammer-delen under Registrering av enterprise-app. Hvis du Office 365 å få tilgang til Mover-appen, logger du ganske enkelt på appen og ber om brukerens samtykke for tillatelsene. Når brukeren gir samtykke, blir denne appen automatisk lagt til leieren med e-post-ID-en du har logget på.

    Når du har logger deg på programmet, skal du kunne finne programmets oppføring under Enterprise Applications'-bladet i AAD. Du må søke etter det programmet ved å skrive inn det fullstendige navnet, det vil si «Office 365 Mover», eller ganske enkelt søke etter «office», og den skal liste opp appen. Hvis du vil ha mer informasjon, Office 365 Mover at det allerede er installert, men at det ikke er oppført i [enterprise-programgalleriet](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html).
8. Hurtigstart: Vis listen over programmer som bruker [Azure Active Directory-tenanten (Azure AD) for](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) identitetsbehandling, som viser deg hvordan du viser programmene, også kalt apper, som allerede er konfigurert til å bruke Azure AD-leieren som identitetsleverandør (IdP).
9. [Feilsøke vanlige problemer med å legge](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) til eller fjerne et program Azure Active Directory hjelper deg med å forstå de vanlige problemene personer opplever når de viser apper i Azure Active Directory.
