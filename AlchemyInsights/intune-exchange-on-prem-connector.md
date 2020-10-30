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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="94086-102">Intune Exchange on-lokal kobling</span><span class="sxs-lookup"><span data-stu-id="94086-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="94086-103">Hvis du vil ha informasjon om hvordan du konfigurerer koblingen mellom Intune og Exchange som er vert for lokalt, kan du se følgende dokumentasjon:</span><span class="sxs-lookup"><span data-stu-id="94086-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="94086-104">Konfigurere Intune on-Premises Exchange Connector i Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="94086-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="94086-105">**VANLIGE spørsmål**</span><span class="sxs-lookup"><span data-stu-id="94086-105">**FAQ:**</span></span>

<span data-ttu-id="94086-106">Sp.: Jeg ser en feil, for eksempel «Exchange Connector-versjonen støttes ikke» når du prøver å konfigurere Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="94086-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="94086-107">Hva kan være årsaken?</span><span class="sxs-lookup"><span data-stu-id="94086-107">What could be the cause?</span></span>

<span data-ttu-id="94086-108">A: kontoen du bruker, er lisensiert riktig – den må ha en aktiv Intune-lisens</span><span class="sxs-lookup"><span data-stu-id="94086-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="94086-109">Sp.: er det mulig å ha flere Exchange-koblinger?</span><span class="sxs-lookup"><span data-stu-id="94086-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="94086-110">A: du kan bare konfigurere én Exchange Connector per Intune-leier per Exchange-organisasjon.</span><span class="sxs-lookup"><span data-stu-id="94086-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="94086-111">Koblingen kan bare installeres på én server i en Exchange-organisasjon med flere servere.</span><span class="sxs-lookup"><span data-stu-id="94086-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="94086-112">Du kan heller ikke konfigurere koblinger for både Exchange lokal pålogging og Exchange Online konfigurert i samme Tenant.</span><span class="sxs-lookup"><span data-stu-id="94086-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="94086-113">Spørsmål: kan koblingen bruke en CAS-matrise som tilkobling til Exchange?</span><span class="sxs-lookup"><span data-stu-id="94086-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="94086-114">A: angivelse av en CAS-matrise er ikke en støttet konfigurasjon i koblings oppsettet.</span><span class="sxs-lookup"><span data-stu-id="94086-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="94086-115">Bare én server må være angitt og bør være hardkodet i koblings konfigurasjons filen som du finner i</span><span class="sxs-lookup"><span data-stu-id="94086-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="94086-116">program data\microsoft\microsoft Intune på den lokale Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="94086-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="94086-117">Finn følgende oppføring ```<ExchangeWebServiceURL />``` , og erstatt URL-adressen med Exchange-serveren.</span><span class="sxs-lookup"><span data-stu-id="94086-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="94086-118">**Eksempel**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="94086-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="94086-119">Hvis du vil ha mer informasjon, kan du se følgende dokumentasjon for ytterligere feil søking: [Feilsøke Intune on-Premises Exchange Connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="94086-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="94086-120">**Aktivere utførlig logging for Exchange Connector**</span><span class="sxs-lookup"><span data-stu-id="94086-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="94086-121">Åpne konfigurasjons filen for sporing av Exchange Connector for redigering.</span><span class="sxs-lookup"><span data-stu-id="94086-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="94086-122">Filen er plassert på:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="94086-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="94086-123">**Eksempel**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="94086-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="94086-124">Finn TraceSourceLine med følgende nøkkel: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="94086-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="94086-125">Endre verdien for SourceLevel-noden fra Information ActivityTracing (standard) til detaljert ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="94086-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="94086-126">**Eksempel**</span><span class="sxs-lookup"><span data-stu-id="94086-126">**Example:**</span></span>
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
4. <span data-ttu-id="94086-127">Start Microsoft Intune Exchange-tjenesten på nytt</span><span class="sxs-lookup"><span data-stu-id="94086-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="94086-128">Full synkronisering i Intune-portalen til den er ferdig og deretter endrer XML tilbake til «informasjon ActivityTracing» og starter Microsoft Intune Exchange-tjenesten på nytt.</span><span class="sxs-lookup"><span data-stu-id="94086-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="94086-129">Plasseringen av loggene er: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="94086-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>