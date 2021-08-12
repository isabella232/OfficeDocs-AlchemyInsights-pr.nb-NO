---
title: Opprette en gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929314"
---
# <a name="create-a-group"></a>Opprette en gruppe

Dette emnet beskriver oppretting av grupper.

**Tillatelse til å opprette en gruppe**

Kontroller at du er autorisert til å opprette en ny gruppe. Globale administratorer kan deaktivere oppretting av grupper i Azure-portalen eller Access Panel. Du må kanskje ha en administrator for å opprette den nye gruppen for deg, eller for å gi deg nødvendige tillatelser.

**Behandle opprettelsestillatelser for grupper**

1. Globale administratorer kan administrere opprettelsestillatelser for grupper (av sikkerhetsrelaterte årsaker) eller Office 365-grupper som er opprettet i Azure-portalen eller accesspanelet, ved å velge «Brukere kan opprette sikkerhetsgrupper i Azure-portaler» eller «Brukere kan opprette Office 365-grupper i Azure Portals»-alternativene i Alle grupper Generelt   >  **(Innstillinger)**.
2. Du kan også begrense oppretting av grupper til å velge en gruppe brukere hvis du har en Azure Active Directory P1 Premium lisens.

**Deaktivere velkomstvarsel for nye Office 365 gruppemedlemmer**

Velkomstvarselet som sendes til brukere som er lagt til Office 365 grupper, kan deaktiveres ved å angi **UnifiedGroupWelcomeMessageEnabled** til False i Powershell. Finn ut mer om denne innstillingen [her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

