---
title: 'AIP-skanner: installasjon og konfigurasjon'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358102"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="18b04-102">AIP-skanner: installasjon og konfigurasjon</span><span class="sxs-lookup"><span data-stu-id="18b04-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="18b04-103">**Hvis du vil installere AIP-skanneren, følger du de anbefalte retningslinjene:**</span><span class="sxs-lookup"><span data-stu-id="18b04-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="18b04-104">Hvis du oppgraderer og ikke utfører en ren installasjon, må du kontrollere at du har fulgt retningslinjene for [oppgradering av Azure Information Protection-skanneren](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) og for enhetlig merkingsklient, kan du se oppgradere Azure Information [Protection-skanneren](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="18b04-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="18b04-105">Kontroller at du overholder alle [krav til innstillinger for brannmurer og nettverksinfrastruktur](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="18b04-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="18b04-106">Kontroller at [policyene](https://docs.microsoft.com/azure/information-protection/configure-policy) dine er satt til automatisk merking eller har en standardetikett i policyen.</span><span class="sxs-lookup"><span data-stu-id="18b04-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="18b04-107">Kontroller at den relevante filtypen er konfigurert for etikett/beskyttelse som beskrevet i [Filtyper som støttes av Azure Information Protection-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="18b04-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="18b04-108">Hvis du vil endre standardvirkemåten, følger du i tillegg disse retningslinjene: [Endre standard beskyttelsesnivå for filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="18b04-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="18b04-109">Kontroller at brukerkontoen som er konfigurert til å kjøre skannertjenesten, har tillatelse til å få tilgang til alle de konfigurerte repositoriene.</span><span class="sxs-lookup"><span data-stu-id="18b04-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="18b04-110">Hvis du fortsatt har problemer, må du eksportere skannerloggene og legge dem til i støttebilletten.</span><span class="sxs-lookup"><span data-stu-id="18b04-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="18b04-111">**Eksportere Azure Information Protection Scanner-logger**</span><span class="sxs-lookup"><span data-stu-id="18b04-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="18b04-112">Gå til %localappdata%\Microsoft\MSIP under brukerkonteksten som kjører skannertjenesten.</span><span class="sxs-lookup"><span data-stu-id="18b04-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="18b04-113">Zip alt innholdet under MSIP-mappen.</span><span class="sxs-lookup"><span data-stu-id="18b04-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="18b04-114">Lagre loggene i ditt valg av sted, og legg dem ved serviceforespørselen.</span><span class="sxs-lookup"><span data-stu-id="18b04-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="18b04-115">Du kan også bruke [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="18b04-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="18b04-116">**Hvis du vil ha mer informasjon, kan du se**:</span><span class="sxs-lookup"><span data-stu-id="18b04-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="18b04-117">Distribuere Azure Information Protection-skanneren for å klassifisere og beskytte filer automatisk</span><span class="sxs-lookup"><span data-stu-id="18b04-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="18b04-118">Angi og bruke tokenparameteren for Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="18b04-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="18b04-119">Kjøre en oppdagelsessyklus og vise rapporter for skanneren</span><span class="sxs-lookup"><span data-stu-id="18b04-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="18b04-120">Se gjennom dokumentasjonen for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="18b04-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="18b04-121">Krav til Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="18b04-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="18b04-122">Last ned Azure Information Protection-klienten</span><span class="sxs-lookup"><span data-stu-id="18b04-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
