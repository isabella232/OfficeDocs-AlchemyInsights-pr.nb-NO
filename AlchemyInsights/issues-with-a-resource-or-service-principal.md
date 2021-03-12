---
title: Problemer med et ressurs- eller tjenesteprinsipp
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714080"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemer med et ressurs- eller tjenesteprinsipp

1. Hvis du akkurat har begynt, beskriver Program- og tjenesteprinsippobjekter i [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) programregistrering, programobjekter og tjenesteprinsipper i Azure Active Directory: hva de er, hvordan de brukes og hvordan de er relatert til hverandre. Et eksempelscenario med flere leiere presenteres også for å illustrere relasjonen mellom programobjektet for et program og tilsvarende tjenesteprinsippobjekter.
2. Du kan finne ut mer om relasjonen mellom programmer og tjenesteprinsipper ved å lese programmer og hovedobjekter for tjenester [i Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. Slik gjør du det: Bruk [portalen](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) til å opprette et Azure AD-program- og tjenesteprinsipp som har tilgang til ressurser, som viser deg hvordan du oppretter et nytt Azure Active Directory-program og tjenesteprinsipp som kan brukes med den rollebaserte tilgangskontrollen.
4. Med [tjenesteprinsipp-API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)kan du programmatisk administrere forekomster av programmer og kontrollere hva et program kan gjøre i leieren.
5. [servicePrincipal-ressurstype](https://docs.microsoft.com/graph/api/resources/serviceprincipal) viser alle egenskaper og metoder for servicePrincipal-ressurstypen.
6. [Forskjeller på ressurstypen mellom Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) og Microsoft Graph fremhever forskjeller mellom Azure AD Graph- og Microsoft Graph-ressurser. Den viser ressurser som har ulike navn eller ikke er tilgjengelige. Den uthever også ressurser som er tilgjengelige i betaversjonen av Microsoft Graph, men ikke i v1.0-versjonen.

**Problemer med gjestebrukere**

- [Hurtigstart:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Legg til gjestebrukere i katalogen i Azure Portal viser deg hvordan du legger til en ny gjestebruker i Azure AD-katalogen via Azure Portal, sender en invitasjon og ser hvordan innløsningsprosessen for gjestebrukeren ser ut.
- [Opplæring: Opprett brukerflyter i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) viser deg hvordan du oppretter noen anbefalte brukerflyter ved hjelp av Azure Portal. Hvis du leter etter informasjon om hvordan du konfigurerer en roPC-flyt (resource owner password credentials) i programmet, kan du se Konfigurere flyten for passordlegitimasjon for ressurseier i Azure AD B2C.
