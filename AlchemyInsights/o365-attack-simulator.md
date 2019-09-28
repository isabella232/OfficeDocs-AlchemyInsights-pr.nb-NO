---
title: 2681 angrep Simulator i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305340"
---
# <a name="attack-simulator-in-office-365"></a>Attack Simulator i Office 365

- Er du mangler Attack Simulator? Attack Simulator krever **office 365 avansert trusselbeskyttelse plan 2 (ATP-plan 2)** eller **Office 365 Enterprise E5**. Attack Simulator er **ikke** inkludert i Office 365 avansert trussel beskyttelses plan 1 (ATP-plan 1), Office 365 Enterprise E3 eller noen Office 365 Business-abonnementer.

- Kontoen du bruker til å starte simulerte angrep, krever global administrator-eller sikkerhetsadministrator tillatelser og multifaktorautentisering (MFA). Hvis du vil ha mer informasjon om Attack Simulator-krav, kan du se [dette emnet](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Viktige ting å vite om **Brute Force passord** angrep simuleringer:

  - Hvis målkontoen har MFA aktivert og passordet ble gjettet riktig, vil kontoen ikke vises som kompromittert (den andre godkjennings faktoren vil være ufullstendig).

  - Passord filen kan ikke være større enn 10 MB. Bruk ett passord per linje, og ta med en tom linje (vognretur) etter det siste passordet i listen.

- Viktige ting å vite om **spyd phishing** feste simuleringer:

  - Som standard kan du ikke angi en egendefinert verdi for **URL-adressen for phishing-pålogging**.

  - Hvis en mottaker bruker [Aktiver rapportmelding-tillegget](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) for å rapportere meldingen som phishing, kan det hende du ikke mottar varsler for meldingen (fordi dette er et simulert angrep).

- Rapporter: etter at det simulerte angrepet er fullført, kan du klikke på **angreps detaljer** for å se rapporten.

- Hvis du vil ha detaljerte instruksjoner og nye funksjoner i Attack Simulator, kan du se [Attack Simulator i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
