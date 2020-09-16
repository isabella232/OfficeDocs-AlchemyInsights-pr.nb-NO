---
title: Opprette regler for INSTALLASJONs etikett
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732184"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="7ffcf-102">Opprette regler for INSTALLASJONs etikett</span><span class="sxs-lookup"><span data-stu-id="7ffcf-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="7ffcf-103">Azure Information Protection-etiketter kan brukes med hele data området som en organisasjon vanligvis oppretter og lagrer, fra den laveste klassifiseringen av personlige data, til den høyeste klassifiseringen av svært konfidensielle data.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="7ffcf-104">Policyer for Azure Information Protection gjelder for Classic-klienten (Azure Information Protection), og ikke den informative,  [enhetlige etikett klienten](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="7ffcf-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="7ffcf-105">Du kan konfigurere flere elementer i en policy for en administrator, inkludert alternativer som:</span><span class="sxs-lookup"><span data-stu-id="7ffcf-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="7ffcf-106">Alternativ for hvilken etikett vil la administratorer eller bruker klassifisering og beskyttelse (valg fritt) dokumenter og e-postmeldinger</span><span class="sxs-lookup"><span data-stu-id="7ffcf-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="7ffcf-107">Alternativ for å fremtvinge klassifisering når brukere lagrer dokumenter og sender e-post</span><span class="sxs-lookup"><span data-stu-id="7ffcf-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="7ffcf-108">Alternativ for å automatisk merke en e-postmelding, basert på vedleggene.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="7ffcf-109">Alternativ for å kontrollere om informasjons beskyttelses feltet vises i Office-programmer</span><span class="sxs-lookup"><span data-stu-id="7ffcf-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="7ffcf-110">Hvis du vil ha flere alternativer og informasjon om policyer for Azure Information Protection, kan du se: [Oversikt over policyen for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="7ffcf-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="7ffcf-111">Hvis du vil ha andre nyttige ressurser vedrørende policyer for å gjøre det.</span><span class="sxs-lookup"><span data-stu-id="7ffcf-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="7ffcf-112">Opplæring: konfigurere policy innstillinger for Azure Information Protection og opprette en ny etikett</span><span class="sxs-lookup"><span data-stu-id="7ffcf-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="7ffcf-113">Konfigurere policyen for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7ffcf-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="7ffcf-114">Opprette og konfigurere følsomme etiketter og deres policyer</span><span class="sxs-lookup"><span data-stu-id="7ffcf-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="7ffcf-115">Veiledninger for vanlige scenarier som bruker Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7ffcf-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="7ffcf-116">Gå gjennom dokumentasjon for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7ffcf-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="7ffcf-117">Krav for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7ffcf-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="7ffcf-118">Hurtigst Art opplæring for Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7ffcf-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="7ffcf-119">Last ned Azure Information Protection-klienten</span><span class="sxs-lookup"><span data-stu-id="7ffcf-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)