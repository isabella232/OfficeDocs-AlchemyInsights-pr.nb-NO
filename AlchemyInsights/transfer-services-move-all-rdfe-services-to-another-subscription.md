---
title: Overføre tjenester – flytte alle RDFE-tjenester til et annet abonnement
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692171"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="98de9-102">Overføre tjenester – flytte alle RDFE-tjenester til et annet abonnement</span><span class="sxs-lookup"><span data-stu-id="98de9-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="98de9-103">**Flytte ressurser**</span><span class="sxs-lookup"><span data-stu-id="98de9-103">**Move resources**</span></span>

<span data-ttu-id="98de9-104">Azure-ressurser kan flyttes til enten et annet Azure-abonnement eller en ressurs gruppe under samme abonnement ved hjelp av Azure Portal, Azure PowerShell, Azure CLI eller REST-API-en til å flytte ressurser.</span><span class="sxs-lookup"><span data-stu-id="98de9-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="98de9-105">Før du kan flytte ressurser, kan du se:</span><span class="sxs-lookup"><span data-stu-id="98de9-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="98de9-106">Sjekk liste før du flytter ressurser</span><span class="sxs-lookup"><span data-stu-id="98de9-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="98de9-107">Tjenester som kan flyttes</span><span class="sxs-lookup"><span data-stu-id="98de9-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="98de9-108">Slik validerer du flyttingen</span><span class="sxs-lookup"><span data-stu-id="98de9-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="98de9-109">Flytte veiledning for tjenester</span><span class="sxs-lookup"><span data-stu-id="98de9-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="98de9-110">Hvis du vil flytte eksisterende ressurser til en annen ressurs gruppe eller-abonnement, kan du bruke:</span><span class="sxs-lookup"><span data-stu-id="98de9-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="98de9-111">Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="98de9-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="98de9-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="98de9-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="98de9-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="98de9-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="98de9-114">REST-API</span><span class="sxs-lookup"><span data-stu-id="98de9-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="98de9-115">Opplæring: [flytte Azure-ressurser til andre ressurs grupper eller-abonnementer](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="98de9-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="98de9-116">**Feilsøke feil med Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="98de9-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="98de9-117">Se artiklene nedenfor for å lære om noen vanlige distribusjons feil i Azure, og motta informasjon for å løse dem.</span><span class="sxs-lookup"><span data-stu-id="98de9-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="98de9-118">Hvis du ikke finner feil koden for distribusjons feilen, kan du se [finne feil koden](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="98de9-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="98de9-119">Feilsøke distribusjons feil</span><span class="sxs-lookup"><span data-stu-id="98de9-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="98de9-120">Feilsøke flytting av Azure-ressurser til ny ressurs gruppe eller et abonnement</span><span class="sxs-lookup"><span data-stu-id="98de9-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="98de9-121">Vær oppmerksom på at hvis du vil oppgradere Azure-abonnementet, for eksempel bytte fra gratis til Betal etter hvert, må du konvertere abonnementet.</span><span class="sxs-lookup"><span data-stu-id="98de9-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="98de9-122">Hvis du vil oppgradere en gratis prøve versjon, kan du se [oppgradere gratis prøve versjon eller Microsoft Forestill deg Azure-abonnementet til å betale etter](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)hvert.</span><span class="sxs-lookup"><span data-stu-id="98de9-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="98de9-123">Hvis du vil endre en betal som-a-konto, kan du se [endre abonnementet på Azure Betal-etter-farten til et annet tilbud](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="98de9-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="98de9-124">**Slik legger du til eller knytter et Azure-abonnement til Azure Active Directory-leieren:**</span><span class="sxs-lookup"><span data-stu-id="98de9-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="98de9-125">Logg på, og Velg abonnementet du vil bruke fra abonnementer- [siden i Azure-portalen](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="98de9-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="98de9-126">Velg **endre katalog**.</span><span class="sxs-lookup"><span data-stu-id="98de9-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="98de9-127">Se gjennom eventuelle advarsler som vises, og velg deretter **endre**.</span><span class="sxs-lookup"><span data-stu-id="98de9-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="98de9-128">Katalogen er endret for abonnementet, og du vil få en vellykket melding.</span><span class="sxs-lookup"><span data-stu-id="98de9-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="98de9-129">Bruk *katalog* -bytte ren for å gå til den nye katalogen.</span><span class="sxs-lookup"><span data-stu-id="98de9-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="98de9-130">Det kan ha opptil ti minutter før alt vises på riktig måte.</span><span class="sxs-lookup"><span data-stu-id="98de9-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="98de9-131">**Anbefalte dokumenter**</span><span class="sxs-lookup"><span data-stu-id="98de9-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="98de9-132">Overføre eierskap for et Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="98de9-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="98de9-133">Flytte ressurser til ny ressurs gruppe eller et abonnement</span><span class="sxs-lookup"><span data-stu-id="98de9-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="98de9-134">Behandle ressurser ved hjelp av Azure-portalen</span><span class="sxs-lookup"><span data-stu-id="98de9-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
