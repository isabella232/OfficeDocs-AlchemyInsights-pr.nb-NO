---
title: La en bruker synkronisere en personlig konto med jobbkontoen i Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813401"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>La en bruker synkronisere en personlig konto med jobbkontoen i Microsoft Edge

Kontroller at du oppfyller disse kriteriene:

- Roaming for virksomhetsstatus er aktivert i administrasjonssenteret for Azure Active Directory, som krever et abonnement på Azure Active Directory Premium eller Enterprise Mobility + Security (EMS). Hvis du vil ha mer informasjon, kan du se [Aktivere roaming](/azure/active-directory/devices/enterprise-state-roaming-enable)av virksomhetsstatus i Azure Active Directory .
- Ett eller begge av følgende vilkår oppfylles:
    - Azure Information Protection-tjenesten er aktivert for leieren. Hvis du vil ha mer informasjon, kan du se [Aktivere Beskyttelse mot Azure Rights Management fra Administrasjonssenter for Microsoft 365](/azure/information-protection/activate-office365).
    - Funksjonen Azure Active Directory Enterprise State Roaming (ESR) er aktivert for alle brukere eller tenanter. Hvis du vil ha mer informasjon, [kan du se Hva er roaming for virksomhetsstatus?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Hvis både AIP og ESR er deaktivert, vises en feilmelding om at synkronisering ikke er tilgjengelig for kontoene deres.
