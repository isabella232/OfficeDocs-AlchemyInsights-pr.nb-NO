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
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992627"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Overvåkingslogger for SharePoint og OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Klassiske SharePoint-logger for sporing

SPO Legacy-overvåking ble overført til Unified overvåkingsloggen (manuell). Alle alle SPO eldre revisjonsrapporter vil nå bli drevet gjennom manuell, og de eldre revisjons signalene er overført til manuell.

Viktige endringer:

* Trimming er ikke tilgjengelig som en funksjon.
* Det er ikke mulig å velge bestemte hendelser som skal overvåkes. Se [dette dokumentet](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.
* Alternativet **plassering** under **tilpassede rapporter** er ikke tilgjengelig.
* Alternativet for **åpning eller nedlasting av dokumenter** hendelser er ikke tilgjengelig.

[Konfigurere overvåkingsinnstillinger for en områdesamling](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint og OneDrive moderne Unified overvåkingslogger fra samsvar

* [Slå på/av Unified Audit logging](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Ingen ekstra konfigurasjon kreves i SharePoint eller OneDrive.

Bruk sporing av overvåkingslogging til å kontrollere aktiviteten til filen (e), mappe (r), bruker (e), tillatelser:

* [Fil-og side aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mappe aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Dele og få tilgang til forespørsels aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniserings aktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter for områdeadministrasjon](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [søke i overvåkingsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
