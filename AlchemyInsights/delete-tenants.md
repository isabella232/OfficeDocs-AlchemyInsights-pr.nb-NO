---
title: Slett Tenant
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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564615"
---
# <a name="delete-tenant"></a>Slett Tenant

Hvis du vil slette en Azure AD, må du kontrollere følgende:
- Du er en global administrator på katalogen.
- Du er ikke logget på med en konto som har standard katalogen, for eksempel contoso.onmicrosoft.com i den påloggede kontoen, for eksempel admin@contoso.onmicrosoft.com.
- Fjern alle aktive programmer i katalogen før sletting. Hvis du vil fjerne aktive programmer, går du til app-registreringer og fjerner eksisterende programmer.
- Det finnes ingen aktive abonnementer for noen Microsoft Online-tjenester, for eksempel Microsoft Azure, Office 365 eller Azure AD Premium, som er knyttet til katalogen. Overfør abonnementene dine eller ekspedere annulleringer av aktive abonnementer via Azure kunde støtte og fakturering. Finn ut mer om hvordan du avbryter Office-365 og Azure-abonnementer. Hvis du vil ha veiledning om hvordan du knytter eller legger til et eksisterende abonnement på en leier, kan du se [knytte til eller legge til et Azure-abonnement i Azure ad-leieren](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Det er ingen aktiv lisens. Hvis du vil fjerne lisenser, kan du se [hvordan du fjerner abonnementet for å fjerne lisensen](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Det er ingen andre aktive brukere i katalogen enn deg selv som den globale administratoren når du prøver å slette Azure AD. Fjern alle andre aktive brukere, og eventuelle avhengigheter i et egen definert domene navn i leieren må også fjernes, for eksempel brukere som er opprettet med admin@contoso.com.

Hvis du vil ha mer informasjon om hvordan du gjør følgende:
- Slett Azure Active Directory eller abonnement, se [slette Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Hvis du fjerner programmer i katalogen, kan du se [fjerne programmer](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
