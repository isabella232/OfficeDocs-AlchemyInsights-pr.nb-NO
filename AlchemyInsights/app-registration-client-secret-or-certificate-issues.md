---
title: Klienthemmelighet for appregistrering eller sertifikatproblemer
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
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951502"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Klienthemmelighet for appregistrering eller sertifikatproblemer

Programklientens hemmelige utløp?

Uavhengig av hvordan det registrerte programmet ble opprettet, enten gjennom standard registreringsprosessen i appregistreringsportalen eller hvis tjenesteprinsippet ble opprettet i leieren ved hjelp av programsamtykke, må en ny klienthemmelighet opprettes før utløpet av den gjeldende og oppdateres i den relaterte programkoden. Den maksimale gyldighetsperioden er 2 år. Som en påminnelse må den hemmelige verdien registreres, da den ikke lenger vil være synlig når du forlater appregistreringssiden i portalen. Hvis du vil ha mer informasjon, kan du se [Hurtigstart:](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) Registrere en app i Microsofts identitetsplattform og [anbefalte fremgangsmåter for Microsofts identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).

Hvis du vil ha mer informasjon, kan du se Opprette [en Azure AD-app & tjenesteprinsipp i portalen – Microsofts identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).
