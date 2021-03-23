---
title: Beskyttelse mot backscatter-angrep
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036077"
---
# <a name="protection-from-backscatter-attack"></a>Beskyttelse mot backscatter-angrep

Backscatter er rapporter om manglende levering (også kalt NDR-er eller returmeldinger) du mottar for meldinger du ikke har sendt. Søppelpostsendere forfalsket **Fra-adressen** til meldingene sine, og de bruker ofte ekte e-postadresser til å gi troverdighet til meldingene sine. Så når søppelpostsendere uunngåelig sender meldinger til ikke-eksisterende mottakere, blir mål-e-postserveren i hovedsak lurt til å returnere meldingen som ikke kan leveres, i en NDR til den forfalskede avsenderen i **Fra:-adressen.**

Du finner mer informasjon i [Backscatter i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Aktivere backscatter-beskyttelse**

Hvis du vil aktivere Backscatter-beskyttelse, følger du banen nedenfor.

**protection.office.com > Policy > Policy > Antispam > Velg policyen for søppelpostfilter og Rediger policy > Egenskaper for søppelpost > Merk som søppelpost > NDR-tilbakevindu > Angi den til På**

Hvis du mener at en konto er kompromittert, kan du se følgende:

- [Svare på en kompromittert e-postkonto](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Fjerne blokkerte brukere fra portalen begrensede brukere i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



