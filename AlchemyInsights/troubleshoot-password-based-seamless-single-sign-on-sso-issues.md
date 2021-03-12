---
title: Feilsøke problemer med passordbasert enkel pålogging (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714881"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="56fc1-102">Feilsøke problemer med passordbasert enkel pålogging (SSO)</span><span class="sxs-lookup"><span data-stu-id="56fc1-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="56fc1-103">Hvis du vil lære det grunnleggende om passordbasert SSO, kan du se [passordbasert godkjenning med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="56fc1-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="56fc1-104">**Konfigurere passordbasert SSO**</span><span class="sxs-lookup"><span data-stu-id="56fc1-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="56fc1-105">[Konfigurere passordbasert enkel pålogging](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – Denne artikkelen handler mer om det passordbaserte SSO-alternativet.</span><span class="sxs-lookup"><span data-stu-id="56fc1-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="56fc1-106">Hvis programmet du legger til, krever egendefinert konfigurasjon og du må bruke passordbasert SSO, er denne artikkelen for deg.</span><span class="sxs-lookup"><span data-stu-id="56fc1-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="56fc1-107">[Konfigurere passordbasert enkel pålogging for](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) apper som er forhåndsinstallert – Programproxy støtter flere modus for enkel pålogging.</span><span class="sxs-lookup"><span data-stu-id="56fc1-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="56fc1-108">Passordbasert pålogging er beregnet for programmer som bruker en brukernavn-/passordkombinasjon for godkjenning.</span><span class="sxs-lookup"><span data-stu-id="56fc1-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="56fc1-109">Når du konfigurerer passordbasert pålogging for programmet, må brukerne logge seg på det lokale programmet én gang.</span><span class="sxs-lookup"><span data-stu-id="56fc1-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="56fc1-110">Deretter lagrer Azure Active Directory påloggingsinformasjonen og automatisk gir den til programmet når brukerne får ekstern tilgang til det.</span><span class="sxs-lookup"><span data-stu-id="56fc1-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="56fc1-111">Du skal allerede ha publisert og testet appen med programproxy.</span><span class="sxs-lookup"><span data-stu-id="56fc1-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="56fc1-112">Hvis ikke, følger du fremgangsmåten i Publiser programmer ved hjelp av Azure AD-programproxy, og deretter fortsetter du konfigurasjonen av passordbasert SSO for programmer som er forhåndsinstallert. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)</span><span class="sxs-lookup"><span data-stu-id="56fc1-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="56fc1-113">Hvis du vil feilsøke passordbasert SSO, kan du se [Feilsøke passordbasert](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) enkel pålogging i Azure AD</span><span class="sxs-lookup"><span data-stu-id="56fc1-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
