---
title: Oppbevaringspolicyer Exchange administrasjonssenteret fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074941"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Oppbevaringspolicyer Exchange administrasjonssenteret

Hvis du vil at vi skal kjøre automatiserte kontroller for innstillingene som er nevnt nedenfor, velger du Tilbake-knappen <- øverst på denne siden, og deretter skriver du inn e-postadressen til brukeren som har problemer med oppbevaringspolicyer.

Hvis du har problemer med oppbevaringspolicyer i Exchange administrasjonssenteret som ikke gjelder for postbokser eller elementer som ikke flyttes til arkivpostboksen, kontrollerer du følgende:

**Grunnårsaker:**

- **Assistent for administrert** mappe har ikke behandlet brukerens postboks. Assistenten for administrert mappe prøver å behandle hver postboks i den skybaserte organisasjonen én gang hver sjuende dag.

  **Løsning:** Kjør assistenten for administrert mappe.

- **Oppbevaringshold** er **aktivert** på postboksen. Hvis postboksen er plassert på en Oppbevaringshold, behandles ikke oppbevaringspolicyen for postboksen i løpet av denne tiden.

  **Løsning:** Kontroller statusen for oppbevaringssperreinnstillingen, og oppdater etter behov. Hvis du vil ha mer informasjon, [kan du se Oppbevaringssperre for postboks](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**Obs!** Hvis en postboks er mindre enn 10 MB, behandler ikke assistenten for administrert mappe postboksen automatisk.
 
Hvis du vil ha mer informasjon om oppbevaringspolicyer i Exchange administrasjonssenteret, kan du se:

- [Oppbevaringskoder og oppbevaringspolicyer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Bruke en oppbevaringspolicy på postbokser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) eller [Legge til eller fjerne oppbevaringskoder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Slik identifiserer du typen sperring som er plassert i en postboks](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
