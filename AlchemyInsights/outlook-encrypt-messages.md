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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511517"
---
# <a name="encrypt-email-messages-in-outlook"></a>Krypter e-postmeldinger i Outlook

Microsoft 365-meldingskryptering er bygget på Microsoft Azure Rights Management (Azure RMS), som er en del av Azure Information Protection. Hvis abonnementet inkluderer Azure Rights Management eller Azure Information Protection, trenger du ikke å utføre handlinger for å aktivere eller aktivere Rights Management-tjenesten **manuelt.**

Basert på tilbakemeldinger fra kunder, vil vi ikke lenger aktivere Exchange-e-postflytregler til automatisk å kryptere utgående e-post som inneholder visse typer sensitiv informasjon i leieren som standard. I stedet gir vi detaljerte instruksjoner om hvordan dere kan gjøre det selv. Hvis du vil ha mer informasjon om hvordan du oppretter en transportregel for å kryptere sensitiv informasjon, kan du se [denne artikkelen](https://aka.ms/OmeEtr).

- Hvis du bruker Outlook på nettet (tidligere **OWA**): Når du skriver en e-postmelding, klikker du bare **Beskytt** i OWA. Dette vil bruke "Ikke videresend" -tillatelse. Klikk **Endre tillatelse,** og velg **Krypter** for å bare kryptere meldingen.

- Hvis du bruker **Outlook-klient**: Hvis du vil sende en kryptert melding fra Outlook 2013 eller 2016 eller Outlook 2016 for Mac, velger du **Alternativer**  >  tillatelser , og deretter velger du**beskyttelsesalternativet**du trenger.

- Hvis du **vil kryptere all e-post** som sendes til bestemte mottakere eller eksterne partnerorganisasjoner automatisk, må du opprette en transportregel for e-postflyt i administrasjonssenteret for Exchange. Detaljerte instruksjoner er gitt i [denne støtteartikkelen](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

