---
title: 2681-angreps Simulator i Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759228"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angripe Simulator i Microsoft 365

- Mangler du angripe Simulator? Angreps Simulator krever **Office 365 Advanced Threat Protection Plan 2 (ATP plan 2)** eller **Office 365 Enterprise E5**. Angripe Simulator er **ikke** inkludert i Office 365 Advanced Threat Protection Plan 1 (ATP plan 1), Office 365 Enterprise E3 eller noen Microsoft 365-apper for forretnings abonnementer.

- Kontoen du bruker til å starte simulerte angrep, krever globale administrator-eller sikkerhets administrator tillatelser og godkjenning med flere faktorer (MFA). Hvis du vil ha mer informasjon om krav til angrep, kan du se [dette emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Viktige ting å vite om **Brute Force passord** angreps simuleringer:

  - Hvis mål kontoen har MFA aktivert og passordet ble antatt riktig, vises ikke kontoen som utsatt (den andre godkjennings faktoren blir ikke fullført).

  - Passord filen kan ikke være større enn 10 MB. Bruk ett passord per linje, og Inkluder en tom linje (vogn retur) etter det siste passordet i listen.

- Viktige ting å vite om **spear phishing** attach-simuleringer:

  - Som standard kan du ikke gi en egen definert verdi for **URL-adresse for phishing-påloggingsserver**.

  - Hvis en mottaker bruker [tillegget Aktiver rapport melding](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til å rapportere meldingen som phishing, kan du kanskje ikke motta varsler for meldingen (fordi dette er et simulert angrep).

- Rapporter: når det simulerte angrepet er fullført, kan du klikke på **angripe detaljer** for å se rapporten.

- Hvis du vil ha detaljerte instruksjoner og nye funksjoner i angripe Simulator, kan du se [angripe Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
