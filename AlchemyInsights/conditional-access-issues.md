---
title: Problemer med betinget tilgang
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014887"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="4f36b-102">Problemer med betinget tilgang</span><span class="sxs-lookup"><span data-stu-id="4f36b-102">Conditional access issues</span></span>

<span data-ttu-id="4f36b-103">**Løse problemer med påloggings diagnose**</span><span class="sxs-lookup"><span data-stu-id="4f36b-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="4f36b-104">Du kan raskt finne ut hva som skjedde eller diagnostisere problemer som er relatert til bruker pålogging ved hjelp av [påloggings diagnosen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="4f36b-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="4f36b-105">Start påloggings diagnosen.</span><span class="sxs-lookup"><span data-stu-id="4f36b-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="4f36b-106">Finn hendelsen for å analysere ved å angi i detaljene du har om brukeren, programmet, påloggings tidspunktet, forespørsels-ID-en eller korrelasjons-IDen.</span><span class="sxs-lookup"><span data-stu-id="4f36b-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="4f36b-107">Se gjennom diagnose resultatene som viser informasjon om hva som skjedde og hvilke handlinger du kan utføre for å gjøre endringer (hvis det er nødvendig med endringer).</span><span class="sxs-lookup"><span data-stu-id="4f36b-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="4f36b-108">**Fremgangs måte for å feilsøke påloggings problemer**</span><span class="sxs-lookup"><span data-stu-id="4f36b-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="4f36b-109">Gå til påloggings siden for Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4f36b-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="4f36b-110">Filtrer pålogginger etter bruker, tids intervall, program, status, klient program og så videre.</span><span class="sxs-lookup"><span data-stu-id="4f36b-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="4f36b-111">Velg en påloggings hendelse, og Vis betinget tilgang-fanen for å se hvilke policyer som ble evaluert.</span><span class="sxs-lookup"><span data-stu-id="4f36b-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="4f36b-112">Klikk på raden i en policy for å vise policy detaljene og forstå hvorfor den er brukt.</span><span class="sxs-lookup"><span data-stu-id="4f36b-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="4f36b-113">**Verktøy for å feilsøke en policy for betinget tilgang**</span><span class="sxs-lookup"><span data-stu-id="4f36b-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="4f36b-114">Bare rapport modus lar deg evaluere en policy uten å påvirke brukere.</span><span class="sxs-lookup"><span data-stu-id="4f36b-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="4f36b-115">Hva-skjer-hvis-verktøyet lar deg simulere påloggings hendelser og se hvilke policyer som gjelder.</span><span class="sxs-lookup"><span data-stu-id="4f36b-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="4f36b-116">Innsikt-og rapporterings arbeids bok viser sann tids innvirkning for hver policy.</span><span class="sxs-lookup"><span data-stu-id="4f36b-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="4f36b-117">**Policyer for grunn linje beskyttelse**</span><span class="sxs-lookup"><span data-stu-id="4f36b-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="4f36b-118">Policyer for grunn linje beskyttelse er avverget.</span><span class="sxs-lookup"><span data-stu-id="4f36b-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="4f36b-119">De blir ikke lenger håndhevet og vil snart bli fjernet fra Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="4f36b-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="4f36b-120">Vi anbefaler at du aktiverer [sikkerhets standarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="4f36b-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="4f36b-121">Hvis du vil ha mer informasjon om betinget tilgang, kan du se:</span><span class="sxs-lookup"><span data-stu-id="4f36b-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="4f36b-122">[Anbefalte Fremgangs måter for betinget tilgang i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Betingelser i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontroller i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Plasseringer i betinget tilgang](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="4f36b-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
