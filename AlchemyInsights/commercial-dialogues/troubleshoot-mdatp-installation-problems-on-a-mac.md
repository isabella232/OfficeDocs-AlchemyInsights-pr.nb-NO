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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091058"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Feilsøke problemer med MDATP-installasjon på en Mac

Hvis manuell installasjon mislykkes, viser **Sammendrag-siden** i installasjonsveiviseren følgende feil:

Det oppstod en feil under installasjonen. Installasjonsprogrammet oppdaget en feil som førte til at installasjonen mislyktes. Kontakt programvareprodusenten for å få hjelp.»

For MDM-distribusjoner viser siden også en generell installasjonsfeil.

Selv om vi ikke viser nøyaktige feil til sluttbrukere, beholder vi en loggfil med installasjonsfremdrift i **/Library/Logs/Microsoft/mdatp/install.log**. Hver installasjonsøkt føyer til denne loggfilen. Hvis du bare vil sende ut den siste installasjonsøkten, bruker du `sed` .

Hvis du vil ha mer informasjon, kan du se Feilsøke [installasjonsproblemer for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
