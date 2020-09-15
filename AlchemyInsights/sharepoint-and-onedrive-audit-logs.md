---
title: Klassiske rapporter for overvåkings Logg for SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662217"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Overvåkings logger for SharePoint og OneDrive

## <a name="sharepoint-classic-audit-logs"></a>SharePoint-klassiske overvåkings logger

SPO eldre overvåking ble overført til Unified Audit log (UAL). Alle SPO eldre overvåkings rapporter blir nå slått på via UAL, og de eldre overvåkings signalene har blitt overført til UAL.

Taste endringer:

* Trimming er ikke tilgjengelig som en funksjon.
* Det er ikke mulig å velge bestemte hendelser som skal overvåkes. Se [dette dokumentet](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.
* **Plasserings** alternativet under **tilpassede rapporter** er ikke tilgjengelig.
* Alternativet for **åpning eller nedlasting av dokument** hendelser er ikke tilgjengelig.

[Konfigurere overvåkings innstillinger for en nettsteds samling](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Overvåkede overvåkings logger for SharePoint og OneDrive fra samsvar

* [Aktivere/deaktivere Unified revisjons logging](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Ingen ekstra konfigurasjon kreves i SharePoint eller OneDrive.

Bruk overvåkings logging søk til å kontrollere aktivitet i filen (e), mappe (r), bruker (e), tillatelser:

* [Fil-og side aktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mappe aktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktiviteter for Delings-og tilgangs forespørsler](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synkroniserings aktiviteter](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktiviteter for nettsteds administrasjon](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [søke i overvåkings loggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
