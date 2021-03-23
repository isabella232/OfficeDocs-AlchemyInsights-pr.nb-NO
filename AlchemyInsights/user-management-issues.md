---
title: Problemer med brukeradministrasjon
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036287"
---
# <a name="user-management-issues"></a>Problemer med brukeradministrasjon

**Hva skjer med gjeldende tilordnede brukere til programmet hvis jeg deaktiverer egenskapen Brukertilordning kreves (angi denne egenskapen til Nei)?**

Deaktivering av **brukertilordning kreves** påvirker IKKE de tilordnede brukerne. Hvis du deaktiverer denne egenskapen, får bare alle brukere tilgang til programmet. Alle de oppførte brukerne og de brukerne som er tilordnet til grupper i programmet, vil fortsatt være gyldige.

- Hvis du vil begrense appen til et bestemt sett med brukere, kan du se – Begrense Azure AD-appen til et sett med brukere [– Microsofts identitetsplattform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Hvis du vil tilordne brukere og grupper, til bedriftsprogrammer i Azure Active Directory (Azure AD), enten fra Azure-portalen eller ved hjelp av PowerShell, kan du se Administrere brukertilordning for en app i [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Hvis du vil delegere tillatelser for oppretting og administrasjon av programmer, kan du se Delegere administratortillatelser for programadministrasjon [– Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Skjul bestemte bedriftsapper for brukere** – Bruk fremgangsmåten nedenfor til å skjule alle Microsoft 365-apper fra **MyApps-panelet.** Appene vil fortsatt være synlige i Office 365-portalen.

 1. Logg på Azure-portalen som global administrator for katalogen. 
 2. Velg **Azure Active Directory**. 
 3. Velg **Brukere**. 
 4. Velg **Brukerinnstillinger**. 
 5. Klikk **Administrer hvordan** sluttbrukere starter og viser programmene under **Virksomhetsprogrammer**. 
 6. For **Brukere kan bare se Office 365-apper i Office 365-portalen,** klikker du **Ja**. 
 7. Klikk på **Lagre**. 
 8. Hvis du vil ha mer informasjon, kan du se Skjule et [Enterprise-program fra brukeropplevelsen i Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Hvis du tilbyr en Programvare som tjenesteapp (SaaS) til mange organisasjoner, kan du konfigurere appen til å godta pålogginger fra en hvilken som helst Azure Active Directory-leier (Azure AD). Denne konfigurasjonen kalles «å gjøre programmet ditt til flere leiere». Brukere i enhver Azure AD-leier kan logge på appen etter at de har samtykket til å bruke kontoen sin med appen. Hvis du vil ha mer informasjon, kan du se Bygge [apper som logger på Azure AD-brukere – Microsofts identitetsplattform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Hvordan får en sluttbruker tilgang til programmet når han/hun er tilordnet til programmet?**

Hver app i Enterprise-programbladet har en kobling som sluttbrukerne kan få tilgang til. Brukere kan også få tilgang til appen via **Myapps-portalen** på en enkel måte.

- **Vil du vite hvilke programmer og hvilken type programmer som brukes av brukere?**

Du kan laste ned påloggingsrapporter for de siste 30 dagene fra portal.azure.com > Azure Active Directory> **Signins> laste ned rapporter.**

- Finn ut hvordan [du gir hele leieren tillatelse til](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) et program og Konfigurerer hvordan [sluttbrukere samtykker i programmer.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- Forstå [hvordan samtykke fungerer og](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) Administrere samtykke til [programmer.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


