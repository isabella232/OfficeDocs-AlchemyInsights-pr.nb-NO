---
title: Gruppepolicy
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256782"
---
# <a name="group-policy"></a>Gruppepolicy

Innstillinger for bruker- og datamaskinobjekter i Azure Active Directory Domain Services (Azure AD DS) behandles ofte ved hjelp av gruppepolicyobjekter (GPOs). Azure AD DS inneholder innebygde GPOs for AADDC-brukere og AADDC-datamaskinbeholdere. Du kan tilpasse disse innebygde gruppepolicyobjektene for å konfigurere gruppepolicy etter behov for miljøet. Medlemmer av administratorgruppen for Azure AD DC har administrasjonsrettigheter for gruppepolicyer i Azure AD DS-domenet, og kan også opprette egendefinerte GPO-er og organisasjonsenheter (OUs). Hvis du vil ha mer informasjon om hvilken gruppepolicy det er og hvordan den fungerer, kan du se [Oversikt over gruppepolicy.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

I et hybridmiljø synkroniseres ikke gruppepolicyer som er konfigurert i et lokalt AD DS-miljø, til Azure AD DS. Hvis du vil definere konfigurasjonsinnstillinger for brukere eller datamaskiner i Azure AD DS, redigerer du et av standard gruppepolicyobjektene eller oppretter et egendefinert gruppepolicyobjekt.

Denne artikkelen [Administrere gruppepolicy viser](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) deg hvordan du installerer verktøyene for gruppepolicybehandling, hvordan du redigerer de innebygde gpoene, og hvordan du oppretter egendefinerte GPOs.



