---
title: Diskforsendelse i Microsoft 365 importtjenesten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731654"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="20c5e-102">Diskforsendelse i Microsoft 365 importtjenesten</span><span class="sxs-lookup"><span data-stu-id="20c5e-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="20c5e-103">Bruk Diskforsendelse ved å kopiere PSTer til en harddisk og deretter sende harddisken til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20c5e-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="20c5e-104">Slik starter du jobben:</span><span class="sxs-lookup"><span data-stu-id="20c5e-104">To start the job:</span></span>

1. <span data-ttu-id="20c5e-105">Velg Importer Microsoft 365 i **samsvarssenteret** for informasjon under **Informasjonsstyring**.</span><span class="sxs-lookup"><span data-stu-id="20c5e-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="20c5e-106">Velg **Velg importjobbtype**, og velg deretter **Neste**.</span><span class="sxs-lookup"><span data-stu-id="20c5e-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="20c5e-107">Hvis du vil se trinnene for dette importalternativet, velger du **Lever harddisker til en av våre fysiske plasseringer**.</span><span class="sxs-lookup"><span data-stu-id="20c5e-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="20c5e-108">Her er noen ting du må huske på:</span><span class="sxs-lookup"><span data-stu-id="20c5e-108">Here are some things to remember:</span></span>

- <span data-ttu-id="20c5e-109">Du må være tilordnet rollen Importer postboks i Exchange Online importere PST-filer til Microsoft 365 postbokser.</span><span class="sxs-lookup"><span data-stu-id="20c5e-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="20c5e-110">Ytelsen kan påvirkes for PST-er som er større enn 20 GB.</span><span class="sxs-lookup"><span data-stu-id="20c5e-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="20c5e-111">Bare 2,5-tommers SSD-er (solid state drives) eller 2,5-tommers eller 3,5-tommers SATA II/III interne harddisker støttes.</span><span class="sxs-lookup"><span data-stu-id="20c5e-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="20c5e-112">Harddisken som inneholder PST-filer, må krypteres med BitLocker.</span><span class="sxs-lookup"><span data-stu-id="20c5e-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="20c5e-113">Kostnaden for å importere PST-filer til Microsoft 365 postbokser ved hjelp av stasjonsforsendelse er USD 2 per GB med data.</span><span class="sxs-lookup"><span data-stu-id="20c5e-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="20c5e-114">Hvis du vil ha mer informasjon om hvordan du bruker diskforsendelsesmetoden for import av PSTer, kan du se Bruke stasjonsforsendelse til [å importere organisasjonens PST-filer](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span><span class="sxs-lookup"><span data-stu-id="20c5e-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>