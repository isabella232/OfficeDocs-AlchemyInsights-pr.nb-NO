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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067849"
---
# <a name="gpo-deployment"></a>Distribusjon av gruppepolicyobjekt

Innstillinger for bruker- og datamaskinobjekter i Azure Active Directory Domain Services (Azure AD DS) administreres ofte ved hjelp av gruppepolicyobjekter (GPOer). Azure AD DS inneholder innebygde gruppepolicyobjekter for AADDC-brukere og AADDC-datamaskiner-beholdere. Du kan tilpasse disse innebygde gruppepolicyobjektene for å konfigurere gruppepolicy etter behov for miljøet. Medlemmer av azure AD DC-administratorgruppen har administratorrettigheter for gruppepolicy i Azure AD DS-domenet, og kan også opprette egendefinerte gruppepolicyobjekter og organisasjonsenheter (OUs). Hvis du vil ha mer informasjon om hvilken gruppepolicy som er og hvordan den fungerer, kan du se [Oversikt over gruppepolicy](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

I et hybridmiljø synkroniseres ikke gruppepolicyer som er konfigurert i et lokalt AD DS-miljø, til Azure AD DS. Hvis du vil definere konfigurasjonsinnstillinger for brukere eller datamaskiner i Azure AD DS, redigerer du et av standard gruppepolicyobjektene eller oppretter et egendefinert gruppepolicyobjekt.

Denne artikkelen [Behandle gruppepolicy viser](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) deg hvordan du installerer verktøyene for gruppepolicybehandling, hvordan du redigerer de innebygde gruppepolicyobjektene og hvordan du oppretter egendefinerte gruppepolicyobjekter.
