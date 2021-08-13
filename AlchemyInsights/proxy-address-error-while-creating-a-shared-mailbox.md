---
title: Proxy-adressefeil under oppretting av en delt postboks
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062917"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Proxy-adressefeil under oppretting av en postboks eller et annet e-postaktivert objekt

Hvis du prøvde å opprette et e-postaktivert objekt (postboks, delt postboks osv.) og fikk feilmeldingen «Proxy-adressen «SMTP:alias@domain.com» brukes allerede...», er e-postadressen du valgte, allerede tatt av et annet e-postaktivert objekt i organisasjonen.
  
Du må finne brukeren, gruppen, den delte postboksen eller fellesmappen som har denne e-postadressen, og slette den eller endre e-postadressen. Deretter kan du opprette et nytt e-postaktivert objekt med den frigjorte e-postadressen. Bruk Søk på hjemmesiden for å finne det. Du kan også bruke følgende Exchange Online PowerShell-kommandoen til å søke etter den:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Hvis du ikke vil slette den eksisterende e-postadressen, velger du en ny e-postadresse for det nye objektet du oppretter.
  