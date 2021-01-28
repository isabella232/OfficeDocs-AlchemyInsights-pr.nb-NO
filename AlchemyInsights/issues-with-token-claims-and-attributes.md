---
title: Problemer med tokenkrav og attributter
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035967"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="b3024-102">Problemer med tokenkrav og attributter</span><span class="sxs-lookup"><span data-stu-id="b3024-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="b3024-103">**Oppdatere, konfigurere eller fjerne tokenkrav**</span><span class="sxs-lookup"><span data-stu-id="b3024-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="b3024-104">Ved å bruke Azure Active Directory (Azure AD) kan du tilpasse kravtypen [for](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) rollekravet i svartokenet som du mottar etter at du har godkjent en app.</span><span class="sxs-lookup"><span data-stu-id="b3024-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="b3024-105">Programutviklere kan bruke valgfrie krav i Azure AD-programmene til å angi hvilke krav de ønsker i tokener som sendes til deres program.</span><span class="sxs-lookup"><span data-stu-id="b3024-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="b3024-106">Hvis du vil ha mer informasjon, [kan du se Oppgi valgfrie krav til appen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="b3024-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="b3024-107">[Konfigurer gruppekrav for programmer med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="b3024-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="b3024-108">Hvis du bruker sømløs enkel pålogging i programmet, kan du se tilpasse krav utstedt i [SAML-token for bedriftsprogrammer.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="b3024-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="b3024-109">**Attributttilordning for krav**</span><span class="sxs-lookup"><span data-stu-id="b3024-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="b3024-110">Hvis du vil konfigurere policy for kravtilordning ved hjelp av PowerShell, kan du se Tilpasse krav som sendes inn tokener for en bestemt app i [en leier (forhåndsvisning).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="b3024-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="b3024-111">Attributter for katalogskjemautvidelse gjør det mulig å lagre tilleggsdata i Azure Active Directory på brukerobjekter og andre katalogobjekter, for eksempel grupper, leierdetaljer, tjenesteprinsipper.</span><span class="sxs-lookup"><span data-stu-id="b3024-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="b3024-112">Bare utvidelsesattributter på brukerobjekter kan brukes for å sende krav til programmer.</span><span class="sxs-lookup"><span data-stu-id="b3024-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="b3024-113">[Bruk av attributter for katalogskjemautvidelse](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) i krav beskriver hvordan du bruker attributter for katalogskjemautvidelse til å sende brukerdata til programmer i tokenkrav.</span><span class="sxs-lookup"><span data-stu-id="b3024-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="b3024-114">Hvis du vil ha mer informasjon om tokenkrav, kan du se:</span><span class="sxs-lookup"><span data-stu-id="b3024-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="b3024-115">Krav i tilgangstoken</span><span class="sxs-lookup"><span data-stu-id="b3024-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="b3024-116">Krav i en id_token</span><span class="sxs-lookup"><span data-stu-id="b3024-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="b3024-117">[Krav](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) som du kan forvente i ID-tokener og tilgangstokener utstedt av Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="b3024-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="b3024-118">Referanse for SAML-tokenkrav</span><span class="sxs-lookup"><span data-stu-id="b3024-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
