---
title: Administrasjonssenter for Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354097"
---
# <a name="teams-admin-center"></a>Administrasjonssenter for Teams

Finn ut om administrasjon av Teams med [administrasjonssenteret for Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Hvis du ikke får tilgang til administrasjonssenteret for Teams, må du kontrollere følgende elementer:

- Kontroller at du har tillatt de riktige [Office 365-IP-adressene og nettadressene](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) på eventuelle perimeterenheter (brannmurer osv.) eller i brannmurreglene på den lokale datamaskinen.
- Kontroller at påloggingen du bruker for å få tilgang til administrasjonsportalen for Teams, samsvarer med brukernavnet som er oppført i [administrasjonsportalen for Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Hvis brukerne ikke vises i administrasjonssenteret for Teams, må du kontrollere følgende:

- Har du opprettet brukere eller tilordnet lisenser de siste 24 timene? Kontroller at du venter minst 24 timer før du åpner en støtteforespørsel.
- Kontroller at du har tildelt riktige lisenser?
- Hvis du har en lokal Active Directory, må du kontrollere at [verdien for msRTCSIP-PrimaryUserAddress eller SIP-adressen i Feltet ProxyAddresses i den lokale Active Directory er unik, og formatet samsvarer med](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip: Brukernavn**for** brukeren fra [administrasjonssenteret for Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Hvis du har tenkt å beholde en Skype for Business Server-distribusjon og få brukere hjemmehjemme og tilkoblet: følg **"Konfigurer hybrid med Teams og Skype for Business Online"** i Kontrollpanelet for Skype for Business Server og flytt brukere på nettet.
