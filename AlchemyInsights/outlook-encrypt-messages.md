---
title: S/MIME i Outlook på nettet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772307"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptere e-postmeldinger i Outlook

Microsoft 365-meldings kryptering er bygd på Microsoft Azure Rights Management (Azure RMS), som er en del av Azure Information Protection. Hvis abonnementet omfatter Azure Rights Management eller Azure Information Protection, **trenger du ikke utføre handlinger for å aktivere eller aktivere** Rights Management-tjenesten manuelt.

Avhengig av tilbake melding fra kunder, vil vi ikke lenger aktivere Exchange-regler for e-postflyter for automatisk kryptering av utgående e-post som inneholder bestemt type sensitiv informasjon i leieren din som standard. I stedet gir vi detaljerte instruksjoner om hvordan du kan gjøre det selv. Hvis du vil ha mer informasjon om hvordan du oppretter en transport regel for å kryptere sensitiv informasjon, kan du se [denne artikkelen](https://aka.ms/OmeEtr).

- Hvis du bruker Outlook på nettet (tidligere **OWA**): Når du skriver en e-postmelding, klikker du bare **Beskytt** i OWA. Dette vil bruke «ikke Videresend»-tillatelsen. Klikk **endre tillatelse** , og velg **Krypter** for å bare kryptere meldingen.

- Hvis du bruker **Outlook-klient**: Hvis du vil sende en kryptert melding fra Outlook 2013 eller 2016, eller Outlook 2016 for Mac, velger du **Alternativer**  >  -**tillatelser**, og deretter velger du beskyttelses alternativet du trenger.

- Hvis du vil **kryptere alle e-postmeldinger** som er sendt til bestemte mottakere eller eksterne partner organisasjoner automatisk, må du opprette en e-postflyt transport regel i administrasjons senteret for Exchange. Du finner detaljerte instruksjoner i [denne kunde støtte artikkelen](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

