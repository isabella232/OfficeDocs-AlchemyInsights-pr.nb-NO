---
title: Problemer med integrering av sømløst SSO med de lokale appene
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868718"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="efc82-102">Problemer med integrering av sømløst SSO med de lokale appene</span><span class="sxs-lookup"><span data-stu-id="efc82-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="efc82-103">Hvis du vil feilsøke problemer med integrering av sømløst SSO med lokale programmer, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="efc82-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="efc82-104">**Anbefalte trinn**</span><span class="sxs-lookup"><span data-stu-id="efc82-104">**Recommended steps**</span></span>

1. <span data-ttu-id="efc82-105">Hvis du vil konfigurere et **lokalt program** for **enkel pålogging via program-proxy**, kan du se [passord hvelving for enkel pålogging med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span><span class="sxs-lookup"><span data-stu-id="efc82-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="efc82-106">**Feilsøke proxy-problemer med programmet**: Vi anbefaler at du starter med å se gjennom feil søkings flyt, [Feilsøk program for proxy Connector-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), for å finne ut om proxy-koblinger for appen er konfigurert riktig.</span><span class="sxs-lookup"><span data-stu-id="efc82-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="efc82-107">Hvis du fremdeles har problemer med å koble til programmet, følger du Fremgangs måten for feil søking i forbindelse med program for [proxy-program for Feilsøk](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span><span class="sxs-lookup"><span data-stu-id="efc82-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="efc82-108">Du kan [identifisere CORS-problemer](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ved å bruke følgende feil søkings verktøy for nett:</span><span class="sxs-lookup"><span data-stu-id="efc82-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="efc82-109">Start nett leseren, og gå til net tap pen.</span><span class="sxs-lookup"><span data-stu-id="efc82-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="efc82-110">Trykk **F12** for å åpne Debug-konsollen.</span><span class="sxs-lookup"><span data-stu-id="efc82-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="efc82-111">Prøv å gjenskape transaksjonen, og se gjennom konsoll meldingen.</span><span class="sxs-lookup"><span data-stu-id="efc82-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="efc82-112">Et CORS-brudd gir en konsoll feil om opprinnelse.</span><span class="sxs-lookup"><span data-stu-id="efc82-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="efc82-113">Noen CORS-problemer kan ikke løses, for eksempel når appen omdirigeres til login.microsoftonline.com for godkjenning, og tilgangstoken utløper.</span><span class="sxs-lookup"><span data-stu-id="efc82-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="efc82-114">CORS-samtalen mislykkes.</span><span class="sxs-lookup"><span data-stu-id="efc82-114">The CORS call then fails.</span></span> <span data-ttu-id="efc82-115">En midlertidig løsning for dette scenariet er å forlenge leve tiden til tilgangstoken for å hindre at det utløper under en brukers økt.</span><span class="sxs-lookup"><span data-stu-id="efc82-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="efc82-116">Hvis du vil ha mer informasjon om hvordan du gjør dette, kan du se [konfigurerbare token-leve tid i Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="efc82-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="efc82-117">**Anbefalte dokumenter**</span><span class="sxs-lookup"><span data-stu-id="efc82-117">**Recommended documents**</span></span>

- [<span data-ttu-id="efc82-118">Konfigurere enkel pålogging til et program-proxy-program</span><span class="sxs-lookup"><span data-stu-id="efc82-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="efc82-119">SAML Single Sign-on for lokale programmer med programproxy</span><span class="sxs-lookup"><span data-stu-id="efc82-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="efc82-120">Forstå og løse problemer med proxy-CORS for Azure Active Directory-app</span><span class="sxs-lookup"><span data-stu-id="efc82-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="efc82-121">Feilsøke konfigurasjoner med begrenset Kerberos-delegering for programproxy</span><span class="sxs-lookup"><span data-stu-id="efc82-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)