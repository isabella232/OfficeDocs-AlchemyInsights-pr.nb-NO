---
title: Intune Exchange on-lokal kobling
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808147"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange on-lokal kobling

Hvis du vil ha informasjon om hvordan du konfigurerer koblingen mellom Intune og Exchange som er vert for lokalt, kan du se følgende dokumentasjon:

[Konfigurere Intune on-Premises Exchange Connector i Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**VANLIGE spørsmål**

Sp.: Jeg ser en feil, for eksempel «Exchange Connector-versjonen støttes ikke» når du prøver å konfigurere Exchange Connector. Hva kan være årsaken?

A: kontoen du bruker, er lisensiert riktig – den må ha en aktiv Intune-lisens

Sp.: er det mulig å ha flere Exchange-koblinger?

A: du kan bare konfigurere én Exchange Connector per Intune-leier per Exchange-organisasjon. Koblingen kan bare installeres på én server i en Exchange-organisasjon med flere servere.

Du kan heller ikke konfigurere koblinger for både Exchange lokal pålogging og Exchange Online konfigurert i samme Tenant.

Spørsmål: kan koblingen bruke en CAS-matrise som tilkobling til Exchange?

A: angivelse av en CAS-matrise er ikke en støttet konfigurasjon i koblings oppsettet. Bare én server må være angitt og bør være hardkodet i koblings konfigurasjons filen som du finner i

program data\microsoft\microsoft Intune på den lokale Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Finn følgende oppføring ```<ExchangeWebServiceURL />``` , og erstatt URL-adressen med Exchange-serveren.

**Eksempel**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Hvis du vil ha mer informasjon, kan du se følgende dokumentasjon for ytterligere feil søking: [Feilsøke Intune on-Premises Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivere utførlig logging for Exchange Connector**

1. Åpne konfigurasjons filen for sporing av Exchange Connector for redigering.  
Filen er plassert på:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Eksempel**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Finn TraceSourceLine med følgende nøkkel: OnPremisesExchangeConnectorService  
  
3. Endre verdien for SourceLevel-noden fra Information ActivityTracing (standard) til detaljert ActivityTracing  

**Eksempel**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Start Microsoft Intune Exchange-tjenesten på nytt  
5. Full synkronisering i Intune-portalen til den er ferdig og deretter endrer XML tilbake til «informasjon ActivityTracing» og starter Microsoft Intune Exchange-tjenesten på nytt.  
6. Plasseringen av loggene er: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`