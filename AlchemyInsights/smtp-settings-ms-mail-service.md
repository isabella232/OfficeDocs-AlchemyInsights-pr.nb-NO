---
title: SMTP-innstillinger for Microsoft 365 e-posttjenesten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 373042e9593faf4eaa486313763beb8e8f48b6e9ea159d1cfb37b9df826384f4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813977"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>SMTP-innstillinger for Microsoft 365 e-posttjenesten

Dette er SMTP-innstillingene for de Microsoft 365 e-posttjenestene:

**Server:** smtp.office365.com </br>
**Port**: 587 </br>
**Kryptering:** STARTTLS (bare TLS 1.2-versjon støttes nå. Kontroller at programmet eller enheten støtter TLS 1.2) </br>
**Brukernavn:** Office 365 (for eksempel example@yourdomain.com) </br>
**Passord:** passordet Office 365 passord </br>
**Godkjenning**: Obligatorisk </br>
**Sendegrenser:** 10 000 e-postmeldinger om dagen </br>

Hvis du vil ha informasjon om POP- og IMAP-innstillinger, kan du [se POP-, IMAP- og SMTP-innstillinger](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Hvis du vil lære om alternativene for videresending av e-post ved hjelp av Microsoft 365 og trinnene, kan du se Slik konfigurerer du en enhet eller et program med flere enheter til å sende e-post ved hjelp av Microsoft 365 eller [Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).