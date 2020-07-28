---
title: Apple MDM Push Sertifikat er ikke satt opp
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440004"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push Sertifikat er ikke satt opp

Et Apple MDM Push Certificate (også kjent som et APPLE Push Notification Service(APNS)-sertifikat) er ikke konfigurert for abonnementet. Uten et Apple MDM Push Sertifikat konfigurert, kan du ikke registrere og administrere iOS- og Mac OS-enheter. Når du har lagt til sertifikatet i Intune, kan brukere installere Firmaportal-appen for å registrere iOS-enhetene sine.

1. Velg **"Jeg godtar."** for å gi Microsoft tillatelse til å sende data til Apple.

2. Velg **Last ned csr** intune sertifikatsigneringsforespørselen som kreves for å opprette et Apple MDM push-sertifikat. Filen brukes til å be om et klareringsrelasjonssertifikat fra Apple Push Certificates Portal.

3. Velg **Opprett MDM push-sertifikatet** for å gå til Apple Push Certificates Portal. Logg på med Apple ID-en for firmaet, og velg deretter **Opprett et sertifikat**. Velg **Velg fil**, bla til forespørselsfilen for sertifikatsignering, og velg deretter Last **opp**. Velg **Last ned** på Bekreftelse-siden for å laste ned sertifikatfilen (PEM), og lagre filen lokalt.
 
**Merk:** Sertifikatet er knyttet til Apple ID-en som brukes til å opprette det. Som en beste praksis, bruk en Apple ID for å administrere oppgaver, og kontroller at postboksen overvåkes av mer enn én person eller ved hjelp av en distribusjonsliste. Bruk aldri en personlig Apple-ID. Bruk samme Apple ID til å fornye Apple Push-sertifikatet hver 12.
 
4. Skriv inn Apple ID-en som brukes til å opprette Apple MDM push-sertifikatet ditt. Registrer denne ID-en som en påminnelse for når du trenger å fornye sertifikatet.

5. Gå til sertifikatfilen (PEM), velg **Åpne**, og velg deretter **Last opp**. Med push-sertifikatet kan Intune registrere og administrere Apple-enheter.