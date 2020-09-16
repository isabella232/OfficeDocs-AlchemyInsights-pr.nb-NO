---
title: 'INSTALLASJONs vilkår: policyer ikke oppfører seg som forventet'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663198"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="3606e-102">INSTALLASJONs vilkår: policyer ikke oppfører seg som forventet</span><span class="sxs-lookup"><span data-stu-id="3606e-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="3606e-103">Azure Information Protection: policyer ikke oppfører seg som forventet, kan du se følgende for anbefalte retnings linjer for ulike policy problemer:</span><span class="sxs-lookup"><span data-stu-id="3606e-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="3606e-104">Hvis du har problemer med visuelle markeringer, kan du se gjennom [når visuelle markeringer brukes](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="3606e-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="3606e-105">Hvis du har problemer med automatisk merking, kan du se [hvordan du konfigurerer betingelser for automatisk og anbefalt klassifisering for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) og [hva de sensitive informasjons typene ser ut for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="3606e-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="3606e-106">Hvis du har problemer med opprinnelig/Pfile beskyttelse, kan du se [fil-API-konfigurasjonen](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="3606e-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="3606e-107">Kontroller om du bruker omfangs policyer som ikke er riktig konfigurert: [Slik konfigurerer du policyen for Azure Information Protection for bestemte brukere ved hjelp av omfangs policyer](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="3606e-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="3606e-108">Hvis automatisk merking ikke fungerer for Outlook når du legger ved et merket dokument, må du bekrefte at DRMEncryptProperty ikke er definert som beskrevet her: [IRM-register innstillinger for sikkerhet](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="3606e-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="3606e-109">Hvis du fremdeles har problemer, kan du samle inn klient logger for Azure Information Protection og knytte de eksporterte loggene til denne billetten.</span><span class="sxs-lookup"><span data-stu-id="3606e-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="3606e-110">Åpne et Office-dokument eller opprette en ny e-post i Outlook.</span><span class="sxs-lookup"><span data-stu-id="3606e-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="3606e-111">Klikk **Beskytt/følsomhet**  >  **Hjelp og tilbake melding**.</span><span class="sxs-lookup"><span data-stu-id="3606e-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="3606e-112">Klikk **Eksporter logger**.</span><span class="sxs-lookup"><span data-stu-id="3606e-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="3606e-113">Lagre loggene på valg av sted, og legg dem ved denne service forespørselen.</span><span class="sxs-lookup"><span data-stu-id="3606e-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="3606e-114">Flere ressurser:</span><span class="sxs-lookup"><span data-stu-id="3606e-114">Additional resources:</span></span>

- [<span data-ttu-id="3606e-115">Slik konfigurerer du en etikett for visuelle markeringer for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="3606e-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="3606e-116">Gå gjennom dokumentasjon for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="3606e-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="3606e-117">Bruk følsomhet-etiketter i Microsoft 365-apper</span><span class="sxs-lookup"><span data-stu-id="3606e-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

