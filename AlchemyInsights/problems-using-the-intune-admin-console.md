---
title: Problemer med å bruke Intune admin console
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555387"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemer med å bruke Intune admin console

**"Ingen tilgang" når du navigerer i administrasjonsportalen for Intune.**

- Hvis du er medlem av en egendefinert intune-rolle, må du kontrollere at en Intune- eller Enterprise Mobility Suite (EMS)-lisens er tilordnet kontoen din.
- Hvis du bruker Configuration Manager til å administrere enheter, må du kontrollere at du ikke er en del av Intune-brukersamlingen for Configuration Manager MDM.
- Kontroller at du er tilordnet de riktige rollebaserte administrasjonskontrolltillatelsene (RBAC) i intune-rollebladet.
- Kontroller at gruppen som brukes, ikke er en distribusjonsliste. Intune i Azure-portalen støtter bare brukerkontoer som tilhører Azure Active Directory-sikkerhetsgrupper. Se gjennom gruppene i Azure-portalen > **Intune**  >  **Groups**eller i Azure-portalen > **Azure Active Directory**.

**Brukeren har for mange tillatelser for tilordnet Intune-rolle**

Råder brukeren til å gå til **Intune**  >  **Intune roller**  >  **Mine tillatelser**  >  **Eksporter** for å se gjennom gitte tillatelser.

**Jeg har lagt til en omfangsgruppe i en rolle, men brukere i denne rollen ser fortsatt andre brukere eller enheter.**

Omfangsgrupper filtrerer ikke ut brukere eller enheter. Omfangsgrupper:

- Begrens hvem brukere kan tilordne policyer eller programmer til.
- Tillat bare bestemte brukere å kjøre eksterne oppgaver på enheter.

Hvis du vil ha mer informasjon om omfangsgrupper, kan du se [Rollebasert tilgangskontroll (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Jeg har lagt til en bruker i en Intune-rolle, men de har fortsatt full tilgang til Intune admin console.**

Naviger til Intune > **brukere** i Azure-portalen, og kontroller at brukeren ikke er tilordnet til noen av følgende roller i Azure-portalen:

- Global administrator
- Intune-tjenesteadministrator
- SharePoint-administrator

Hvis du vil ha mer informasjon, kan du se [Rollebasert tilgangskontroll (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemer med tilgang**

Hvis du vil ha mer informasjon, kan du se [Du kan ikke logge på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).