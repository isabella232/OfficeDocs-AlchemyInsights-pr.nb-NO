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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010733"
---
# <a name="encrypt-email-messages-in-outlook"></a>Kryptere e-postmeldinger i Outlook

Microsoft 365 Meldingskryptering er Microsoft Azure Rights Management (Azure RMS), som er en del av Azure Information Protection. Hvis abonnementet omfatter Azure Rights Management eller Azure Information **Protection,** trenger du ikke å utføre noen handlinger for å aktivere eller aktivere Rights Management Service manuelt.

Basert på tilbakemeldinger fra kunder, vil vi ikke lenger aktivere Exchange regler for e-postflyt for å kryptere utgående e-post som inneholder bestemt type sensitiv informasjon i leieren som standard. I stedet gir vi detaljerte instruksjoner om hvordan du kan gjøre dette selv. Hvis du vil ha mer informasjon om hvordan du oppretter en transportregel for å kryptere sensitiv informasjon, kan du se [denne artikkelen](https://aka.ms/OmeEtr).

- Hvis du Outlook på nettet (tidligere **OWA):** Når du skriver en e-postmelding, klikker du bare **Beskytt** i OWA. Dette gjelder tillatelsen Ikke videresend. Klikk **Endre tillatelse,** og velg **Krypter** for bare å kryptere meldingen.

- Hvis du **bruker Outlook-klient:** Hvis du vil sende en kryptert melding fra Outlook 2013 eller 2016, eller Outlook 2016 for Mac, velger du Alternativertillatelser og deretter  >  beskyttelsesalternativet du trenger.

- Hvis **du vil kryptere all e-post** som sendes automatisk til bestemte mottakere eller eksterne partnerorganisasjoner, må du opprette en transportregel for e-postflyt i Exchange administrasjonssenteret. Du finner detaljerte instruksjoner i [denne støtteartikkelen](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

