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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404782"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Klienthemmelighet for appregistrering eller sertifikatproblemer

Programklientens hemmelige utløp?

Uavhengig av hvordan det registrerte programmet ble opprettet, enten gjennom standard registreringsprosessen i appregistreringsportalen eller hvis tjenesteprinsippet ble opprettet i leieren ved hjelp av programsamtykke, må en ny klienthemmelighet opprettes før utløpet av den gjeldende og oppdateres i den relaterte programkoden. Den maksimale gyldighetsperioden er 2 år. Som en påminnelse må den hemmelige verdien registreres, da den ikke lenger vil være synlig når du forlater appregistreringssiden i portalen. Hvis du vil ha mer informasjon, kan du se [Hurtigstart: Registrere en app](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) i Microsofts identitetsplattform og Anbefalte fremgangsmåter [for Microsoft-identitetsplattformen.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Hvis du vil ha mer informasjon, kan du [se Opprette en Azure AD-app & tjenesteprinsipp i portalen – Microsofts identitetsplattform.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
