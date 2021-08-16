---
title: Krypter Office 365 e-postmeldinger som sendes til bestemte domener automatisk
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082195"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Krypter Office 365 e-postmeldinger som sendes til bestemte domener automatisk

1. I [administrasjonssenteret Exchange](https://outlook.office365.com/ecp/)velger du **e-postflyt > regler**. 
2. Klikk Ny **(+)-ikonet,** og klikk **deretter Bruk Office 365-meldingskryptering og rettighetsbeskyttelse på meldinger.**
3. Skriv **inn** et navn på regelen i Navn, for eksempel Krypter *meldinger som sendes til contoso.com*.
4. I **Bruk denne regelen hvis** velger du Mottakeren > domenet **er**. 
5. Skriv inn navnet på domenet, for eksempel **contoso.com**.
6. Klikk Legg **til (+)-ikonet,** og klikk deretter **OK**.
7. Klikk Velg et ved siden **av** Gjør **følgende-feltet.** 
8. Velg Krypter på rullegardinmenyen for **RMS-malen,** og klikk deretter **OK**. (Hvis du ikke ser dette alternativet, betyr det at planen ikke inkluderer automatisk kryptering. Men du kan legge den til!)
9. Velg et valgfritt utvalg (fra en liste over valgfrie valg som du kan gjøre på dette tidspunktet, hvorav mange kan stå igjen med standardinnstillingen for enkelhet).
10. Klikk på **Lagre**.

> [!IMPORTANT]
> Du kan alltid komme tilbake og redigere denne regelen senere.

Hvis du vil ha mer informasjon om hvordan du oppretter regler for kryptering, kan du se Definere regler for e-postflyt for [å kryptere e-postmeldinger Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)