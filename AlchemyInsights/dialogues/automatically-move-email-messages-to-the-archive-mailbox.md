---
title: Flytte e-postmeldinger til arkivpostboksen automatisk
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527105"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Flytte e-postmeldinger til arkivpostboksen automatisk

Slik konfigurerer du en policy slik at en brukers gamle e-post flyttes automatisk til arkivpostboksen:

1. Gå til [**Sikkerhet & for**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **samsvarsdatastyringsarkivet** for å bekrefte at en  >   arkivpostboks er aktivert for brukeren. Hvis den ikke har det, klikker du **Aktiver** og **deretter Ja** i advarselen.
2. Gå til [**administrasjonssenteret for Exchange > for samsvarsbehandling > oppbevaringskoder.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Velg +-ikonet, og velg **deretter automatisk bruk på hele postboksen.**
4. Tilordne et navn til oppbevaringskoden, og velg **Flytt til arkiv.** Angi ønsket tid for oppbevaringsperioden, for eksempel 90 dager. Klikk på **Lagre**.
5. Nå kan du opprette en **oppbevaringspolicy: velg** oppbevaringspolicyer, velg ikonet for å legge til en ny policy.
6. Tilordne et navn til oppbevaringspolicyen, og klikk og rull for å finne og legge til oppbevaringskoden du nettopp opprettet. Klikk på **Lagre**.
7. Til slutt bruker du oppbevaringspolicyen på brukerens postboks: Fortsatt i **administrasjonssenteret** for Exchange, gå til  >  **mottakerpostbokser.** Velg alle brukerne du vil bruke policyen på, og velg deretter **Rediger** (blyantikonet).
8. Klikk postboksfunksjoner i **dialogboksen.** Bruk **policyen du** nettopp opprettet under Oppbevaringspolicy, og > **Lagre.**
9. Hvis du vil ha instruksjoner for hvordan du bruker policyen på alle brukere, kan du se [Bruke en oppbevaringspolicy på postbokser.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
