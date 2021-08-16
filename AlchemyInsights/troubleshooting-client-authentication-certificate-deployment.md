---
title: Feilsøke klientgodkjenningssertifikatdistribusjon
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020813"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Feilsøke klientgodkjenningssertifikatdistribusjon

Sertifikatprofiler for Intune NDES/SCEP og PKCS/PFX-klient brukes vanligvis sammen med andre profiltyper, for eksempel Wifi, VPN og e-post, slik at brukere kan godkjenne til bedriftens ressurser. Når disse profiltypene er koblet til en klientsertifikatprofil, avhenger den vellykkede distribusjonen av denne profilen.

Første infrastrukturoppsett og tilknyttet konfigurasjon av klientsertifikatprofilen krever ofte feilsøking. Hvis du vil ha en trinnvis veiledning for vellykket konfigurasjon av NDES-koblingen og feilsøkingsveiledning for å isolere problemer med sertifikatdistribusjon, kan du se: 

- [Konfigurere infrastruktur for å støtte SCEP med Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Oversikt for feilsøking av SCEP-sertifikatprofiler med Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Bruk de refererte powershell-skriptene til å bekrefte konfigurasjonen. Hvis du vil ha mer informasjon, kan du se [Bekreftelsesskript for Intune Certificate-kobling](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Andre vanlige problemer**

**Når jeg prøver å installere Intune-sertifikatkoblingen på NDES-koblingsserveren, får jeg meldingen «Passordet i sertifikatforespørselen kan ikke bekreftes. Den kan allerede ha blitt brukt. Få et nytt passord for å sende inn med denne forespørselen.»**  

Denne meldingen betyr at du må kjøre installasjonen av sertifikatkoblingen som administrator.

I enkelte miljøer må serverne der Intune-sertifikatet kjører, bruke en proxy-server til å koble til Intune, og derfor må sertifikatkoblingen bruke en proxy. I noen tilfeller ignorerer NDES Connector de konfigurerte proxy-innstillingene, og det kan være nødvendig å konfigurere proxy-innstillingene mens du kjører i sikkerhetskonteksten for LocalSystem. 
 
Løsningen er å kjøre Internet Explorer som SYSTEM og konfigurere en proxy i IE. Etter en omstart av Intune Connector-tjenesten kobles NDES-koblingen til Intune.

**Brukerenheter mottar ikke lenger SCEP-sertifikater fra NDES.**

Det er mulig at klientgodkjenningssertifikatet utstedt til NDES-serveren, og angitt under installasjonen av NDES-koblingen, har utløpt eller mangler. Slik løser du dette: 
 
1. Avinstaller NDES-koblingen.  
2. Bruk disse detaljene til å be om et nytt klientgodkjennings- eller servergodkjenningssertifikat: 
 
    - Emnenavn: CN=ekstern fqdn  
    - Alternativt emnenavn (begge er obligatorisk): DNS=ekstern fqdn, DNS=intern fqdn 
 
3. Installer NDES-koblingen på nytt med det nye sertifikatet.