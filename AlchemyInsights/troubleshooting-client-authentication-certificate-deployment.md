---
title: Feilsøke distribusjon av klientgodkjenningssertifikat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555304"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Feilsøke distribusjon av klientgodkjenningssertifikat

Intune NDES/SCEP- og PKCS/PFX Client-sertifikatprofiler brukes ofte sammen med andre profiler som Wifi, VPN og e-post for å tillate brukere å godkjenne til bedriftsressurser. Når disse profiltypene er koblet til en klientsertifikatprofil, avhenger av vellykket distribusjon av denne profilen.

Første infrastrukturoppsett og tilknyttet konfigurasjon av klientsertifikatprofilen krever ofte feilsøking. Hvis du vil ha en trinnvis veiledning for vellykket oppsett av NDES-koblingen og feilsøkingsveiledningen for å isolere problemer med sertifikatdistribusjon, kan du se: 

- [Konfigurere infrastruktur for å støtte SCEP med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Oversikt for feilsøking av SCEP-sertifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Bruk de refererte powershell-skriptene til å bekrefte konfigurasjonen. Hvis du vil ha mer informasjon, kan du se [Skript for bekreftelse av Intune Sertifikat-kobling](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Andre vanlige problemer**

**Når jeg prøver å installere Intune sertifikatkoblingen på NDES connector-serveren, får jeg meldingen "Passordet i sertifikatforespørselen kan ikke bekreftes. Det kan ha blitt brukt allerede. Få et nytt passord å sende inn med denne forespørselen."**  

Denne meldingen betyr at du må kjøre installasjonen av sertifikatkoblingen som administrator.

I noen miljøer må serverne der Intune-sertifikatet kjører, bruke en proxy-server til å koble til Intune, og derfor må sertifikatkoblingen bruke en proxy. I noen tilfeller ignorerer NDES Connector de konfigurerte proxy-innstillingene, og det kan være nødvendig å konfigurere proxy-innstillingene mens du kjører i sikkerhetskonteksten for LocalSystem. 
 
Løsningen er å kjøre Internet Explorer som SYSTEM og konfigurere en proxy i IE. Etter en omstart av Intune Connector Service, kobler NDES-kontakten til Intune.

**Brukerenheter mottar ikke lenger SCEP-sertifikater fra NDES.**

Det er mulig at klientgodkjenningssertifikatet som er utstedt til NDES-serveren, og angitt under installasjonen av NDES-koblingen, er utløpt eller mangler. Slik løser du: 
 
1. Avinstaller NDES-kontakten.  
2. Bruk disse detaljene til å be om en ny klientgodkjenning eller servergodkjenningssertifikat: 
 
    - Emnenavn: CN=external fqdn  
    - Emne alternativ navn (begge er nødvendig): DNS = ekstern fqdn, DNS = intern fqdn 
 
3. Installer NDES-koblingen på nytt med det nye sertifikatet.