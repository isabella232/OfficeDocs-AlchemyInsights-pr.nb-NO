---
title: Intune Exchange lokale kobling
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013973"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange lokale kobling

Hvis du vil ha mer informasjon om hvordan du konfigurerer koblingen mellom Intune og Exchange som driftes lokalt, kan du se følgende dokumentasjon:

[Konfigurere den lokale Intune-Exchange i Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Vanlige spørsmål:**

Sp.: Jeg ser en feil, for eksempel «Exchange Connector-versjonen støttes ikke» når jeg prøver å konfigurere Exchange koblingen. Hva kan være årsaken?

Svar: Kontoen du bruker, er lisensiert på riktig måte – den må ha en aktiv Intune-lisens

Spørsmål: Er det mulig å ha flere Exchange koblinger?

A: Du kan bare konfigurere én Exchange kobling per Intune-leier per Exchange organisasjon. Koblingen kan bare installeres på én server i en organisasjon med flere servere.

Du kan heller ikke ha koblinger konfigurert for både Exchange lokale og Exchange Online konfigurert i samme tenant.

Spørsmål: Kan koblingen bruke en CAS-matrise som tilkobling til Exchange?

A: Angivelse av en CAS-matrise er ikke en støttet konfigurasjon i koblingsoppsettet. Bare én enkelt server bør angis og skal være hardkodet i konfigurasjonsfilen for koblinger som du finner i

program data\microsoft\microsoft Intune on premiss Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Finn følgende oppføring, ```<ExchangeWebServiceURL />``` og erstatt nettadressen med Exchange-serveren.

**Eksempel:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Se følgende dokumentasjon for ytterligere feilsøking: Feilsøke [den lokale Intune-Exchange-koblingen](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Aktivere detaljert logging for Exchange-koblingen**

1. Åpne konfigurasjonsfilen Exchange koblingssporing for redigering.  
Filen er plassert på : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Eksempel:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Finn TraceSourceLine med følgende nøkkel: OnPremisesExchangeConnectorService  
  
3. Endre SourceLevel-nodeverdien fra Information ActivityTracing (standard) til Detaljert ActivityTracing  

**Eksempel:**
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
4. Start Microsoft Intune Exchange tjenesten på nytt  
5. Full synkronisering i Intune Portal til den er ferdig, og endre deretter XML-filen tilbake til «Information ActivityTracing», og start Microsoft Intune Exchange tjenesten.  
6. Plasseringen av loggene er: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`