---
title: Administrasjonssenter for Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826388"
---
# <a name="teams-admin-center"></a>Administrasjonssenter for Teams

Finn ut om administrasjon av Teams med [administrasjonssenteret for Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Hvis du ikke får tilgang til administrasjonssenteret for Teams, må du kontrollere følgende elementer:

- Kontroller at du har tillatt de riktige [Office 365-IP-adressene og nettadressene](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på eventuelle perimeterenheter (brannmurer osv.) eller i brannmurreglene på den lokale datamaskinen.
- Kontroller at påloggingen du bruker for å få tilgang til administrasjonsportalen for Teams, samsvarer med brukernavnet som er oppført i [administrasjonsportalen for Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Hvis brukerne ikke vises i administrasjonssenteret for Teams, må du kontrollere følgende:

- Har du opprettet brukere eller tilordnet lisenser de siste 24 timene? Kontroller at du venter minst 24 timer før du åpner en støtteforespørsel.
- Kontroller at du har tildelt riktige lisenser?
- Hvis du har en lokal Active Directory, må du kontrollere at verdien av [msRTCSIP-PrimaryUserAddress eller SIP-adressen i ProxyAddresses-feltet](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) i den lokale Active Directory er unik, og at formatet samsvarer med sip:**Brukernavnet** til brukeren fra administrasjonssenteret [for Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Hvis du har tenkt å beholde en Skype for Business Server-distribusjon og få brukerne til å være hjemmebruk lokalt og på Nettet: følg «Konfigurer hybrid med Teams og **Skype for Business Online»** i kontrollpanelet for Skype for Business Server og flytt brukere på Nettet.
