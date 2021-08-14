---
title: Problemer med administratorsamtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952582"
---
# <a name="admin-consent-issues"></a>Problemer med administratorsamtykke

1. Aktiver [arbeidsflyten for administratorsamtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) slik at brukere kan be om administratorgodkjenning direkte fra skjermbildet for samtykke.

1. Hvis du eller brukerne av programmet ser uventede feil under samtykkeprosessen, kan du se denne artikkelen for feilsøkingstrinn: Uventet feil når du gir samtykke [til et program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Finn ut mer [om administratorsamtykke](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) på Microsofts identitetsplattform, hvordan samtykkemeldingen fungerer og hvordan du evaluerer en forespørsel om administratorsamtykke for hele [leieren.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)

1. Programmer som integreres med Microsofts identitetsplattform, følger en autorisasjonsmodell som gir brukere og administratorer kontroll over hvordan data kan nås. Implementeringen av autorisasjonsmodellen er oppdatert på Microsofts identitetsplattform endepunktet, og den endrer hvordan en app må samhandle med Microsofts identitetsplattform. Se [Tillatelser og samtykke i Microsofts identitetsplattform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for en oversikt over denne godkjenningsmodellen, inkludert omfang, tillatelser og samtykke.