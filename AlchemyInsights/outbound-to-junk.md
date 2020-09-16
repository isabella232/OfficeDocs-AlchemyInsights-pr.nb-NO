---
title: Utgående e-post til søppel post mappen
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
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769192"
---
# <a name="outbound-email-to-junk-email-folder"></a>Utgående e-post til søppel post mappen

Hvis du ser utgående meldinger som blir merket som søppel post, gjør du følgende:

- Hvis du ikke allerede har gjort det, bør du vurdere å [konfigurere policyer for utgående søppel post](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).

- Bruk [meldings sporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) til å se om den utgående meldingen har hendelses verdien **søppel post** med tilleggs detaljene: **Bruk høy risiko for leverings utvalg**.

  For disse meldingene kontrollerer du meldings innholdet for å se hva som kan anses som søppel post. Signaturer kan for eksempel noen ganger forårsake problemer for mange brukere.

  Hvis du har flere eksempler på legitime utgående meldinger som skal merkes som søppel post, åpner du en kunde støtte billett og ber kunde støtte agenten om å sende meldinger som falske positiver til vår søppel post analytikere. Vær klar til å gi eksempel meldinger som inneholder alle meldings hodene.
