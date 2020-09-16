---
title: Overføring fra det administrative alternativet til MIP/Unified-merking i Samsvars senteret
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674335"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="9d68e-102">Overføring fra det administrative alternativet til MIP/Unified-merking i Samsvars senteret</span><span class="sxs-lookup"><span data-stu-id="9d68e-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="9d68e-103">Hvis du vil overføre fra brukerførte etiketter til enhetlig merking i sikkerhets-og Samsvars senteret, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="9d68e-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="9d68e-104">**Aktivere beskyttelse fra Azure-portalen**</span><span class="sxs-lookup"><span data-stu-id="9d68e-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="9d68e-105">Hvis du ikke allerede har gjort det, åpner du et nytt nett leser vindu og [logger deg på Azure-portalen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="9d68e-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="9d68e-106">Gå til blad for **Azure Information Protection** .</span><span class="sxs-lookup"><span data-stu-id="9d68e-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="9d68e-107">Klikk for eksempel **alle tjenester** på hub-menyen, og begynn å skrive inn **informasjon** i Filter-boksen.</span><span class="sxs-lookup"><span data-stu-id="9d68e-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="9d68e-108">Velg **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="9d68e-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="9d68e-109">Hvis du ikke har brukt Azure Information Protection blad før, kan du se [ytterligere trinn](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) for å legge til dette Bladt i portalen.</span><span class="sxs-lookup"><span data-stu-id="9d68e-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="9d68e-110">Hvis du vil åpne blad for Azure Information Protection, må du ha enten en [Azure Information Protection Premium-plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller en Office 365-plan som inkluderer rettighets administrasjon.</span><span class="sxs-lookup"><span data-stu-id="9d68e-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="9d68e-111">Hvis du har et av disse abonnementene, men ser en melding om at et gyldig abonnement ikke blir funnet, kan du [kontakte Microsoft kunde støtte](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller bruke standard støtte kanaler.</span><span class="sxs-lookup"><span data-stu-id="9d68e-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="9d68e-112">Finn alternativer for **Administrer** -menyen, og velg deretter **beskyttelses aktivering**.</span><span class="sxs-lookup"><span data-stu-id="9d68e-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="9d68e-113">Klikk **Aktiver**, og bekreft deretter handlingen.</span><span class="sxs-lookup"><span data-stu-id="9d68e-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="9d68e-114">Når aktiveringen er fullført, viser informasjons linjen **aktivering**er fullført.</span><span class="sxs-lookup"><span data-stu-id="9d68e-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="9d68e-115">**Overføre etiketter for Azure Information Protection til Office 365 sikkerhets & Samsvars senter**</span><span class="sxs-lookup"><span data-stu-id="9d68e-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="9d68e-116">Kontroller at du er logget på som bruker med global administrator tillatelse.</span><span class="sxs-lookup"><span data-stu-id="9d68e-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="9d68e-117">Gå til blad for **Azure Information Protection** .</span><span class="sxs-lookup"><span data-stu-id="9d68e-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="9d68e-118">Velg **Unified labelion**på **Manage** Menu-alternativet.</span><span class="sxs-lookup"><span data-stu-id="9d68e-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="9d68e-119">Klikk **Aktiver** i det elektroniske utvelgings blad for **Azure Information Protection** , og følg instruksjonene.</span><span class="sxs-lookup"><span data-stu-id="9d68e-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="9d68e-120">**Obs**! Kontroller at du har de nødvendige tillatelsene før du aktiverer sikkerhets & av samsvars senteret.</span><span class="sxs-lookup"><span data-stu-id="9d68e-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="9d68e-121">Se disse artiklene for mer informasjon:</span><span class="sxs-lookup"><span data-stu-id="9d68e-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="9d68e-122">Trenger du å være en global administrator for å konfigurere Azure Information Protection, eller kan jeg delegere til andre administratorer?</span><span class="sxs-lookup"><span data-stu-id="9d68e-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="9d68e-123">Viktig informasjon om administrative roller etter overgangen til sikkerhets & Samsvars senter.</span><span class="sxs-lookup"><span data-stu-id="9d68e-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="9d68e-124">Hvis du vil ha mer informasjon om overføring av sikkerhets-og Samsvars senteret for det administrative alternativet, kan du se [overføre etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="9d68e-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
