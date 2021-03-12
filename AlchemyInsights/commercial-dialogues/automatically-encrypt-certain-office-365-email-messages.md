---
title: Kryptere bestemte Office 365-e-postmeldinger automatisk
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749439"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Kryptere bestemte Office 365-e-postmeldinger automatisk

Du kan automatisk kryptere meldinger som brukere sender til bestemte eksterne personer eller organisasjoner. Hvis du vil gjøre dette, utfører du følgende trinn:

1. Velg [e-postflyt i](https://outlook.office365.com/ecp/) **administrasjonssenteret for** Exchange > regler . 
2. Klikk på **Nytt (+)-ikonet,** og klikk deretter Bruk Meldingskryptering og rettighetsbeskyttelse for **Office 365 på meldinger.**
3. Skriv **inn** et navn på regelen i Navn, for eksempel Krypter *meldinger som sendes til DrToniRamos@gmail.com*.
4. I **Bruk denne regelen hvis** velger du Mottakeren > denne **personen**. 
5. Velg navnet **på** personen du vil at krypteringsregelen skal gjelde for, i Velg **medlemmer-vinduet,** og klikk deretter legg til . 
6. Når du er ferdig med å legge til brukere, klikker du **OK**.
7. Klikk Velg et ved siden **av** Gjør **følgende-feltet.** 
8. Velg Krypter på rullegardinmenyen for **RMS-malen,** og klikk deretter **OK**. (Hvis du ikke ser dette alternativet, betyr det at planen ikke inkluderer automatisk kryptering. Men du kan legge den til!)
9. Velg et valgfritt utvalg (fra en liste over valgfrie valg som du kan gjøre på dette tidspunktet, hvorav mange kan stå igjen med standardinnstillingen for enkelhet).
10. Klikk på **Lagre**.

> [!IMPORTANT]
> Du kan alltid komme tilbake og redigere denne regelen senere.

Hvis du vil ha mer informasjon om hvordan du oppretter regler for kryptering, kan du se Definere regler for e-postflyt for [å kryptere e-postmeldinger i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

