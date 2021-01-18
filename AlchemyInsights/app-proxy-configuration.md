---
title: Proxy-konfigurasjon for App
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885522"
---
# <a name="app-proxy-configuration"></a>Proxy-konfigurasjon for App

1. Hvis du vil forstå hvordan du konfigurerer et program-proxy-program i Azure AD for å eksponere lokale programmer i skyen, kan du se [hvordan du konfigurerer en](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)programproxy for programmet.
2. Enkel pålogging (SSO) lar brukerne få tilgang til et program uten å godkjenne flere ganger. Den gjør det mulig å utføre enkel godkjenning i skyen mot Azure Active Directory, og tillater tjenesten eller kontakten å representere brukeren for å fullføre eventuelle ytterligere godkjennings utfordringer fra programmet. Hvis du vil ha mer informasjon, kan du se [Slik konfigurerer du enkel pålogging til et program-proxy-program](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Bruk [denne artikkelen](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) til å feilsøke vanlige problemer som personer står overfor når du oppretter et nytt program-proxy-program.
4. Hvis du har problemer med å konfigurere bak godkjenning til programmet, må du kanskje [Feilsøke Kerberos-begrensede delegerings konfigurasjoner for programproxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) eller følge veiledning om [konfigurasjon av program med PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) for å løse problemet.
