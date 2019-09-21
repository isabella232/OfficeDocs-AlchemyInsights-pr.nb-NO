---
title: Klassiske overvåkingslogg rapporter for SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068032"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Overvåkingslogger for SharePoint og OneDrive

**SharePoint og OneDrive moderne Unified overvåkingslogger fra samsvar**

- [Slå på/av Unified Audit logging](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Ingen ekstra konfigurasjon kreves i SharePoint eller OneDrive.

- Bruk sporing av overvåkingslogging til å kontrollere aktiviteten til filen (e), mappe (r), bruker (e), tillatelser:

    - [Fil-og side aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Mappe aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Dele og få tilgang til forespørsels aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Synkroniserings aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Aktiviteter for områdeadministrasjon](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [søke i overvåkingsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Klassiske SharePoint-logger for sporing**

Vi overførte SPO eldre revisjon til Unified overvåkingsloggen (manuell). Dette betyr i hovedsak at alle SPO eldre revisjonsrapporter vil nå bli drevet gjennom manuell, og de eldre revisjons signalene har blitt overført til manuell.

Viktige endringer:

- Trimming som en funksjon er ikke tilgjengelig.
- Delen der du velger bestemte hendelser som skal overvåkes, er ikke tilgjengelig. Vennligst referer til [dette dokumentet](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.
- Alternativet "location" under **tilpassede rapporter** er ikke tilgjengelig. 
- Hendelser som åpner eller laster ned dokumenter, er ikke tilgjengelig. 

