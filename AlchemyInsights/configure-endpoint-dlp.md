---
title: Konfigurere hindring av datatap for endepunkt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402442"
---
# <a name="configure-endpoint-dlp"></a>Konfigurere hindring av datatap for endepunkt

Hindring av datatap for Microsoft endepunkt gir deg mulighet for å utvide beskyttelse og overvåking av hindring av datatap for sensitiv informasjon på Windows 10-enheter. Etter at enheter er pålastet i enhetsbehandling, kan du opprette policyer for hindring av datatap for å tvinge frem beskyttende handlinger på elementer. Aktivitetsutforsker kan brukes til å overvåke aktivitet for sensitive elementer. For mer informasjon, se [Pålasting av enheter i enhetsbehandling](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

For å komme i gang med hindring av datatap for endepunkt:

- Kontroller at du har den nødvendige SKU/abonnementlisensieringen. For mer informasjon, se [SKU/abonnementlisensiering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontroller tillatelsene som er nødvendige for å aktivere enhetsbehandling, få tilgang til pålastingssiden, eller aktivere/deaktivere enhetsovervåking. Hvis du vil ha mer informasjon, kan du se [Tillatelser](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Pålast enheter i enhetsbehandling ved å følge prosedyren for pålasting av enheter. Hvis du mangler alternativet pålasting av enheter (forhåndsversjon) under **Innstillinger** for M365-samsvar, bekreft at du har den nødvendige lisensen og tillatelser som referert over. Hvis du vil ha mer informasjon, kan du se [Pålasting av enheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Opprett policyer for hindring av datatap for å beskytte sensitive elementer. For informasjon, se [Scenarier for policy for hindring av datatap for endepunkt](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

For mer informasjon om hindring av datatap for endepunkter, se [Lær om hindring av datatap for Microsoft 365-endepunkt (forhåndsversjon)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Viktige trinn for datainnsamling hvis du trenger støtte:**

1. Last ned forhåndsversjon av MDATP Client Analyzer fra [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Kjør verktøyet som administrator fra cmd-vinduet:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Når du blir bedt om “Skriv inn antall minutter for innsamling av spor: “, skriv inn antall minutter som trengs for å kjøre scenariet
5. Kjør scenariet

Samle inn Zip-fil-utdata som skal gis til kundestøtterepresentanten.
