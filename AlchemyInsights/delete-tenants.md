---
title: Slett tenant
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993902"
---
# <a name="delete-tenant"></a>Slett tenant

Hvis du vil slette en Azure AD, må du sørge for at:
- Du er global administrator i katalogen.
- Du er IKKE logget på med en konto som har standardkatalogen, for eksempel contoso.onmicrosoft.com den påloggede kontoen, for eksempel admin@contoso.onmicrosoft.com.
- Fjern eventuelle aktive programmer i katalogen før sletting. Hvis du vil fjerne aktive programmer, går du til Appregistreringer og fjerner de eksisterende programmene.
- Det finnes ingen aktive abonnementer for noen Microsoft Online Services, for eksempel Microsoft Azure, Office 365 eller Azure AD Premium tilknyttet på katalogen. Overfør abonnementene eller fremskynde kansellering av aktive abonnementer via Azure-støtte og fakturering. Finn ut mer om Hvordan du kansellere Office 365 og Azure-abonnementer. Hvis du vil ha veiledning om hvordan du knytter til eller legger til et eksisterende abonnement i en leier, kan du se Knytte eller legge til et Azure-abonnement i [Azure AD-leieren.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Det finnes ingen aktiv lisens. Hvis du vil fjerne lisenser, [kan du se Slik fjerner du abonnementet for å fjerne lisensen](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Det finnes ingen andre aktive brukere i katalogen, bortsett fra deg selv som global administrator når du prøver å slette Azure AD. Fjern andre aktive brukere, og eventuelle avhengigheter av et egendefinert domenenavn i leieren må også fjernes, for eksempel brukere som er opprettet med admin@contoso.com.

Hvis du vil ha mer detaljerte trinn om hvordan du gjør følgende:
- Slett «Azure Active Directory» eller «abonnement», se [Slett Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Hvis du fjerner programmer i katalogen, kan [du se Fjerne programmer](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
