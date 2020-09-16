---
title: Kan ikke angi eller vise AllowSelfServicePurchase-policyen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735208"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Kan ikke angi eller vise AllowSelfServicePurchase-policyen

Når du prøver å angi eller vise AllowSelfServicePurchase-policyen, får du følgende feil melding:

*HandleError: kan ikke hente produkt policy med PolicyId ' AllowSelfServicePurchase ', ErrorMessage-den underliggende tilkoblingen ble lukket: Det oppstod en uventet feil under sendingen.*

Dette kan skyldes en eldre versjon av TLS (Transport Layer Security). Hvis du vil koble til MSCommerce-tjenesten, må du bruke TLS 1,2 eller nyere.  

Prøv følgende trinn for å aktivere/sette TLS-protokollen til 1,2, bekrefte og prøve på nytt.
 1. I PowerShell-ledeteksten (PS C: \) Angi følgende kommando for å angi TLS-protokollen til versjon 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Kontroller hvilken TLS-protokoll som er i bruk, med følgende kommando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Prøv kommandoene Hent eller oppdater på nytt etter behov.

