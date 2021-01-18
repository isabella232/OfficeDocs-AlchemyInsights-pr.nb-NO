---
title: Proxy-konfigurasjon for App
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885522"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="7cb85-102">Proxy-konfigurasjon for App</span><span class="sxs-lookup"><span data-stu-id="7cb85-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="7cb85-103">Hvis du vil forstå hvordan du konfigurerer et program-proxy-program i Azure AD for å eksponere lokale programmer i skyen, kan du se [hvordan du konfigurerer en](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)programproxy for programmet.</span><span class="sxs-lookup"><span data-stu-id="7cb85-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="7cb85-104">Enkel pålogging (SSO) lar brukerne få tilgang til et program uten å godkjenne flere ganger.</span><span class="sxs-lookup"><span data-stu-id="7cb85-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="7cb85-105">Den gjør det mulig å utføre enkel godkjenning i skyen mot Azure Active Directory, og tillater tjenesten eller kontakten å representere brukeren for å fullføre eventuelle ytterligere godkjennings utfordringer fra programmet.</span><span class="sxs-lookup"><span data-stu-id="7cb85-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="7cb85-106">Hvis du vil ha mer informasjon, kan du se [Slik konfigurerer du enkel pålogging til et program-proxy-program](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="7cb85-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="7cb85-107">Bruk [denne artikkelen](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) til å feilsøke vanlige problemer som personer står overfor når du oppretter et nytt program-proxy-program.</span><span class="sxs-lookup"><span data-stu-id="7cb85-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="7cb85-108">Hvis du har problemer med å konfigurere bak godkjenning til programmet, må du kanskje [Feilsøke Kerberos-begrensede delegerings konfigurasjoner for programproxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) eller følge veiledning om [konfigurasjon av program med PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) for å løse problemet.</span><span class="sxs-lookup"><span data-stu-id="7cb85-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
