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
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323927"
---
# <a name="configure-endpoint-dlp"></a>Konfigurere hindring av datatap for endepunkt

Hindring av datatap for Microsoft endepunkt gir deg mulighet for å utvide beskyttelse og overvåking av hindring av datatap for sensitiv informasjon på Windows 10-enheter. Etter at enheter er pålastet i enhetsbehandling, kan du opprette policyer for hindring av datatap for å tvinge frem beskyttende handlinger på elementer. Aktivitetsutforsker kan brukes til å overvåke aktivitet for sensitive elementer. For mer informasjon, se [Pålasting av enheter i enhetsbehandling](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

For å komme i gang med hindring av datatap for endepunkt:

- Kontroller at du har den nødvendige SKU/abonnementlisensieringen. For mer informasjon, se [SKU/abonnementlisensiering](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontroller tillatelsene som er nødvendige for å aktivere enhetsbehandling, få tilgang til pålastingssiden, eller aktivere/deaktivere enhetsovervåking. Hvis du vil ha mer informasjon, kan du se [Tillatelser](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Pålast enheter i enhetsbehandling ved å følge prosedyren for pålasting av enheter. Hvis du vil ha mer informasjon, kan du se [Pålasting av enheter](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Opprett policyer for hindring av datatap for å beskytte sensitive elementer. For informasjon, se [Scenarier for policy for hindring av datatap for endepunkt](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

For mer informasjon om hindring av datatap for endepunkter, se [Lær om hindring av datatap for Microsoft 365-endepunkt (forhåndsversjon)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Viktige trinn for datainnsamling hvis du trenger støtte:**

1. Last [ned forhåndsvisningen av MDATP Client Analyzer](https://aka.ms/betamdatpanalyzer).
1. Kjør verktøyet som administrator fra cmd-vinduet:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Når du blir bedt om det med Angi antall minutter for å samle inn **sporinger:** angir du hvor mange minutter som kreves for å kjøre scenarioet.
1. Kjør scenarioet.

Samle inn zip-filutdataene du vil gi til kundestøtterepresentanten.
