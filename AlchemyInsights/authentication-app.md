---
title: Godkjenningsapp
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405067"
---
# <a name="authentication-app"></a><span data-ttu-id="3bae0-102">Godkjenningsapp</span><span class="sxs-lookup"><span data-stu-id="3bae0-102">Authentication app</span></span>

<span data-ttu-id="3bae0-103">Hvis du er global administrator, kan du raskt finne ut hva som skjedde eller diagnostisere problemer relatert til brukerlogging ved hjelp av [påloggingsdiagnose](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="3bae0-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="3bae0-104">Start diagnostikken ved å klikke[startdiagnose-knappen.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="3bae0-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="3bae0-105">Finn hendelsen du vil analysere, ved å skrive inn detaljene du har om brukeren, programmet, tidspunktet for pålogging, forespørsels-ID eller korrelasjons-ID.</span><span class="sxs-lookup"><span data-stu-id="3bae0-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="3bae0-106">Se gjennom diagnoseresultatene som viser detaljer om hva som skjedde og hvilke handlinger du kan utføre for å gjøre endringer, hvis det er nødvendig med endringer.</span><span class="sxs-lookup"><span data-stu-id="3bae0-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="3bae0-107">**Kontroller scenarioet som gjelder:**</span><span class="sxs-lookup"><span data-stu-id="3bae0-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="3bae0-108">Hvis en bruker ikke får et push-varsel i Microsoft Authenticator-appen, må du kontrollere at de ikke vises under de MFA-blokkerte brukerne, som beskrevet i Blokkere og [oppheve blokkeringen av brukere.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="3bae0-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="3bae0-109">Hvis brukeren ikke er blokkert for MFA, men ikke mottar en push-varsling, kan de åpne Microsoft Authenticator-appen, som vil trekke ventende godkjenningsforespørsler.</span><span class="sxs-lookup"><span data-stu-id="3bae0-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="3bae0-110">Som en alternativ påloggingsmetode kan brukeren også klikke på Logg på en annen måte og velge å bruke en bekreftelseskode fra mobilappen.</span><span class="sxs-lookup"><span data-stu-id="3bae0-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="3bae0-111">Microsoft Authenticator-appen er den eneste tilgjengelige metoden for mange brukere.</span><span class="sxs-lookup"><span data-stu-id="3bae0-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="3bae0-112">[Finn ut mer om sikkerhetsstandarder](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), se Vanlige spørsmål om [Authenticator-appen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for vanlige spørsmål og hvordan du løser dem.</span><span class="sxs-lookup"><span data-stu-id="3bae0-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="3bae0-113">**Anbefalte videoer**</span><span class="sxs-lookup"><span data-stu-id="3bae0-113">**Recommended Videos**</span></span>

<span data-ttu-id="3bae0-114">[Slik konfigurerer du Authenticator-appen på en ny telefon (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="3bae0-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
