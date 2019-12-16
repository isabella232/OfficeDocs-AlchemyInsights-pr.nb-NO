---
title: S/MIME i Outlook på weben
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053234"
---
# <a name="encrypt-email-messages-in-outlook"></a>Krypter e-postmeldinger i Outlook

Office 365 meldingskryptering er bygd på Microsoft Azure Rights Management (Azure RMS), som er en del av Azure Information Protection. Hvis abonnementet inkluderer Azure Rights Management eller Azure Information Protection, **trenger du ikke utføre noen handlinger for å aktivere eller aktivere** Rights Management-tjenesten manuelt.

Basert på tilbakemeldinger fra kunder, vil vi ikke lenger aktivere Exchange e-post flyt regler for å automatisk kryptere utgående e-post som inneholder visse typer sensitiv informasjon i leieren som standard. I stedet gir vi detaljerte instruksjoner om hvordan du kan gjøre det selv. Hvis du vil ha mer informasjon om hvordan du oppretter en regel for transport for å kryptere sensitiv informasjon, kan du se [denne artikkelen](https://aka.ms/OmeEtr).

- Hvis du bruker Outlook på weben (tidligere **OWA**): Når du skriver en e-postmelding, klikker du bare **Beskytt** i OWA. Dette vil gjelde "ikke Videresend" tillatelse. Klikk **endre tillatelse** , og velg **Krypter** for å bare kryptere meldingen.

- Hvis du **bruker Outlook-klienten**: Hvis du vil sende en kryptert melding fra Outlook 2013 eller 2016 eller Outlook 2016 for Mac, velger du **Alternativer** > -**tillatelser**, og deretter velger du beskyttelses alternativet du trenger.

- Hvis du **automatisk vil kryptere all e-post** som sendes til bestemte mottakere eller eksterne partner organisasjoner, må du opprette en transport regel for e-postflyt i administrasjonssenteret for Exchange. Du finner detaljerte instruksjoner i [denne kundestøtteartikkelen](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

