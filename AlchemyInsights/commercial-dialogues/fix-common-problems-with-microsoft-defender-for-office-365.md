---
title: Løs vanlige problemer med Microsoft Defender for Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898253"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Løs vanlige problemer med Microsoft Defender for Office 365

Her er noen løsninger på vanlige problemer med Microsoft Defender for Office 365:

- **Meldingsforsinkelse:**

  Forsinkelser i levering av e-post kan være årsak Safe skanning av vedlegg i meldinger. Hvis du vil ha mer [informasjon, Safe policyinnstillinger](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)for vedlegg .

- **Rapporter falske positive eller negative resultater:**

  Hvis du vil ha mer informasjon, [kan du se Rapportere meldinger og filer til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Aktiver Safe koblingsbeskyttelse:**

  1. I Microsoft 365 Defender-portalen på går du til Policyer & for e-post & policyer Safe <https://security.microsoft.com/>  \>  \>  \> **koblinger** i **Policyer-delen.**

     Hvis du vil gå direkte **til Safe koblinger-siden,** bruker du <https://security.microsoft.com/safelinksv2> .

  2. Velg **policyen Safe** på siden Koblinger ved å klikke navnet på policyen.
  3. Gjør ett av følgende i undermenyen for detaljer som vises:
     - Hvis du vil legge til en ny policy, **velger du + Opprett**. En veiviser starter for å hjelpe deg med å definere policyinnstillingene.
     - Hvis du vil redigere en eksisterende policy, velger du policyen ved å klikke på navnet på policyen. Velg Rediger i delen Beskyttelsesinnstillinger på detaljer-undermenyen som vises.  
  4. Konfigurer **følgende innstillinger på** siden Beskyttelsesinnstillinger:
     - Aktiver **Velg handlingen for ukjente potensielt skadelige nettadresser i meldinger**.
     - Velg **Bruk klarerte koblinger på meldinger som sendes i organisasjonen**.

  Hvis du vil ha mer informasjon, [kan du se Konfigurere Safe koblingspolicyer i Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies).
