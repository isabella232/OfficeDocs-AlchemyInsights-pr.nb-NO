---
title: Oppdatere navneserveren til å peke til Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: d9d66e366db14840a86b681deba78b89ddff5e068a3b931c88e493d2ec791b10
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073609"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Oppdatere navneserveren til å peke til Microsoft

Obs! Noen ganger kan det ta opptil 48 timer før endringer i navneserverne overføres.
  
Hvis du vil konfigurere domenet med Microsoft, må navneserverne hos registratoren oppdateres. Opprette eller redigere navneserverpostene hos domeneregistratoren.
  
1. Gå til domeneregistratorens nettsted og finn området der du kan redigere navneserverne.

2. Opprett eller rediger to navneserverposter slik at de samsvarer med disse verdiene:

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. Lagre endringer.

Du finner også detaljerte instruksjoner i denne artikkelen: Endre navneservere for å konfigurere Microsoft 365 med en hvilken som helst [domeneregistrator](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)
  