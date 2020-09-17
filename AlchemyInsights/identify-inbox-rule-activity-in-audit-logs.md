---
title: Identifisere regel aktivitet for innboksen i overvåkings logger
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779060"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifisere regel aktivitet for innboksen i overvåkings logger

Du kan bruke overvåkings Logg søk i 365 Microsofts sikkerhets & Samsvars senter for å vise regel hendelser for innboksen (oppretting, endring og sletting av regler for innboksen).

1. Logg på [sikkerhets & samsvars senteret til Microsoft 365](https://protection.office.com/).

2. Gå til **Search**  >  **søke siden for overvåkings Logg** for søk.

3. Velg dato området i feltene **Start dato** og **slutt dato** .

4. Under **Exchange post boks aktiviteter**kontrollerer du at **aktiviteter** -feltet er satt til **New-InboxRule Create/modify/enable/disable Rule**.

5. Klikk **Søk**.

Velg en overvåkings post i resultatene. Klikk **mer informasjon**i under menyen detaljer. Informasjon om innstillingene for innboks-regelen vises i **Parametere** -feltet.

Hvis du vil ha mer informasjon, kan du se [fastslå om en bruker har opprettet en innboks-regel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
