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
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="754c8-102">Feilsøke distribusjon av klient godkjennings sertifikat</span><span class="sxs-lookup"><span data-stu-id="754c8-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="754c8-103">Intune NDES/SCEP-og PKCS/PFX-klient sertifikat profiler brukes ofte sammen med andre profil typer, for eksempel WiFi, VPN og e-post, slik at brukere kan godkjenne til firma ressurser.</span><span class="sxs-lookup"><span data-stu-id="754c8-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="754c8-104">Når disse profil typene er koblet til en klient sertifikat profil, er avhengig av vellykket distribusjon av profilen.</span><span class="sxs-lookup"><span data-stu-id="754c8-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="754c8-105">Innledende infrastruktur konfigurasjon og tilknyttet konfigurasjon av klient sertifikat profilen krever ofte feil søking.</span><span class="sxs-lookup"><span data-stu-id="754c8-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="754c8-106">Hvis du vil ha en trinnvis veiledning for vellykket konfigurasjon av NDES Connector og veiledning for feil søking for å isolere problemer med sertifikat distribusjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="754c8-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="754c8-107">Konfigurere infrastrukturen til å støtte SCEP med Intune</span><span class="sxs-lookup"><span data-stu-id="754c8-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="754c8-108">Oversikt over feil søking av SCEP-sertifikat profiler med Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="754c8-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="754c8-109">Bruk de refererte PowerShell-skriptene for å bekrefte konfigurasjonen.</span><span class="sxs-lookup"><span data-stu-id="754c8-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="754c8-110">Hvis du vil ha mer informasjon, kan du se [verifiserings skript for Intune Certificate Connector](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="754c8-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="754c8-111">**Andre vanlige problemer**</span><span class="sxs-lookup"><span data-stu-id="754c8-111">**Other common issues**</span></span>

<span data-ttu-id="754c8-112">**Når jeg prøver å installere Intune Certificate Connector på NDES Connector-serveren, får jeg meldingen «passordet i sertifikat forespørselen kan ikke bekreftes. Den kan allerede ha blitt brukt. Få et nytt passord for å sende med denne forespørselen.**</span><span class="sxs-lookup"><span data-stu-id="754c8-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="754c8-113">Denne meldingen betyr at du må kjøre Certificate Connector-installasjonen som administrator.</span><span class="sxs-lookup"><span data-stu-id="754c8-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="754c8-114">I enkelte miljøer må serverne der Intune-sertifikatet kjører, bruke en proxy-server til å koble seg til Intune, og derfor må sertifikat koblingen bruke en proxy.</span><span class="sxs-lookup"><span data-stu-id="754c8-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="754c8-115">I enkelte tilfeller ignorerer NDES Connector de konfigurerte proxy-innstillingene, og det kan være nødvendig å konfigurere proxy-innstillingene mens du kjører i sikkerhets omgivelsene til LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="754c8-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="754c8-116">Løsningen er å kjøre Internet Explorer som SYSTEM og konfigurere en proxy i IE.</span><span class="sxs-lookup"><span data-stu-id="754c8-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="754c8-117">Når tjenesten Intune Connector er startet på nytt, kobles NDES Connector til Intune.</span><span class="sxs-lookup"><span data-stu-id="754c8-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="754c8-118">**Bruker enheter mottar ikke lenger SCEP-sertifikater fra NDES.**</span><span class="sxs-lookup"><span data-stu-id="754c8-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="754c8-119">Det er mulig at klient godkjennings sertifikatet som er utstedt til NDES server, og som ble angitt under installasjonen av NDES Connector, er utløpt eller mangler.</span><span class="sxs-lookup"><span data-stu-id="754c8-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="754c8-120">Slik løser du:</span><span class="sxs-lookup"><span data-stu-id="754c8-120">To resolve:</span></span> 
 
1. <span data-ttu-id="754c8-121">Avinstaller NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="754c8-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="754c8-122">Bruk disse detaljene til å be om et nytt klient godkjenning eller sertifikat for servergodkjenning:</span><span class="sxs-lookup"><span data-stu-id="754c8-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="754c8-123">Emnenavn: CN = eksternt FQDN</span><span class="sxs-lookup"><span data-stu-id="754c8-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="754c8-124">Alternativt navn for emne (begge er nødvendige): DNS = eksternt FQDN, DNS = intern FQDN</span><span class="sxs-lookup"><span data-stu-id="754c8-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="754c8-125">Installer NDES Connector med det nye sertifikatet.</span><span class="sxs-lookup"><span data-stu-id="754c8-125">Reinstall the NDES connector with the new certificate.</span></span>