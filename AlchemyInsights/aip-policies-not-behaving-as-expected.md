---
title: 'AIP: Policyer oppfører seg ikke som forventet'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821636"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="3454c-102">AIP: Policyer oppfører seg ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="3454c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="3454c-103">Azure Information Protection: Policyer oppfører seg ikke som forventet, se følgende for anbefalte retningslinjer for ulike policyproblemer:</span><span class="sxs-lookup"><span data-stu-id="3454c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="3454c-104">Hvis du har problemer med visuelle markeringer, kan du se [gjennom Når visuelle markeringer brukes](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="3454c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="3454c-105">Hvis du har problemer med automatisk merking, kan du se Slik konfigurerer du betingelser for automatisk og anbefalt klassifisering [for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og Hva ser de sensitive [informasjonstypene etter.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="3454c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="3454c-106">Hvis du har problemer med opprinnelig/Pfile-beskyttelse, kan du se [Fil-API-konfigurasjonen](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="3454c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="3454c-107">Kontroller om du bruker begrensede policyer som ikke er riktig konfigurert: Slik konfigurerer du policyen for Azure Information Protection for bestemte brukere ved hjelp [av omfangsbestemte policyer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="3454c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="3454c-108">Hvis automatisk merking ikke fungerer for Outlook når du legger ved et merket dokument, må du kontrollere at DRMEncryptProperty ikke er definert som beskrevet her: [IRM-registerinnstillinger for sikkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="3454c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="3454c-109">Hvis du fremdeles har problemer, kan du samle inn Azure Information Protection-klientlogger og legge ved de eksporterte loggene i denne billetten.</span><span class="sxs-lookup"><span data-stu-id="3454c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="3454c-110">Åpne et Office-dokument eller opprett en ny e-postmelding i Outlook.</span><span class="sxs-lookup"><span data-stu-id="3454c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="3454c-111">Klikk **Beskytt/følsomhet**  >  **Hjelp og tilbakemelding**.</span><span class="sxs-lookup"><span data-stu-id="3454c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="3454c-112">Klikk **Eksporter logger**.</span><span class="sxs-lookup"><span data-stu-id="3454c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="3454c-113">Lagre loggene på ønsket plassering, og legg dem ved denne serviceforespørselen.</span><span class="sxs-lookup"><span data-stu-id="3454c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="3454c-114">Flere ressurser:</span><span class="sxs-lookup"><span data-stu-id="3454c-114">Additional resources:</span></span>

- [<span data-ttu-id="3454c-115">Slik konfigurerer du en etikett for visuelle markeringer for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="3454c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="3454c-116">Se gjennom dokumentasjonen for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="3454c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="3454c-117">Bruke følsomhetsetiketter i Microsoft 365-apper</span><span class="sxs-lookup"><span data-stu-id="3454c-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

