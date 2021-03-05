---
title: Klargjøring av arbeidsdager til AD-bruker går i karantenetilstand
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481880"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Klargjøring av arbeidsdager til AD-bruker går i karantenetilstand

**Klargjøring av arbeidsdager til AD-bruker går i karantenetilstand, og ingen brukere opprettes i AD**

Klargjøringsjobben for arbeidsdagen til AD-bruker er satt i karantene, og overvåkingsloggene viser eksportfeilhendelser med **feilmeldingsfeilen: OperationsError-SvcErr: Det oppstod en operasjonsfeil. Ingen overordnet referanse er konfigurert for katalogtjenesten. Katalogtjenesten kan derfor ikke utstede henvisninger til objekter utenfor denne skogen.** Denne feilen vises vanligvis hvis organisasjonsenheten for Active Directory-beholder ikke er riktig angitt, eller hvis det er problemer med uttrykkstilordningen som brukes for **parentDistinguishedName.**

Se etter skrivefeil i **parameteren** Standard organisasjonsenheten for nye brukere. Kontroller at den angitte organisasjonsenheten allerede finnes i AD. Hvis du bruker **parentDistinguishedName** i attributttilordningen, må du kontrollere at det alltid evalueres til en kjent beholder innenfor AD-domenet. Kontroller Eksport-hendelsen i overvåkingsloggene for å se den genererte verdien.

Hvis du vil ha mer informasjon om hvordan du konfigurerer arbeidsdag for automatisert klargjøring, kan du se [Opplæring: Konfigurere arbeidsdag for automatisk klargjøring av brukere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

