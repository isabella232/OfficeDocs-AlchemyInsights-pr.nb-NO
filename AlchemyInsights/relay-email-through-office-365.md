---
title: Videresende e-postmeldinger via Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117992"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Konfigurere en enhet eller et program med flere funksjoner til å sende e-post

Hvis du vil vite mer om alternativene og trinnene, kan du se [Slik konfigurerer du en enhet eller et program med flere funksjoner til å sende e-post ved hjelp av Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Hvis du har en enhet eller et program som nylig sluttet å fungere, er de vanligste problemene:

- **Godkjenningsrelaterte feil under bruk av SMTP Auth-klientinnsending** Vi har nylig gjort noen endringer relatert til hvordan SMTP-godkjenning fungerer. Hvis du vil ha mer informasjon om hvordan du løser problemer, kan du se delen Om godkjenning mislyktes i Løse problemer med [skrivere, skannere](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)og LOB-programmer som sender e-post ved hjelp av Microsoft 365 eller Office 365 .
- **Vi godtar bare TLS 1.2-versjonen mens du gjør en sikker tilkobling til Office 365** Hvis du bruker Sikker tilkobling (TLS), må du kontrollere at programenheten støtter TLS 1.2. Hvis du vil ha mer informasjon, kan du se [Klargjøre for TLS 1.2 i Office 365 og Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Hvis du vil ha andre problemer og løsninger, kan du se Løse problemer med skrivere, skannere og [LOB-programmer](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)som sender e-post ved hjelp av Microsoft 365 eller Office 365 .

Hvis du vil se de berørte enhetene, kan du gå til [rapporten SMTP AUTH-klienter](https://protection.office.com/mailflow/dashboard).

**Obs!** Exchange Online ikke tar hensyn til scenarioer for masseutsendelse. Hvis du vil sende masseutsendelse av kommersiell e-post (for eksempel kundenyhetsbrev), bør du bruke tredjepartsleverandører som er spesialister på disse tjenestene.
