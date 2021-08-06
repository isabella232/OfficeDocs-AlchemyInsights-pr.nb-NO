---
title: Arbeidsdag til AD-bruker klargjøring går i karantenetilstand
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036501"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Arbeidsdag til AD-bruker klargjøring går i karantenetilstand

**Arbeidsdag til AD Bruker klargjøring går i karantenetilstand, og ingen brukere opprettes i AD**

Jobben Klargjøring av bruker for Arbeidsdag til AD har gått i karantenetilstand, og overvåkingsloggene viser eksportfeilhendelser med feilmeldingen **Feil: OperationsError-SvcErr: Det oppstod en operasjonsfeil. Ingen overordnet referanse er konfigurert for katalogtjenesten. Katalogtjenesten kan derfor ikke utstede henvisninger til objekter utenfor denne skogen**. Denne feilen vises vanligvis hvis Active Directory Container OU ikke er riktig angitt, eller hvis det er problemer med uttrykkstilordningen som brukes for **overordnetDistinguishedName**.

Kontroller standard OU for **Nye brukere-parameteren** for skrivefeil. Kontroller at den angitte organisasjonsenheten allerede finnes i AD. Hvis du bruker **overordnetDistinguishedName** i attributttilordningen, må du kontrollere at den alltid evalueres til en kjent beholder i AD-domenet. Kontroller Eksporter-hendelsen i overvåkingsloggene for å se den genererte verdien.

Hvis du vil ha mer informasjon om hvordan du konfigurerer arbeidsdag for automatisert klargjøring, kan du se [Opplæring: Konfigurere arbeidsdag for automatisk klargjøring av brukere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

