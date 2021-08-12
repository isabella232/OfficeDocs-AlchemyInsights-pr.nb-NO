---
title: Feilsøke problemer med gjestebrukere
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939388"
---
# <a name="troubleshoot-guest-user-issues"></a>Feilsøke problemer med gjestebrukere

1. Hvis du vil ha veiledning om hvordan du administrerer gjestetilgang til programmer, kan du se [Administrere gjestetilgang med Azure AD-tilgangsanmeldelser](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. Legg til gjestebrukere i katalogen i [Azure-portalen:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)I denne hurtigstarten legger du til en ny gjestebruker i Azure AD-katalogen via Azure-portalen, sender en invitasjon og ser hvordan innløsningsprosessen for gjestebrukeren ser ut.
1. [Legg til en gjestebruker med PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)I denne hurtigstarten bruker du kommandoen New-AzureADMSInvitation til å legge til én gjestebruker i Azure-tenanten.
1. Hvis du vil lære hvordan du tilordner brukere og grupper, til bedriftsprogrammer i Azure Active Directory (Azure AD), enten fra Azure-portalen eller ved hjelp av PowerShell, kan du se Administrere brukertilordning for en [app i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B-samarbeid fungerer med de fleste apper som integreres med Azure AD. I denne [artikkelen](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)går vi gjennom instruksjoner for hvordan du konfigurerer noen populære SaaS-apper for bruk med Azure AD B2B.
1. Som en organisasjon som bruker Azure Active Directory (Azure AD) B2B-samarbeidsfunksjoner til å invitere gjestebrukere fra partnerorganisasjoner til Azure AD, kan du nå gi disse B2B-brukerne tilgang til lokale apper. Disse lokale appene kan bruke SAML-basert godkjenning eller Integrert Windows-godkjenning (IWA) med begrenset Kerberos-delegering (KCD). Hvis du vil ha mer informasjon, kan du se [Gi B2B-brukere i Azure AD tilgang til de lokale programmene.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Finn ut hvordan du gir lokalt administrerte partnerkontoer tilgang til skyressurser ved hjelp [av Azure AD B2B-samarbeid.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)