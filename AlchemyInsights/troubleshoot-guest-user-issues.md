---
title: Feilsøke gjeste bruker problemer
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901584"
---
# <a name="troubleshoot-guest-user-issues"></a>Feilsøke gjeste bruker problemer

1. Hvis du vil ha veiledning om hvordan du administrerer gjeste tilgang til programmer, kan du se [administrere gjeste tilgang med Azure ad Access-gjennomgang](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Legge til gjeste brukere i katalogen i Azure-portalen](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): i denne hurtigst Art skal du legge til en ny gjeste bruker i Azure ad-katalogen via Azure-portalen, sende en invitasjon og se hva gjeste innløsnings prosessen for invitasjonen ser ut.
1. [Legge til en gjeste bruker med PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): i denne hurtigst Art skal du bruke New-AzureADMSInvitation-kommandoen til å legge til én gjeste bruker i Azure-leieren.
1. Hvis du vil lære hvordan du tilordner brukere, og grupper, til virksomhets programmer i Azure Active Directory (Azure AD), enten fra i Azure-portalen eller ved hjelp av PowerShell, kan du se [administrere bruker tilordning for en app i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B-samarbeid fungerer med de fleste apper som integreres med Azure AD. I denne [artikkelen](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)går vi gjennom instruksjoner for å konfigurere noen populære Saas-apper for bruk med Azure ad B2B.
1. Som en organisasjon som bruker Azure Active Directory (Azure AD) B2B-samarbeids funksjoner til å invitere gjeste brukere fra partner organisasjoner til Azure AD, kan du nå gi disse B2B-brukerne tilgang til lokale apper. Disse lokale appene kan bruke SAML-basert godkjenning eller integrert Windows-godkjenning (IWA) med Kerberos begrenset delegering (KCD). Hvis du vil ha mer informasjon, kan du se [gi B2B-brukere i Azure ad Access til lokale programmer](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Lær hvordan du [gir lokale, administrerte partner kontoer tilgang til Sky ressurser ved hjelp av Azure ad B2B-samarbeid](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).