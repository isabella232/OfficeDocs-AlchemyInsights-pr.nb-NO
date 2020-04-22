---
title: S/MIME i Outlook på nettet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764881"
---
# <a name="encrypt-email-messages-in-outlook"></a>Krypter e-postmeldinger i Outlook

Microsoft 365 Message Encryption er bygget på Microsoft Azure Rights Management (Azure RMS), som er en del av Azure Information Protection. Hvis abonnementet inkluderer Azure Rights Management eller Azure Information Protection, **trenger du ikke å gjøre noen handlinger for å aktivere eller aktivere** Rights Management-tjenesten manuelt.

Basert på tilbakemeldinger fra kunder, vil vi ikke lenger aktivere Exchange-regler for e-postflyt for automatisk å kryptere utgående e-post som inneholder visse typer sensitiv informasjon i leieren som standard. I stedet gir vi detaljerte instruksjoner om hvordan dere kan gjøre det selv. Hvis du vil ha mer informasjon om hvordan du oppretter en transportregel for å kryptere sensitiv informasjon, kan du se [denne artikkelen](https://aka.ms/OmeEtr).

- Hvis du bruker Outlook på weben (tidligere **OWA**): Når du skriver en e-postmelding, klikker du bare **Beskytt** i OWA. Dette vil gjelde "Ikke videresend" tillatelse. Klikk **Endre tillatelse,** og velg **Krypter** for å bare kryptere meldingen.

- Hvis du bruker **Outlook-klient:** Hvis du vil sende en kryptert melding fra Outlook 2013 eller 2016 eller Outlook 2016 for Mac, velger du > **Alternativer-tillatelser**, og deretter velger du beskyttelsesalternativet du trenger. **Options**

- Hvis du vil **kryptere all e-post** som sendes til bestemte mottakere eller eksterne partnerorganisasjoner, må du opprette en regel for transport av e-postflyt i administrasjonssenteret for Exchange. Detaljerte instruksjoner er gitt i [denne støtteartikkelen](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

