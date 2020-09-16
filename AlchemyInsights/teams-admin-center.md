---
title: Administrasjonssenter for Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670373"
---
# <a name="teams-admin-center"></a>Administrasjonssenter for Teams

Finn ut om administrasjon av Teams med [administrasjonssenteret for Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Hvis du ikke får tilgang til administrasjonssenteret for Teams, må du kontrollere følgende elementer:

- Kontroller at du har tillatt de riktige [Office 365-IP-adressene og nettadressene](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på eventuelle perimeterenheter (brannmurer osv.) eller i brannmurreglene på den lokale datamaskinen.
- Kontroller at påloggingen du bruker for å få tilgang til administrasjonsportalen for Teams, samsvarer med brukernavnet som er oppført i [administrasjonsportalen for Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Hvis brukerne ikke vises i administrasjonssenteret for Teams, må du kontrollere følgende:

- Har du opprettet brukere eller tilordnet lisenser de siste 24 timene? Kontroller at du venter minst 24 timer før du åpner en støtteforespørsel.
- Kontroller at du har tildelt riktige lisenser?
- Hvis du har en lokal Active Directory, må du kontrollere at [verdien til msRTCSIP-PrimaryUserAddress eller SIP-adressen i proxyAddresses-feltet i den lokale Active Directory er unik, og formatet Sams varer](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) med SIP:**bruker navnet** til brukeren fra [administrasjons senteret for Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Hvis du har tenkt å holde en distribusjon av Skype for Business Server og la brukere være hjemme og tilkoblet: Følg denne Fremgangs muligheten **med å konfigurere hybrid med team og Skype for business online** i Skype for Business Server Control Panel og flytte brukere på nettet.
