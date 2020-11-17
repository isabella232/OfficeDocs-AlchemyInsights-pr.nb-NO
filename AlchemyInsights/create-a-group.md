---
title: Opprette en gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088909"
---
# <a name="create-a-group"></a>Opprette en gruppe

Dette emnet beskriver opprettelse av grupper.

**Tillatelse til å opprette en gruppe**

Kontroller at du har tillatelse til å opprette en ny gruppe. Globale administratorer kan deaktivere opprettelse av grupper i Azure-portalen eller tilgangs panelet. Du trenger kanskje en administrator for å opprette den nye gruppen for deg, eller for å gi deg nødvendige tillatelser.

**Behandle tillatelser for opprettelse av grupper**

1. Globale administratorer kan behandle tillatelser for opprettelse av grupper (for sikkerhetsrelaterte årsaker) eller Office 365-grupper som er opprettet i Azure-portalen eller tilgangs panelet, ved å velge alternativene brukere kan opprette sikkerhets grupper i Azure-portaler eller brukere kan opprette Office 365-grupper i Azure-portaler i **alle grupper**  >  **Generelt (innstillinger)**.
2. Du kan også begrense opprettelsen av grupper for å velge en gruppe med brukere hvis du har en Azure Active Directory P1 Premium-lisens.

**Deaktivere velkommen varsling for nye medlemmer i Office 365-gruppen**

Velkommens varselet som sendes til brukere som er lagt til i Office 365-grupper, kan deaktiveres ved å angi **UnifiedGroupWelcomeMessageEnabled** til Usann i PowerShell. Lær mer om denne innstillingen [her](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

