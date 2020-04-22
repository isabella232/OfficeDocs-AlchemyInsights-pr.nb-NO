---
title: Identifisere slette meldingshendelser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716505"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvåkingslogger for slettede e-postmeldinger

Fra og med januar 2019 aktiverer Microsoft overvåkingslogging for postboks som standard. Hvis du vil se gjennom slettemeldingshendelser for en bestemt bruker, må du aktivere slettehandlingene for sporing av endringer manuelt. Hvis overvåkingslogging for postboksallerede er aktivert for organisasjonen eller for den bestemte brukeren, følger du fremgangsmåten nedenfor.

1. Logge på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klikk **Søk og undersøkelse,** og velg **Søk etter overvåkingslogg**.

3. Velg datoperioden i feltene **Startdato** og **Sluttdato.** Angi brukernavn for brukeren du vil undersøke (brukeren som slettet elementene). Velg **Slettede meldinger fra Slettede elementer-mappen** i **Aktiviteter-feltet,** og **Flytt meldinger til Slettede elementer-mappen**.

4. Klikk **Søk**.

Velg en overvåkingspost i resultatene. Klikk **Mer informasjon**i undermenyen for detaljer. Tilleggsinformasjon om det slettede elementet (for eksempel emnelinjen og plasseringen av elementet da det ble slettet) vises i **berørtelementer-feltet.** Egenskapen **ClientInfoString** viser om slettingen oppstod i Outlook, Outlook på nettet (tidligere kjent som Outlook Web App) eller en annen enhet.

Hvis du vil ha mer informasjon, kan du se [Finne ut hvem som konfigurerer videresending av e-post for en postboks](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Merk:** Du kan ikke hente slettede elementer ved hjelp av funksjonen for overvåkingslogg. Hvis du vil hente slettede meldinger i Outlook på nettet, kan du se [Gjenopprette slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
