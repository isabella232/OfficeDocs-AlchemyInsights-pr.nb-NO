---
title: Arbeide med godkjenningsbiblioteker
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035826"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="32da6-102">Arbeide med godkjenningsbiblioteker</span><span class="sxs-lookup"><span data-stu-id="32da6-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="32da6-103">Hvis du vil løse problemet med Microsoft Authentication Library (MSAL), utfører du følgende anbefalte trinn:</span><span class="sxs-lookup"><span data-stu-id="32da6-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="32da6-104">**Arbeide med MSAL:** [Godkjenningsbiblioteker for Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – Denne artikkelen viser støtte for Microsoft Authentication Library for flere programtyper.</span><span class="sxs-lookup"><span data-stu-id="32da6-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="32da6-105">Den inneholder koblinger til kildekoden for biblioteket. hvor du får pakken for appens prosjekt; og om biblioteket støtter bruker pålogging (godkjenning), tilgang til beskyttede web-API-er (autorisasjon) eller begge deler.</span><span class="sxs-lookup"><span data-stu-id="32da6-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="32da6-106">**Feilsøkingsgodkjenning:** MSAL støtter flere godkjenningsflyter for bruk i ulike programscenarioer.</span><span class="sxs-lookup"><span data-stu-id="32da6-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="32da6-107">Avhengig av hvordan klientprogrammet er bygd, kan MSAL bruke én eller flere av godkjenningsflytene som støttes av Microsoft-identitetsplattformen.</span><span class="sxs-lookup"><span data-stu-id="32da6-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="32da6-108">Disse flytene kan produsere flere typer tokener og autorisasjonskoder, og kreve ulike tokener for å få dem til å fungere.</span><span class="sxs-lookup"><span data-stu-id="32da6-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="32da6-109">**Tilgangstokener:** [Tilgangstokener for Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Finn ut hvordan API-en kan validere og bruke påstandene i et tilgangstoken.</span><span class="sxs-lookup"><span data-stu-id="32da6-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="32da6-110">All dokumentasjon i denne artikkelen, unntatt der det er notert, gjelder bare for tokener utstedt for API-er du har registrert.</span><span class="sxs-lookup"><span data-stu-id="32da6-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="32da6-111">Det gjelder ikke tokener utstedt for Microsoft-eide API-er, og disse tokenene kan heller ikke brukes til å validere hvordan Microsoft-identitetsplattformen vil utstede tokener for en API du oppretter.</span><span class="sxs-lookup"><span data-stu-id="32da6-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="32da6-112">**Slutt på støtte for Azure Active Directory Authentication Library (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="32da6-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="32da6-113">**Fra og med 30. juni 2020** legger vi ikke lenger til noen nye funksjoner i ADAL og Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="32da6-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="32da6-114">Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.</span><span class="sxs-lookup"><span data-stu-id="32da6-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="32da6-115">**Fra og med 30. juni 2022** avslutter vi støtte for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.</span><span class="sxs-lookup"><span data-stu-id="32da6-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="32da6-116">Apper som bruker ADAL på eksisterende OS-versjoner, vil fortsette å fungere etter dette tidspunktet, men vil ikke få teknisk *støtte eller sikkerhetsoppdateringer.*</span><span class="sxs-lookup"><span data-stu-id="32da6-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="32da6-117">Apper som bruker Azure AD Graph etter dette tidspunktet, mottar kanskje ikke lenger svar fra Azure AD Graph-endepunktet.</span><span class="sxs-lookup"><span data-stu-id="32da6-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="32da6-118">**ADAL-overføring**</span><span class="sxs-lookup"><span data-stu-id="32da6-118">**ADAL Migration**</span></span>

- <span data-ttu-id="32da6-119">Vi anbefaler å oppdatere til MSAL, som har de nyeste funksjonene og sikkerhetsoppdateringene.</span><span class="sxs-lookup"><span data-stu-id="32da6-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="32da6-120">Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre appene til MSAL innen tidsfristen for kundestøtten utløper, slik at de vil dra nytte av MSAL sine pågående sikkerhets- og funksjonsforbedringer.</span><span class="sxs-lookup"><span data-stu-id="32da6-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="32da6-121">[Les vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="32da6-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="32da6-122">[Lær om hvordan du overfører apper per plattform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="32da6-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="32da6-123">Hvis du har flere spørsmål etter å ha lest veiledningen for appens plattform, kan du publisere på [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) med koden [azure-ad-adal-deprecation] eller åpne et problem i bibliotekets GitHub-repositorium.</span><span class="sxs-lookup"><span data-stu-id="32da6-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="32da6-124">Se [språk- og rammeverkdelen i](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) **MSAL-oversiktsartikkelen** for koblinger til hvert biblioteks repo.</span><span class="sxs-lookup"><span data-stu-id="32da6-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="32da6-125">Hvis du trenger hjelp til å forstå hvilke av **appene som bruker ADAL,** anbefaler vi at du ser gjennom kildekoden til alle appene dine.</span><span class="sxs-lookup"><span data-stu-id="32da6-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="32da6-126">Hvis det er aktuelt, kan du ta kontakt med uavhengige programvareleverandører (ISV-er) eller appleverandører.</span><span class="sxs-lookup"><span data-stu-id="32da6-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="32da6-127">Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.</span><span class="sxs-lookup"><span data-stu-id="32da6-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







