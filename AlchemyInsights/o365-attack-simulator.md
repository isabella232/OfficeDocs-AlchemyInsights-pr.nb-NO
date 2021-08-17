---
title: 2681 Attack Simulator i Microsoft 365
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
- "2681"
ms.assetid: ''
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895800"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angrepssimulator i Microsoft 365

- Mangler du Angrepssimulator? Attack Simulator krever **Microsoft Defender for Office 365 Plan 2** **eller Office 365 Enterprise E5**. Attack Simulator er **ikke** inkludert i Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3 eller noen Microsoft 365 Apps for business abonnementer.

- Kontoen du bruker til å starte simulerte angrep, krever globale administrator- eller sikkerhetsadministratortillatelser og godkjenning med flere faktorer (MFA). Hvis du vil ha mer informasjon om angrepssimulatorkrav, kan du [se dette emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Viktige ting du må vite om **Angrepssimuleringer for Brute Force-passord:**

  - Hvis målkontoen har aktivert MFA og passordet ble gjettet riktig, vises ikke kontoen som kompromittert (den andre godkjenningsfaktoren vil være ufullstendig).

  - Passordfilen kan ikke være større enn 10 MB. Bruk ett passord per linje, og inkluder en tom linje (retur) etter det siste passordet i listen.

- Viktige ting du må vite om å legge ved **simulasjoner for Phishing-phishing:**

  - Som utforming kan du ikke angi en egendefinert verdi for nettadressen for **phishing-påloggingsserveren**.

  - Hvis en mottaker bruker [tillegget](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Aktiver rapportmelding til å rapportere meldingen som phishing, mottar du kanskje ikke varsler for meldingen (fordi dette er et simulert angrep).

- Rapporter: Når det simulerte angrepet er fullført, kan du klikke **Angrepsdetaljer** for å se rapporten.

- Hvis du vil ha detaljerte instruksjoner og nye funksjoner i Attack Simulator, kan du se [Angrepssimulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
