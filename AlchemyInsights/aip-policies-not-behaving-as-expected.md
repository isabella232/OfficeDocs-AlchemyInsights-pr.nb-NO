---
title: 'AIP: Retningslinjer oppfører seg ikke som forventet'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493162"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="b02d0-102">AIP: Retningslinjer oppfører seg ikke som forventet</span><span class="sxs-lookup"><span data-stu-id="b02d0-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="b02d0-103">Azure Information Protection: Policyer som ikke fungerer som forventet, kan du se følgende for anbefalte retningslinjer for ulike policyproblemer:</span><span class="sxs-lookup"><span data-stu-id="b02d0-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="b02d0-104">Hvis du har problemer med visuelle markeringer, kan du se [Når visuelle markeringer brukes](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="b02d0-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="b02d0-105">Hvis du har problemer med automatisk merking, kan du se Slik konfigurerer du [betingelser for automatisk og anbefalt klassifisering for Azure Information Protection og](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) Hva de sensitive [informasjonstypene ser etter](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="b02d0-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="b02d0-106">Hvis du har problemer med opprinnelig/pfile beskyttelse, kan du se [fil-API-konfigurasjon](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="b02d0-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="b02d0-107">Kontroller om du bruker policyer for omfang som ikke er riktig konfigurert: Slik konfigurerer du [policyen for Azure information protection for bestemte brukere ved hjelp av policyer for omfang](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="b02d0-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="b02d0-108">Hvis automatisk merking ikke fungerer for Outlook når du legger ved et merket dokument, må du kontrollere at DRMEncryptProperty ikke er definert som beskrevet her: [IRM-registerinnstillinger for sikkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="b02d0-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="b02d0-109">Hvis du fortsatt har problemer, kan du samle inn Azure Information Protection-klientlogger og legge ved de eksporterte loggene til denne billetten.</span><span class="sxs-lookup"><span data-stu-id="b02d0-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="b02d0-110">Åpne et Office-dokument eller opprett en ny e-post i Outlook.</span><span class="sxs-lookup"><span data-stu-id="b02d0-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="b02d0-111">Klikk På Hjelp og tilbakemelding **for beskyttelse/følsomhet**  >  **Help and feedback**.</span><span class="sxs-lookup"><span data-stu-id="b02d0-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="b02d0-112">Klikk **Eksporter logger**.</span><span class="sxs-lookup"><span data-stu-id="b02d0-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="b02d0-113">Lagre loggene til ditt valg av plassering, og legg dem ved denne serviceforespørselen.</span><span class="sxs-lookup"><span data-stu-id="b02d0-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="b02d0-114">Flere ressurser:</span><span class="sxs-lookup"><span data-stu-id="b02d0-114">Additional resources:</span></span>

- [<span data-ttu-id="b02d0-115">Slik konfigurerer du en etikett for visuelle markeringer for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b02d0-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="b02d0-116">Se gjennom dokumentasjonen for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="b02d0-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="b02d0-117">Bruke følsomhetsetiketter i Office-apper</span><span class="sxs-lookup"><span data-stu-id="b02d0-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

