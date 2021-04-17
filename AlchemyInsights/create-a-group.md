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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816365"
---
# <a name="create-a-group"></a>Opprette en gruppe

Dette emnet beskriver oppretting av grupper.

**Tillatelse til å opprette en gruppe**

Kontroller at du er autorisert til å opprette en ny gruppe. Globale administratorer kan deaktivere oppretting av grupper i Azure-portalen eller Access Panel. Du må kanskje ha en administrator for å opprette den nye gruppen for deg, eller for å gi deg nødvendige tillatelser.

**Behandle opprettelsestillatelser for grupper**

1. Globale administratorer kan administrere opprettelsestillatelser for grupper (av sikkerhetsrelaterte årsaker) eller Office 365-grupper som er opprettet i Azure-portalen eller accesspanelet, ved å velge «Brukere kan opprette sikkerhetsgrupper i Azure-portaler» eller «Brukere kan opprette Office 365-grupper i Azure Portals»-alternativer i Alle grupper Generelt  >  **(Innstillinger)**.
2. Du kan også begrense oppretting av grupper til å velge en gruppe brukere hvis du har en Azure Active Directory P1 Premium-lisens.

**Deaktivere velkomstvarsel for nye Medlemmer i Office 365-gruppen**

Velkomstvarselet som sendes til brukere som er lagt til i Office 365-grupper, kan deaktiveres ved å angi **UnifiedGroupWelcomeMessageEnabled** til False i Powershell. Finn ut mer om denne innstillingen [her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

