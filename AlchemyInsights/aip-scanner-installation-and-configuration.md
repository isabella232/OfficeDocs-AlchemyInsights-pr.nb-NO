---
title: 'AIP-skanner: installasjon og konfigurasjon'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821672"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="712cb-102">AIP-skanner: installasjon og konfigurasjon</span><span class="sxs-lookup"><span data-stu-id="712cb-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="712cb-103">Følg de anbefalte retningslinjene for **å installere AIP-skanneren:**</span><span class="sxs-lookup"><span data-stu-id="712cb-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="712cb-104">Hvis du oppgraderer og ikke utfører en ren installasjon, må du kontrollere at du har fulgt retningslinjene for oppgradering av [Azure Information Protection-skanneren](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) og for enhetlig merkingsklient, se Oppgradere [Azure Information Protection-skanneren](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="712cb-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="712cb-105">Kontroller at du overholder alle [krav til brannmurer og innstillinger for nettverksinfrastruktur.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="712cb-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="712cb-106">Kontroller at [policyene er satt til](https://docs.microsoft.com/azure/information-protection/configure-policy) automatisk merking eller har en standardetikett i policyen.</span><span class="sxs-lookup"><span data-stu-id="712cb-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="712cb-107">Kontroller at den relevante filtypen er konfigurert for etikett/beskyttelse som beskrevet i Filtyper som støttes av [Azure Information Protection-klienten.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="712cb-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="712cb-108">Hvis du vil endre standard virkemåte, følger du i tillegg disse retningslinjene: Endre standard beskyttelsesnivå [for filer](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="712cb-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="712cb-109">Kontroller at brukerkontoen som er konfigurert til å kjøre skannertjenesten, har tillatelse til å få tilgang til alle konfigurerte repositorier.</span><span class="sxs-lookup"><span data-stu-id="712cb-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="712cb-110">Hvis du fremdeles opplever problemer, kan du eksportere skannerloggene og legge dem til i støtteforespørselen.</span><span class="sxs-lookup"><span data-stu-id="712cb-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="712cb-111">**Eksportere Azure Information Protection Scanner-logger**</span><span class="sxs-lookup"><span data-stu-id="712cb-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="712cb-112">Gå til %localappdata%\Microsoft\MSIP under brukerkonteksten som kjører skannertjenesten.</span><span class="sxs-lookup"><span data-stu-id="712cb-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="712cb-113">Zip alt innholdet under MSIP-mappen.</span><span class="sxs-lookup"><span data-stu-id="712cb-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="712cb-114">Lagre alle loggene på valgt plassering, og legg dem ved tjenesteforespørselen.</span><span class="sxs-lookup"><span data-stu-id="712cb-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="712cb-115">Du kan også bruke [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="712cb-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="712cb-116">**Hvis du vil ha mer informasjon, kan du se:**</span><span class="sxs-lookup"><span data-stu-id="712cb-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="712cb-117">Distribuere Azure Information Protection-skanneren for å automatisk klassifisere og beskytte filer</span><span class="sxs-lookup"><span data-stu-id="712cb-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="712cb-118">Angi og bruk Token-parameteren for Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="712cb-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="712cb-119">Kjøre en oppdagelsessyklus og vise rapporter for skanneren</span><span class="sxs-lookup"><span data-stu-id="712cb-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="712cb-120">Gå gjennom Azure Information Protection-dokumentasjon</span><span class="sxs-lookup"><span data-stu-id="712cb-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="712cb-121">Krav for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="712cb-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="712cb-122">Last ned Azure Information Protection-klient</span><span class="sxs-lookup"><span data-stu-id="712cb-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
