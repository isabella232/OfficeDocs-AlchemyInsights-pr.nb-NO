---
title: Rapporter for klassisk SharePoint-overvåkingslogg
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
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509609"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Overvåkingslogger for SharePoint og OneDrive

## <a name="sharepoint-classic-audit-logs"></a>SharePoint klassiske overvåkingslogger

SPO eldre revisjon ble overført til Unified Audit Log (UAL). Alle SPO eldre revisjonsrapporter vil nå bli drevet gjennom UAL, og de eldre revisjonssignalene er overført til UAL.

Viktige endringer:

* Trimming er IKKE tilgjengelig som en evne.
* Å velge bestemte hendelser som skal revideres er IKKE tilgjengelig. Se [dette dokumentet](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.
* Alternativet **Plassering** under **Tilpassede rapporter** er IKKE tilgjengelig.
* Alternativet **Åpne eller laste ned dokumenter** hendelser er IKKE tilgjengelig.

[Konfigurere overvåkingsinnstillinger for en områdesamling](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint og OneDrive moderne enhetlig overvåkingslogger fra samsvar

* [Aktivere/deaktivere logging av enhetlig revisjon](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Ingen ekstra konfigurasjon er nødvendig i SharePoint eller OneDrive.

Bruk søk etter overvåkingslogging til å kontrollere aktiviteten til filen(e), mappe(er), bruker(er), tillatelser:

* [Fil- og sideaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mappeaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Delings- og tilgangsforespørselsaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniseringsaktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter for administrasjon av nettsteder](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [Søke i overvåkingsloggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
