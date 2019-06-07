---
title: Identifisere Slett melding hendelser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755161"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Overvåkingsloggen for slettede e-postmeldinger

Starter i januar 2019, slås Microsoft på postboks-sporing logger som standard. Ellers, hvis du vil se gjennom Slett melding hendelser for en bestemt bruker, må du aktivere manuelt slette-aksjoner for overvåking. Hvis postboksen overvåkes logging allerede er aktivert for organisasjonen, eller for en bestemt bruker, følger du fremgangsmåten nedenfor.

1. Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/)

2. Klikk **Søk og undersøkelser** , og velg **Overvåk Logg Søk**.

3. Velg datointervallet i feltene **Startdato** og **Sluttdato** . Angi brukernavnet for brukeren som du vil undersøke (brukeren som slettet elementene). Velg **Slettede meldinger fra Slettede elementer-mappen** og **Moved meldinger til Slettede elementer-mappen**i **aktiviteter** -feltet.

4. Klikk **Søk**.

I resultatene, velger du et kontrollregister. Klikk **Mer informasjon**i detaljer-undermeny. Hvis du vil ha mer informasjon om slettet element (for eksempel Emne-linjen, og plasseringen av elementet når det ble slettet) vises i feltet **AffectedItems** . Egenskapen **ClientInfoString** viser Hvis slettingen oppstod i Outlook, Outlook på weben (tidligere kjent som Outlook Web App) eller andre enheter.

Hvis du vil ha mer informasjon, kan du se [Determining som konfigurere e-post videresending for en bestemt postboks](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Merk**: du kan ikke gjenopprette slettede elementer ved hjelp av funksjonen for overvåkingspolicy logg. Hvis du vil hente slettede meldinger i Outlook på World Wide web, kan du se [Gjenopprett slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
