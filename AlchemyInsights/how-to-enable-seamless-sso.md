---
title: Slik aktiverer du Sømløs SSO
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825740"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="0aa36-102">Slik aktiverer du Sømløs SSO</span><span class="sxs-lookup"><span data-stu-id="0aa36-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="0aa36-103">Aktiver sømløs SSO via [Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)</span><span class="sxs-lookup"><span data-stu-id="0aa36-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="0aa36-104">Hvis du gjør en ny installasjon av Azure AD Connect, velger du den [egendefinerte installasjonsbanen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="0aa36-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="0aa36-105">På **brukerloggingssiden** velger du alternativet **Aktiver enkel pålogging.**</span><span class="sxs-lookup"><span data-stu-id="0aa36-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="0aa36-106">Slik kontrollerer du at du har aktivert Sømløs SSO på riktig måte:</span><span class="sxs-lookup"><span data-stu-id="0aa36-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="0aa36-107">Logg på [administrasjonssenteret for Azure Active Directory](https://aad.portal.azure.com) som global administrator.</span><span class="sxs-lookup"><span data-stu-id="0aa36-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="0aa36-108">Velg **Azure Active Directory** i den venstre ruten.</span><span class="sxs-lookup"><span data-stu-id="0aa36-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="0aa36-109">Kontroller at Sømløs enkel pålogging er **aktivert**.</span><span class="sxs-lookup"><span data-stu-id="0aa36-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="0aa36-110">Hvis du vil ha mer informasjon, kan du se Sømløs enkel pålogging [for Azure Active Directory: Hurtigstart](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="0aa36-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  