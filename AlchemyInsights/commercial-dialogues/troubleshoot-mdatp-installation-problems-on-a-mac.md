---
title: Feilsøke problemer med MDATP-installasjon på en Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749774"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Feilsøke problemer med MDATP-installasjon på en Mac

Hvis manuell installasjon mislykkes, viser **Sammendrag-siden** i installasjonsveiviseren følgende feil:

Det oppstod en feil under installasjonen. Installasjonsprogrammet oppdaget en feil som førte til at installasjonen mislyktes. Kontakt programvareprodusenten for å få hjelp.»

For MDM-distribusjoner viser siden også en generell installasjonsfeil.

Selv om vi ikke viser nøyaktige feil til sluttbrukere, beholder vi en loggfil med installasjonsfremdrift i **/Library/Logs/Microsoft/mdatp/install.log**. Hver installasjonsøkt føyer til denne loggfilen. Hvis du bare vil sende ut den siste installasjonsøkten, bruker du `sed` .

Hvis du vil ha mer informasjon, kan du se Feilsøke [installasjonsproblemer for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
