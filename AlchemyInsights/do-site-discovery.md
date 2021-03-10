---
title: Gjøre nettstedsoppdaging
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694563"
---
# <a name="do-site-discovery"></a>Gjøre nettstedsoppdaging

Hvis organisasjonen fremdeles bruker eldre nettprogrammer og planer til å bruke Internet Explorer-modus (som de fleste kunder gjør), bør du gjøre noe ekstra nettstedsoppdaging.

**Du har allerede distribuert en eldre versjon av Microsoft Edge**

Hvis du allerede har konfigurert listen over virksomhetsnettsteder til å fungere for den eldre versjonen av Microsoft Edge, er nettstedssøk nesten ferdig. Det du kanskje må gjøre, er å legge til nøytrale nettsteder.

Nøytrale nettsteder er vanligvis nettsteder som gir enkel pålogging (SSO). Hvis du går til et nøytralt nettsted fra Microsoft Edge, ønsker du å bli i Microsoft Edge for å godkjenne. Hvis du går til et nøytralt nettsted i Internet Explorer-modus, må du være i Internet Explorer-modus for å godkjenne.

Identifiser eventuelle SSO-er eller andre nøytrale nettsteder du bruker, og legg dem til i listen over virksomhetsnettsteder.

**Internet Explorer er standardleseren din**

Hvis du bare bruker Internet Explorer nå, vet du kanskje ikke hvilke nettsteder som har oppgradert til moderne nettstandarder, og som fremdeles krever Internet Explorer. Du kan finne og legge til disse nettstedene i listen over virksomhetsnettsteder, slik at du bare kan bruke Internet Explorer-modus for disse nettstedene.

> [!NOTE]
> [Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) oppdager nettsteder som kanskje trenger Internet Explorer-modus. Den kan samle inn data på datamaskiner som kjører Windows Internet Explorer 8 via Internet Explorer 11 på Windows 10, Windows 8.1 eller Windows 7.

**Analysere dataene**

Når du har samlet inn nettstedsdata, anbefaler vi følgende firetrinns prosess for å analysere dataene:
1. Sorter dataene etter domene, og deretter etter URL-adresse.
2. Definer grensene for en app for å konfigurere for Internet Explorer-modus. Du vil inkludere alle nettstedene og nettkontrollene som definerer appen, men du vil ikke inkludere ekstra nettsteder og kontroller. Noen nettsteder kan være så enkle som, mens andre kan kreve at du *https://contoso.com/app1* definerer flere nettsteder og sider.
3. Test appen for å bekrefte at den ikke fungerer opprinnelig. Mange nettsteder tilbyr moderne innhold når de oppdager en moderne nettleser og bare tilbyr eldre innhold når de oppdager Internet Explorer.
4. Legg til appen i listen over virksomhetsnettsteder hvis den ikke tester.

> [!NOTE]
> Den beste praksisen er å gruppere alle nettstedene som utgjør en app. Når du oppgraderer en app, er det på denne måten enklere å fjerne hele nettstedet fra Internet Explorer-modus og begynne å bruke en moderne nettleser for appen.

Når du er ferdig med nettstedsoppdagingen og du har analysert dataene, er du klar til å begynne å se på kanalstrategien.

