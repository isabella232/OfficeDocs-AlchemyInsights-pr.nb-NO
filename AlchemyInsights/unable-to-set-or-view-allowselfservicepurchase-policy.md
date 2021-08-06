---
title: Kan ikke angi eller vise AllowSelfServicePurchase-policyen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020201"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Kan ikke angi eller vise AllowSelfServicePurchase-policyen

Når du prøver å angi eller vise AllowSelfServicePurchase-policyen, får du følgende feilmelding:

*HandleError: Kan ikke hente produktpolicy med PolicyId 'AllowSelfServicePurchase', ErrorMessage – Den underliggende tilkoblingen ble lukket: Det oppstod en uventet feil under sending.*

Dette kan skyldes en eldre versjon av Transport Layer Security (TLS). Hvis du vil koble til MSCommerce-tjenesten, må du bruke TLS 1.2 eller større.  

Prøv følgende trinn for å aktivere/sette TLS-protokollen til 1.2, bekrefte og prøve på nytt.
 1. I PowerShell-ledeteksten (PS C: skriver du inn følgende kommando for å angi \) TLS-protokollen til versjon 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Bekreft TLS-protokollen(e) som er i bruk, med følgende kommando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Forsøk kommandoene Hent eller Oppdater etter behov.

