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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657938"
---
# <a name="configure-endpoint-dlp"></a>Konfigurere hindring av datatap for endepunkt

Hindring av datatap for Microsoft endepunkt gir deg mulighet for å utvide beskyttelse og overvåking av hindring av datatap for sensitiv informasjon på Windows 10-enheter. Etter at enheter er pålastet i enhetsbehandling, kan du opprette policyer for hindring av datatap for å tvinge frem beskyttende handlinger på elementer. Aktivitetsutforsker kan brukes til å overvåke aktivitet for sensitive elementer. For mer informasjon, se [Pålasting av enheter i enhetsbehandling](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

For å komme i gang med hindring av datatap for endepunkt:

- Kontroller at du har den nødvendige SKU/abonnementlisensieringen. For mer informasjon, se [SKU/abonnementlisensiering](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Kontroller tillatelsene som er nødvendige for å aktivere enhetsbehandling, få tilgang til pålastingssiden, eller aktivere/deaktivere enhetsovervåking. Hvis du vil ha mer informasjon, kan du se [Tillatelser](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Pålast enheter i enhetsbehandling ved å følge prosedyren for pålasting av enheter. Hvis du vil ha mer informasjon, kan du se [Pålasting av enheter](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Opprett policyer for hindring av datatap for å beskytte sensitive elementer. For informasjon, se [Scenarier for policy for hindring av datatap for endepunkt](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

For mer informasjon om hindring av datatap for endepunkter, se [Lær om hindring av datatap for Microsoft 365-endepunkt (forhåndsversjon)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Viktige trinn for datainnsamling hvis du trenger støtte:**

1. Last [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Kjør verktøyet som administrator fra cmd-vinduet:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Når du blir bedt om det med Angi antall minutter for å samle inn **sporinger:** angir du hvor mange minutter som kreves for å kjøre scenarioet.
1. Kjør scenarioet.

Samle inn zip-filutdataene du vil gi til kundestøtterepresentanten.
