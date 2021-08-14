---
title: Kryptere bestemte e-postmeldinger automatisk fra Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988844"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Kryptere bestemte e-postmeldinger automatisk fra Office 365

1. I [administrasjonssenteret Exchange](https://outlook.office365.com/ecp/)velger du **e-postflyt > regler**. 
2. Klikk Ny **(+)-ikonet,** og klikk **deretter Bruk Office 365-meldingskryptering og rettighetsbeskyttelse på meldinger.**
3. Skriv **inn** et navn på regelen i Navn , for eksempel *Krypter alle meldinger*.
4. I **Bruk denne regelen hvis** velger du **[Bruk på alle meldinger]**. 
5. Klikk Velg et ved siden **av** Gjør **følgende-feltet.** 
6. Velg Krypter på rullegardinmenyen for **RMS-malen,** og klikk deretter **OK**. (Hvis du ikke ser dette alternativet, betyr det at planen ikke inkluderer automatisk kryptering. Men du kan legge den til!)
7. Merk av **for Overvåk denne** regelen med alvorsgrad, og velg deretter ønsket nivå. Hvis firmaet har kontraktsmessige forpliktelser til å sende alle e-postmeldinger kryptert, anbefaler jeg å sette nivået til **Høy**.
8. Klikk **Påtving under** Velg en modell for denne **regelen.** 
9. Velg et valgfritt utvalg (fra en liste over valgfrie valg som du kan gjøre på dette tidspunktet, hvorav mange kan stå igjen med standardinnstillingen for enkelhet).
10. Klikk på **Lagre**.

> [!IMPORTANT]
> Du kan alltid komme tilbake og redigere denne regelen senere.

Hvis du vil ha mer informasjon om hvordan du oppretter regler for kryptering, kan du se Definere regler for e-postflyt for [å kryptere e-postmeldinger Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

