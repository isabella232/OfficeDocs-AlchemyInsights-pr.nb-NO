---
title: Distribusjon av gruppepolicyobjekt
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427565"
---
# <a name="gpo-deployment"></a>Distribusjon av gruppepolicyobjekt

Innstillinger for bruker- og datamaskinobjekter i Azure Active Directory Domain Services (Azure AD DS) behandles ofte ved hjelp av gruppepolicyobjekter (GPOs). Azure AD DS inneholder innebygde GPOs for AADDC-brukere og AADDC-datamaskinbeholdere. Du kan tilpasse disse innebygde gruppepolicyobjektene for å konfigurere gruppepolicy etter behov for miljøet. Medlemmer av administratorgruppen for Azure AD DC har administrasjonsrettigheter for gruppepolicyer i Azure AD DS-domenet, og kan også opprette egendefinerte GPO-er og organisasjonsenheter (OUs). Hvis du vil ha mer informasjon om hvilken gruppepolicy det er og hvordan den fungerer, kan du se [Oversikt over gruppepolicy.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

I et hybridmiljø synkroniseres ikke gruppepolicyer som er konfigurert i et lokalt AD DS-miljø, til Azure AD DS. Hvis du vil definere konfigurasjonsinnstillinger for brukere eller datamaskiner i Azure AD DS, redigerer du et av standard gruppepolicyobjektene eller oppretter et egendefinert gruppepolicyobjekt.

Denne artikkelen [Administrere gruppepolicy viser](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) deg hvordan du installerer verktøyene for gruppepolicybehandling, hvordan du redigerer de innebygde gpoene, og hvordan du oppretter egendefinerte GPOs.
