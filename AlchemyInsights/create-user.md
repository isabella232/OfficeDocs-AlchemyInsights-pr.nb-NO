---
title: Opprette bruker
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569740"
---
# <a name="create-user"></a>Opprette bruker

**KUNNGJØRING:**

- [Avvikling av støtte for WebView-pålogging fra Google fra og med 4. januar 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Test om appene kan bli påvirket ved å følge [Googles veiledning](https://go.microsoft.com/fwlink/?linkid=2157323) om testing av kompatibilitet.
- Kontroller at du bruker systemets nettvisning eller systemleser når du logger på brukerne med forbrukerkontoer fra Google. Hvis du vil ha mer informasjon, kan du se Problemer med å logge [på programmer bare ved hjelp av Chrome-nettleseren.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Jeg kan ikke opprette en ny bruker i Azure AD-katalogen**

1. Kontroller at du er autorisert til å opprette en ny standardbruker. Bare rollen global administrator eller brukeradministrator i Azure Active Directory (AD) kan opprette en ny standardbruker. Hvis du ikke er i en av disse rollene, kan du be en administrator om å legge deg til i en av disse rollene eller opprette den nye brukerkontoen for deg.
1. Kontroller at brukernavnet er i et domene som er bekreftet i Azure AD. Hvis du ikke har noen bekreftede egendefinerte domenenavn i Azure AD, kan du bruke det opprinnelige Azure AD-domenet, som slutter med *.onmicrosoft.com.
1. Kontroller at brukernavnet er i et domene som ikke er forbundsbasert til Azure AD fra den lokale AD-en. Brukere kan ikke legges til i skyen med domenenavn som er forbundsbasert fra lokalt.
1. Kontroller at ingen andre brukere eller kontakter allerede har brukernavnet du vil tilordne til den nye brukeren. Brukernavn må være unike på tvers av Azure AD.
1. Se [Azure AD-roller og -administratorer](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for Azure AD.
1. Se [domenenavnene](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for Azure AD.
1. Se [gjennom overvåkingslogger](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for å se mer detaljert informasjon om en nylig opprettet eller slettet bruker, for eksempel hvem som utførte handlingen og når.
1. Hvis du vil ha mer informasjon om hvordan du legger til nye brukere, kan du se Bruke [Azure-portalen til å opprette en ny bruker i Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Administrative roller i Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)Administratorrolletillatelser i Azure Active Directory
1. Du kan også [bruke Azure AD PowerShell til å opprette en ny bruker.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
