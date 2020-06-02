---
title: 2681 Attack Simulator i Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506747"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator i Microsoft 365

- Mangler du Attack Simulator? Attack Simulator krever **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** eller **Office 365 Enterprise E5**. Attack Simulator er **ikke** inkludert i Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 eller microsoft 365 Apps for business-abonnementer.

- Kontoen du bruker til å starte simulerte angrep, krever globale administrator- eller sikkerhetsadministratortillatelser og multifaktorautentisering (MFA). Hvis du vil ha mer informasjon om krav til Attack Simulator, kan du se [dette emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Viktige ting å vite om **Brute Force Passord** angrep simuleringer:

  - Hvis målkontoen har aktivert MFA og passordet ble gjettet riktig, vises ikke kontoen som kompromittert (den andre godkjenningsfaktoren vil være ufullstendig).

  - Passordfilen kan ikke være større enn 10 MB. Bruk ett passord per linje, og ta med en tom linje (vognretur) etter det siste passordet i listen.

- Viktige ting å vite om **Spear Phishing** feste simuleringer:

  - Ved utforming kan du ikke angi en egendefinert verdi for **URL-adresse for phishing-påloggingsserver .**

  - Hvis en mottaker bruker [tillegget Aktiver rapportmelding](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til å rapportere meldingen som phishing, kan det hende du ikke mottar varsler for meldingen (fordi dette er et simulert angrep).

- Rapporter: Når det simulerte angrepet er fullført, kan du klikke på **Angrepsdetaljer** for å se rapporten.

- Hvis du vil ha detaljerte instruksjoner og nye funksjoner i Attack Simulator, kan du se [Attack Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
