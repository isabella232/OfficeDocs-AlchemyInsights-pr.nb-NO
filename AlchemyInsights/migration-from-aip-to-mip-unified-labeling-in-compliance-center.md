---
title: Overføring fra AIP til MIP/Unified Labeling i samsvarssenteret
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
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825380"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="b3e2b-102">Overføring fra AIP til MIP/Unified Labeling i samsvarssenteret</span><span class="sxs-lookup"><span data-stu-id="b3e2b-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="b3e2b-103">Hvis du vil overføre fra AIP-etiketter til Enhetlig merking i sikkerhets- og samsvarssenteret, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="b3e2b-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="b3e2b-104">**Aktivere beskyttelse fra Azure-portalen**</span><span class="sxs-lookup"><span data-stu-id="b3e2b-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="b3e2b-105">Hvis du ikke allerede har gjort det, åpner du et nytt nettleservindu og [logger på Azure-portalen.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="b3e2b-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="b3e2b-106">Gå til **Azure Information Protection-bladet.**</span><span class="sxs-lookup"><span data-stu-id="b3e2b-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="b3e2b-107">Klikk for eksempel Alle tjenester på hubmenyen, **og** begynn å skrive **inn informasjon** i Filter-boksen.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="b3e2b-108">Velg **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="b3e2b-109">Hvis du ikke har tilgang til Azure Information Protection-bladet før, kan du se engangstrinnene for å legge til dette bladet i portalen. [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)</span><span class="sxs-lookup"><span data-stu-id="b3e2b-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="b3e2b-110">Hvis du vil åpne Azure Information Protection-bladet, må du enten ha et [Azure Information Protection Premium-abonnement](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller et Office 365-abonnement som inkluderer Rights Management.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="b3e2b-111">Hvis du har et av disse abonnementene, men ser en melding om at et gyldig abonnement ikke finnes, kan du kontakte [Microsoft Kundestøtte](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller bruke standard støttekanaler.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="b3e2b-112">Finn **alternativene for** Administrer meny, og velg **Beskyttelsesaktivering**.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="b3e2b-113">Klikk **Aktiver**, og bekreft deretter handlingen.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="b3e2b-114">Når aktiveringen er fullført, viser informasjonslinjen **aktiveringen fullført.**</span><span class="sxs-lookup"><span data-stu-id="b3e2b-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="b3e2b-115">**Overføre Azure Information Protection-etiketter til Sikkerhets- & i Office 365**</span><span class="sxs-lookup"><span data-stu-id="b3e2b-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="b3e2b-116">Kontroller at du er logget på som en bruker med global administratortillatelse.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="b3e2b-117">Gå til **Azure Information Protection-bladet.**</span><span class="sxs-lookup"><span data-stu-id="b3e2b-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="b3e2b-118">Velg **Enhetlig** merking fra **behandle-menyalternativet.**</span><span class="sxs-lookup"><span data-stu-id="b3e2b-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="b3e2b-119">Klikk **Aktiver på Azure Information Protection – Unified labeling** **bladet,** og følg instruksjonene på nettet.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="b3e2b-120">**Obs!** Kontroller at du har de riktige tillatelsene før du aktiverer overføringen av sikkerhets- & samsvarssenteret.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="b3e2b-121">Se disse artiklene for mer informasjon:</span><span class="sxs-lookup"><span data-stu-id="b3e2b-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="b3e2b-122">Må du være global administrator for å konfigurere Azure Information Protection, eller kan jeg delegere til andre administratorer?</span><span class="sxs-lookup"><span data-stu-id="b3e2b-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="b3e2b-123">Viktig informasjon om administrative roller etter overføring til sikkerhets- & samsvarssenteret.</span><span class="sxs-lookup"><span data-stu-id="b3e2b-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="b3e2b-124">Hvis du vil ha mer informasjon om AIP til Unified Labeling-overføring til sikkerhets- og samsvarssenteret, kan du se [Overføre etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="b3e2b-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
