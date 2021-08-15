---
title: Identifisere innboksregelaktivitet i overvåkingslogger
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976874"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifisere innboksregelaktivitet i overvåkingslogger

Du kan bruke søk i overvåkingsloggen i Microsoft 365 sikkerhets- & samsvarssenteret til å vise innboksregelhendelser (opprette, endre og slette innboksregler).

1. Logg på Microsoft 365 [Samsvarssenter](https://protection.office.com/).

2. Gå til **søkesiden**  >  **søk i overvåkingsloggen.**

3. Velg datoområdet i **feltene Startdato og** **Sluttdato.**

4. Kontroller **Exchange** Aktiviteter-feltet er  satt til Ny **innboksRegel Opprett/endre/aktiver/deaktiver** innboksregel under Exchange postboksaktiviteter .

5. Klikk **Søk**.

Velg en overvåkingspost i resultatene. Klikk Mer informasjon på **detaljer-undermenyen.** Informasjon om innstillingene for innboksregelen vises i **Parametere-feltet.**

Hvis du vil ha mer informasjon, [kan du se Fastslå om en bruker opprettet en innboksregel](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
