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
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508997"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvåkingslogger for slettede e-postmeldinger

Fra og med januar 2019 aktiverer Microsoft som standard logging av overvåking av postboks. Hvis du vil se gjennom slette meldingshendelser for en bestemt bruker, må du manuelt aktivere slettehandlingene for sporing av endringer. Hvis overvåkingslogging for postboksen allerede er aktivert for organisasjonen eller for den bestemte brukeren, følger du fremgangsmåten nedenfor.

1. Logge på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)

2. Klikk **Søk og etterforskning,** og velg **Søk etter overvåkingslogg**.

3. Velg datointervallet i feltene **Startdato** og **Sluttdato.** Angi brukernavn for brukeren du vil undersøke (brukeren som slettet elementene). I **Aktiviteter-feltet** velger du **Slettede meldinger fra Slettede elementer-mappen** og **Flyttet meldinger til Slettede elementer-mappen**.

4. Klikk **Søk**.

Velg en overvåkingspost i resultatene. Klikk **Mer informasjon**i detalj-undermenyen. Tilleggsinformasjon om det slettede elementet (for eksempel emnelinjen og plasseringen av elementet da det ble slettet) vises i **Feltet AffectedItems.** **Egenskapen ClientInfoString** viser om slettingen oppstod i Outlook, Outlook på nettet (tidligere kjent som Outlook Web App) eller en annen enhet.

Hvis du vil ha mer informasjon, kan du se [Finne ut hvem som konfigurerte videresending av e-post for en postboks](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Merk:** Du kan ikke hente slettede elementer ved hjelp av funksjonen for overvåkingslogg. Hvis du vil hente slettede meldinger i Outlook på nettet, kan du se [Gjenopprette slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
