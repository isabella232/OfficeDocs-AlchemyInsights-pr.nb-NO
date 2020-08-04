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
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="09d5b-102">Feilsøke distribusjon av klientgodkjenningssertifikat</span><span class="sxs-lookup"><span data-stu-id="09d5b-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="09d5b-103">Intune NDES/SCEP- og PKCS/PFX Client-sertifikatprofiler brukes ofte sammen med andre profiler som Wifi, VPN og e-post for å tillate brukere å godkjenne til bedriftsressurser.</span><span class="sxs-lookup"><span data-stu-id="09d5b-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="09d5b-104">Når disse profiltypene er koblet til en klientsertifikatprofil, avhenger av vellykket distribusjon av denne profilen.</span><span class="sxs-lookup"><span data-stu-id="09d5b-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="09d5b-105">Første infrastrukturoppsett og tilknyttet konfigurasjon av klientsertifikatprofilen krever ofte feilsøking.</span><span class="sxs-lookup"><span data-stu-id="09d5b-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="09d5b-106">Hvis du vil ha en trinnvis veiledning for vellykket oppsett av NDES-koblingen og feilsøkingsveiledningen for å isolere problemer med sertifikatdistribusjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="09d5b-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="09d5b-107">Konfigurere infrastruktur for å støtte SCEP med Intune</span><span class="sxs-lookup"><span data-stu-id="09d5b-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="09d5b-108">Oversikt for feilsøking av SCEP-sertifikatprofiler med Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="09d5b-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="09d5b-109">Bruk de refererte powershell-skriptene til å bekrefte konfigurasjonen.</span><span class="sxs-lookup"><span data-stu-id="09d5b-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="09d5b-110">Hvis du vil ha mer informasjon, kan du se [Skript for bekreftelse av Intune Sertifikat-kobling](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="09d5b-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="09d5b-111">**Andre vanlige problemer**</span><span class="sxs-lookup"><span data-stu-id="09d5b-111">**Other common issues**</span></span>

<span data-ttu-id="09d5b-112">**Når jeg prøver å installere Intune sertifikatkoblingen på NDES connector-serveren, får jeg meldingen "Passordet i sertifikatforespørselen kan ikke bekreftes. Det kan ha blitt brukt allerede. Få et nytt passord å sende inn med denne forespørselen."**</span><span class="sxs-lookup"><span data-stu-id="09d5b-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="09d5b-113">Denne meldingen betyr at du må kjøre installasjonen av sertifikatkoblingen som administrator.</span><span class="sxs-lookup"><span data-stu-id="09d5b-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="09d5b-114">I noen miljøer må serverne der Intune-sertifikatet kjører, bruke en proxy-server til å koble til Intune, og derfor må sertifikatkoblingen bruke en proxy.</span><span class="sxs-lookup"><span data-stu-id="09d5b-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="09d5b-115">I noen tilfeller ignorerer NDES Connector de konfigurerte proxy-innstillingene, og det kan være nødvendig å konfigurere proxy-innstillingene mens du kjører i sikkerhetskonteksten for LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="09d5b-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="09d5b-116">Løsningen er å kjøre Internet Explorer som SYSTEM og konfigurere en proxy i IE.</span><span class="sxs-lookup"><span data-stu-id="09d5b-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="09d5b-117">Etter en omstart av Intune Connector Service, kobler NDES-kontakten til Intune.</span><span class="sxs-lookup"><span data-stu-id="09d5b-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="09d5b-118">**Brukerenheter mottar ikke lenger SCEP-sertifikater fra NDES.**</span><span class="sxs-lookup"><span data-stu-id="09d5b-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="09d5b-119">Det er mulig at klientgodkjenningssertifikatet som er utstedt til NDES-serveren, og angitt under installasjonen av NDES-koblingen, er utløpt eller mangler.</span><span class="sxs-lookup"><span data-stu-id="09d5b-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="09d5b-120">Slik løser du:</span><span class="sxs-lookup"><span data-stu-id="09d5b-120">To resolve:</span></span> 
 
1. <span data-ttu-id="09d5b-121">Avinstaller NDES-kontakten.</span><span class="sxs-lookup"><span data-stu-id="09d5b-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="09d5b-122">Bruk disse detaljene til å be om en ny klientgodkjenning eller servergodkjenningssertifikat:</span><span class="sxs-lookup"><span data-stu-id="09d5b-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="09d5b-123">Emnenavn: CN=external fqdn</span><span class="sxs-lookup"><span data-stu-id="09d5b-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="09d5b-124">Emne alternativ navn (begge er nødvendig): DNS = ekstern fqdn, DNS = intern fqdn</span><span class="sxs-lookup"><span data-stu-id="09d5b-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="09d5b-125">Installer NDES-koblingen på nytt med det nye sertifikatet.</span><span class="sxs-lookup"><span data-stu-id="09d5b-125">Reinstall the NDES connector with the new certificate.</span></span>