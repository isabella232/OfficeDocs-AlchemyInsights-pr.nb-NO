---
title: Identifisere slette meldingshendelser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115657"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvåkingslogger for slettede e-postmeldinger

Fra og med januar 2019 aktiverer Microsoft overvåkingslogging for postboks som standard. Hvis du vil se gjennom slette meldingshendelser for en bestemt bruker, må du manuelt aktivere slettehandlingene for overvåking. Hvis overvåkingslogging for postboks allerede er aktivert for organisasjonen eller for den bestemte brukeren, følger du fremgangsmåten nedenfor.

1. Logg på Microsoft 365 [samsvarssenteret](https://protection.office.com/)

2. Klikk **Søk og undersøkelser,** og velg **Søk i overvåkingslogg**.

3. Velg datoområdet i **feltene Startdato og** **Sluttdato.** Angi brukernavnet for brukeren du vil undersøke (brukeren som slettet elementene). Velg **Slettede** meldinger fra **Slettede** elementer-mappen og Flyttet meldinger til **Slettede elementer-mappen i Aktiviteter-feltet.**

4. Klikk **Søk**.

Velg en overvåkingspost i resultatene. Klikk Mer informasjon på **detaljer-undermenyen.** Tilleggsinformasjon om det slettede elementet (for eksempel emnelinjen og plasseringen til elementet da det ble slettet) vises i **AffectedItems-feltet.** **ClientInfoString-egenskapen** viser om slettingen oppstod i Outlook, Outlook på nettet (tidligere kalt Outlook Web App), eller en annen enhet.

Hvis du vil ha mer informasjon, kan du se [Fastslå hvem som konfigurerte videresending av e-post for en postboks](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Obs!** Du kan ikke hente slettede elementer ved hjelp av overvåkingsloggfunksjonen. Hvis du vil hente slettede meldinger i Outlook på nettet, kan du se [Gjenopprette slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
