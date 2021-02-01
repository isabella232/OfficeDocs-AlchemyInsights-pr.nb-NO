---
title: Problemer med godkjenningsbiblioteker
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063639"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="a905e-102">Problemer med godkjenningsbiblioteker</span><span class="sxs-lookup"><span data-stu-id="a905e-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="a905e-103">[Biblioteker for Godkjenning av Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) viser biblioteker for Microsoft-støttede og kompatible klienter og middleware.</span><span class="sxs-lookup"><span data-stu-id="a905e-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="a905e-104">Microsoft Authentication Library (MSAL) støtter flere [godkjenningsflyter](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for bruk i ulike programscenarier.</span><span class="sxs-lookup"><span data-stu-id="a905e-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="a905e-105">Hvis du vil godkjenne og skaffe tokener, initialiserer du et nytt offentlig eller konfidensielt klientprogram i koden.</span><span class="sxs-lookup"><span data-stu-id="a905e-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="a905e-106">Du kan angi flere konfigurasjonsalternativer når du initialiserer klientappen i Microsoft Authentication Library (MSAL).</span><span class="sxs-lookup"><span data-stu-id="a905e-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="a905e-107">Hvis du vil ha mer informasjon, kan du [se konfigurasjonsalternativer for programmet.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="a905e-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="a905e-108">**Slutt på støtte for Azure Active Directory Authentication Library (ADAL) og Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="a905e-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="a905e-109">**Fra og med 30. juni 2020** vil vi ikke lenger legge til nye funksjoner i ADAL og Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="a905e-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="a905e-110">Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.</span><span class="sxs-lookup"><span data-stu-id="a905e-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="a905e-111">**Fra og med 30. juni 2022** avslutter vi støtten for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.</span><span class="sxs-lookup"><span data-stu-id="a905e-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="a905e-112">Apper som bruker ADAL på eksisterende OS-versjoner, vil fortsette å fungere etter dette tid, men vil ikke få noen teknisk støtte *eller sikkerhetsoppdateringer.*</span><span class="sxs-lookup"><span data-stu-id="a905e-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="a905e-113">Apper som bruker Azure AD Graph etter dette tid, kan ikke lenger motta svar fra Azure AD Graph-endepunktet.</span><span class="sxs-lookup"><span data-stu-id="a905e-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="a905e-114">**ADAL-overføring**</span><span class="sxs-lookup"><span data-stu-id="a905e-114">**ADAL Migration**</span></span>

<span data-ttu-id="a905e-115">Vi anbefaler at du oppdaterer til [Microsofts godkjenningbibliotek (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de nyeste funksjonene og sikkerhetsoppdateringene.</span><span class="sxs-lookup"><span data-stu-id="a905e-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="a905e-116">Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre programmene til MSAL innen tidsfristen for slutten av støtten, slik at de vil dra nytte av MSALs pågående sikkerhets- og funksjonsforbedringer.</span><span class="sxs-lookup"><span data-stu-id="a905e-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="a905e-117">Hvis du vil ha mer informasjon, kan du se:</span><span class="sxs-lookup"><span data-stu-id="a905e-117">For more information, see:</span></span>

1. [<span data-ttu-id="a905e-118">Les Vanlige spørsmål om ADAL</span><span class="sxs-lookup"><span data-stu-id="a905e-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="a905e-119">Finn ut hvordan du overfører apper per plattform</span><span class="sxs-lookup"><span data-stu-id="a905e-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="a905e-120">Hvis du trenger hjelp til å forstå hvilke apper som bruker ADAL, anbefaler vi at du går gjennom alle appenes kildekode, og hvis aktuelt, kan du ta kontakt med eventuelle ISV-er eller appleverandører.</span><span class="sxs-lookup"><span data-stu-id="a905e-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="a905e-121">Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a905e-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="a905e-122">**AAD Graph-overføring**</span><span class="sxs-lookup"><span data-stu-id="a905e-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="a905e-123">For programmer som bruker Azure AD Graph, følger du veiledningen vår for [å overføre Azure AD Graph-apper til Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="a905e-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="a905e-124">Sjekklisten for overføring gir deg et komme i gang-punkt.</span><span class="sxs-lookup"><span data-stu-id="a905e-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="a905e-125">Appregistreringsportalen for Azure viser hvilke programmer som bruker AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="a905e-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="a905e-126">Vi anbefaler at du ser gjennom kildekoden for alle appene, og hvis det er aktuelt, tar du kontakt med en uavhengig programvareleverandør eller appleverandør.</span><span class="sxs-lookup"><span data-stu-id="a905e-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="a905e-127">Microsoft Kundestøtte kan også gi deg en liste over all AAD Graph-bruk i tenanten din.</span><span class="sxs-lookup"><span data-stu-id="a905e-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="a905e-128">Brukeren eller administratoren må gi appen de riktige tillatelsene via en samtykkeprosess for at den skal få tilgang til data i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a905e-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="a905e-129">[Tillatelsesreferansen for Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) viser tillatelsene som er knyttet til hvert hovedsett av Microsoft Graph API-er.</span><span class="sxs-lookup"><span data-stu-id="a905e-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="a905e-130">Den gir også veiledning om hvordan du bruker tillatelsene.</span><span class="sxs-lookup"><span data-stu-id="a905e-130">It also provides guidance about how to use the permissions.</span></span>
