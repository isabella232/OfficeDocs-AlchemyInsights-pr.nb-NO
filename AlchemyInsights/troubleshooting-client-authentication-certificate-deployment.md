---
title: Feilsøke distribusjon av klient godkjennings sertifikat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658995"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Feilsøke distribusjon av klient godkjennings sertifikat

Intune NDES/SCEP-og PKCS/PFX-klient sertifikat profiler brukes ofte sammen med andre profil typer, for eksempel WiFi, VPN og e-post, slik at brukere kan godkjenne til firma ressurser. Når disse profil typene er koblet til en klient sertifikat profil, er avhengig av vellykket distribusjon av profilen.

Innledende infrastruktur konfigurasjon og tilknyttet konfigurasjon av klient sertifikat profilen krever ofte feil søking. Hvis du vil ha en trinnvis veiledning for vellykket konfigurasjon av NDES Connector og veiledning for feil søking for å isolere problemer med sertifikat distribusjon, kan du se: 

- [Konfigurere infrastrukturen til å støtte SCEP med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Oversikt over feil søking av SCEP-sertifikat profiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Bruk de refererte PowerShell-skriptene for å bekrefte konfigurasjonen. Hvis du vil ha mer informasjon, kan du se [verifiserings skript for Intune Certificate Connector](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Andre vanlige problemer**

**Når jeg prøver å installere Intune Certificate Connector på NDES Connector-serveren, får jeg meldingen «passordet i sertifikat forespørselen kan ikke bekreftes. Den kan allerede ha blitt brukt. Få et nytt passord for å sende med denne forespørselen.**  

Denne meldingen betyr at du må kjøre Certificate Connector-installasjonen som administrator.

I enkelte miljøer må serverne der Intune-sertifikatet kjører, bruke en proxy-server til å koble seg til Intune, og derfor må sertifikat koblingen bruke en proxy. I enkelte tilfeller ignorerer NDES Connector de konfigurerte proxy-innstillingene, og det kan være nødvendig å konfigurere proxy-innstillingene mens du kjører i sikkerhets omgivelsene til LocalSystem. 
 
Løsningen er å kjøre Internet Explorer som SYSTEM og konfigurere en proxy i IE. Når tjenesten Intune Connector er startet på nytt, kobles NDES Connector til Intune.

**Bruker enheter mottar ikke lenger SCEP-sertifikater fra NDES.**

Det er mulig at klient godkjennings sertifikatet som er utstedt til NDES server, og som ble angitt under installasjonen av NDES Connector, er utløpt eller mangler. Slik løser du: 
 
1. Avinstaller NDES Connector.  
2. Bruk disse detaljene til å be om et nytt klient godkjenning eller sertifikat for servergodkjenning: 
 
    - Emnenavn: CN = eksternt FQDN  
    - Alternativt navn for emne (begge er nødvendige): DNS = eksternt FQDN, DNS = intern FQDN 
 
3. Installer NDES Connector med det nye sertifikatet.