---
title: API-tillatelser og samtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975000"
---
# <a name="api-permissions-and-consent"></a>API-tillatelser og samtykke

Programmer som integreres med Microsoft Identity Platform, følger en Autorisasjons modell som gir brukere og administratorer kontroll over hvordan data kan nås. Implementeringen av Autorisasjons modellen er oppdatert på Microsoft Identity Platform Endpoint. Den endrer hvordan en app må samhandle med Microsoft Identity Platform. [Tillatelser og samtykke i Microsoft Identity Platform Endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) dekker de grunnleggende konseptene til denne Autorisasjons modellen, inkludert omfang, tillatelser og samtykke.

[Azure Active Directory (Azure ad) samtykke rammeverk](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) gjør det enkelt å utvikle nett og opprinnelige klient programmer med flere Tenant. Disse programmene tillater pålogging av bruker kontoer fra en Azure AD-leier som er forskjellig fra den som programmet er registrert i. Det kan også hende at de trenger tilgang til nett-APIer, for eksempel Microsoft Graph API (for å få tilgang til Azure AD, Intune og tjenester i Microsoft 365) og andre Microsoft Services-APIer, i tillegg til dine egne nett BAS-APIer.

