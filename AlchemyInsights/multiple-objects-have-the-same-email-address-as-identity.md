---
title: Flere objekter har samme e-postadresse som identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439189"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Flere objekter har samme e-postadresse som identitet

**Flere objekter**

En av de vanligste årsakene til denne feilen er ikke å kunne rute en Outlook Web Access-forespørsel riktig i en tilstedeværelse av flere objekter som har samme e-postadresse som identitet. Hvis du vil finne disse objektene, kjører du følgende kommandoer:

· Få-mottaker<email address>

· Få-bruker<email address>

· Få bruker <email address> -SoftDeletedUser

· Få kontakt<email address>

· Get-Postboks <email address> - PublicFolder

· Get-Postboks <email address> -IncludeSoftDeletedMailbox

· Get-Postboks <email address> -InaktivMailboxBare

Hvis du vil løse problemet, kan du fjerne flere objekter med samme e-postidentitet og kontrollere at det er ett enkelt objekt med den bestemte e-postidentiteten, og at mottakertypen er UserMailbox.

**Samme adresse brukes for forretnings- og forbrukerpostbokser**

En annen årsak er når den samme adressen brukes for forretnings- og forbrukerpostbokser. I dette tilfellet må brukeren endre sitt primære forbrukeralias til Cafe støtter dette scenariet. Dette er en permanent feil som ikke går bort uten inngripen.

Hvis du vil ha mer informasjon, kan du se [Endre e-postadressen eller telefonnummeret for Microsoft-kontoen](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).