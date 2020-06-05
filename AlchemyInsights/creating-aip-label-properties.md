---
title: Opprette policyer for AIP-etikett
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569506"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="89b9d-102">Opprette policyer for AIP-etikett</span><span class="sxs-lookup"><span data-stu-id="89b9d-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="89b9d-103">Azure Information Protection(AIP)-etiketter kan brukes med hele spekteret av data som en organisasjon vanligvis oppretter og lagrer, fra den laveste klassifiseringen av personopplysninger, til den høyeste klassifiseringen av svært konfidensielle data.</span><span class="sxs-lookup"><span data-stu-id="89b9d-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="89b9d-104">Azure Information Protection Policies gjelder for den klassiske azure-klienten for informasjonsbeskyttelse(AIP) og ikke [AIP Unified Labeling-klienten](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="89b9d-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="89b9d-105">Du kan konfigurere flere elementer i en AIP-policy, inkludert alternativer som:</span><span class="sxs-lookup"><span data-stu-id="89b9d-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="89b9d-106">Alternativ for hvilken etikett som lar administratorer eller bruker klassifisere og beskytte (valgfrie) dokumenter og e-poster</span><span class="sxs-lookup"><span data-stu-id="89b9d-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="89b9d-107">Mulighet til å håndheve klassifisering når brukere lagrer dokumenter og sender e-post</span><span class="sxs-lookup"><span data-stu-id="89b9d-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="89b9d-108">Alternativ for å merke en e-postmelding automatisk, basert på vedleggene.</span><span class="sxs-lookup"><span data-stu-id="89b9d-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="89b9d-109">Alternativ for å kontrollere om informasjonsbeskyttelseslinjen vises i Office-programmer</span><span class="sxs-lookup"><span data-stu-id="89b9d-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="89b9d-110">Hvis du vil ha flere alternativer og informasjon om policyer for Azure Information Protection, kan du se: [Oversikt over policyen for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="89b9d-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="89b9d-111">Hvis du vil ha andre nyttige ressurser angående AIP-policyer, kan du se:</span><span class="sxs-lookup"><span data-stu-id="89b9d-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="89b9d-112">Opplæring: Konfigurere policyinnstillingene for Azure Information Protection og opprette en ny etikett</span><span class="sxs-lookup"><span data-stu-id="89b9d-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="89b9d-113">Konfigurere azure informasjonsbeskyttelsespolicy</span><span class="sxs-lookup"><span data-stu-id="89b9d-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="89b9d-114">Opprette og konfigurere følsomhetsetiketter og deres policyer</span><span class="sxs-lookup"><span data-stu-id="89b9d-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="89b9d-115">Veiledninger for vanlige scenarier som bruker Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="89b9d-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="89b9d-116">Se gjennom dokumentasjonen for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="89b9d-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="89b9d-117">Krav til Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="89b9d-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="89b9d-118">Hurtigstartveiledning for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="89b9d-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="89b9d-119">Last ned Azure Information Protection-klient</span><span class="sxs-lookup"><span data-stu-id="89b9d-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)