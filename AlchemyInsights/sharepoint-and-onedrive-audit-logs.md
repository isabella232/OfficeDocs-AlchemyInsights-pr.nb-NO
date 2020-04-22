---
title: Klassiske rapporter for SharePoint-overvåkingslogg
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741974"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint- og OneDrive-overvåkingslogger

## <a name="sharepoint-classic-audit-logs"></a>Klassiske overvåkingslogger for SharePoint

SPO eldre revisjon ble overført til Unified Audit Log (UAL). Alle SPO eldre revisjonsrapporter vil nå bli drevet gjennom UAL, og de eldre revisjonssignalene er overført til UAL.

Viktige endringer:

* Trimming er IKKE tilgjengelig som en funksjon.
* Velge bestemte hendelser som skal revideres er IKKE tilgjengelig. Se [dette dokumentet](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.
* **Alternativet Plassering** under **Tilpassede rapporter** er IKKE tilgjengelig.
* Alternativet **Åpne eller laste ned dokumenter** hendelser er IKKE tilgjengelig.

[Konfigurere overvåkingsinnstillinger for en områdesamling](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint- og OneDrive Modern Unified-overvåkingslogger fra samsvar

* [Aktivere/deaktivere logging av enhetlig revisjon](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Ingen ekstra konfigurasjon er nødvendig i SharePoint eller OneDrive.

Bruk søk i overvåkingslogging til å kontrollere aktiviteten til filen(e), mappen(e), bruker(er), tillatelser:

* [Fil- og sideaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Mappeaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Dele og få tilgang til forespørselsaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsaktiviteter](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter for områdeadministrasjon](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [Søke i overvåkingsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
