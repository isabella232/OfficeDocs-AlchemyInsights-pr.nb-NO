---
title: SAML-deklarasjoner (tokener)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885670"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="ba250-102">SAML-deklarasjoner (tokener)</span><span class="sxs-lookup"><span data-stu-id="ba250-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="ba250-103">Sikkerhets deklarasjoner Markup Language (SAML)-tokener er XML representasjoner av krav.</span><span class="sxs-lookup"><span data-stu-id="ba250-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="ba250-104">Som standard er Windows Communication Foundation (WCF) som bruker i sikkerhets scenarioer i organisasjons nettverk utsteder koder.</span><span class="sxs-lookup"><span data-stu-id="ba250-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="ba250-105">Hvis du vil ha mer informasjon, kan du se [SAML tokens og krav](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="ba250-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="ba250-106">Microsoft Identity Platform sender ut flere typer sikkerhetstokener i behandlingen av hver godkjennings flyt.</span><span class="sxs-lookup"><span data-stu-id="ba250-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="ba250-107">[Referansen for krav til SAML-token](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) beskriver formatet, sikkerhets egenskapene og innholdet i SAML 2,0-tokener.</span><span class="sxs-lookup"><span data-stu-id="ba250-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="ba250-108">Følg rettledningen i [konfigurerbare token-leve tid i Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) for å forstå hvordan du konfigurerer token-leve tid.</span><span class="sxs-lookup"><span data-stu-id="ba250-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="ba250-109">Følg Fremgangs måten i [denne artikkelen](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) for å forstå hvordan du konfigurerer Azure ad SAML token Encryption.</span><span class="sxs-lookup"><span data-stu-id="ba250-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="ba250-110">I Azure AD kan du konfigurere alternativer for sertifikat signering og algoritme for sertifikat signering.</span><span class="sxs-lookup"><span data-stu-id="ba250-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="ba250-111">Hvis du vil ha mer informasjon, kan du se [Avanserte alternativer for sertifikat signering i SAML-token for Gallery-apper i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="ba250-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
