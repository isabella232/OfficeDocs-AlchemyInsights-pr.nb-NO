---
title: Kan ikke angi eller vise policyen AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091738"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Kan ikke angi eller vise policyen AllowSelfServicePurchase

Når du prøver å angi eller vise policyen AllowSelfServicePurchase, får du følgende feilmelding:

*HandleError : Kan ikke hente produktpolicy med PolicyId 'AllowSelfServicePurchase', ErrorMessage - Den underliggende tilkoblingen ble lukket: Det oppstod en uventet feil ved sending.*

Dette kan skyldes en eldre versjon av Transport Layer Security (TLS). Hvis du vil koble til MSCommerce-tjenesten, må du bruke TLS 1.2 eller nyere.  

Prøv følgende trinn for å aktivere/sette TLS-protokollen til 1.2, kontrollere og prøve på nytt.
 1. Ved PowerShell-ledeteksten (PS\) C: skriv inn følgende kommando for å sette TLS-protokollen til versjon 1.2:

    \[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12

2. Kontroller TLS-protokollen(e) som er i bruk, med følgende kommando:

    \[Net.ServicePointManager]::SecurityProtocol 

3. Prøv kommandoene Hent eller Oppdater på nytt etter behov.

