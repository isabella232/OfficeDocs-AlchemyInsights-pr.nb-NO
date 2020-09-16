---
title: Ytelses problemer – SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771253"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="aa6d2-102">SharePoint eller OneDrive langsomt, utilgjengelig eller ikke tilgjengelig for flere brukere</span><span class="sxs-lookup"><span data-stu-id="aa6d2-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="aa6d2-103">Hvis et OneDrive-eller SharePoint-nettsted ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjeneste problem.</span><span class="sxs-lookup"><span data-stu-id="aa6d2-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="aa6d2-104">[Kontroller instrument bordet for tjeneste tilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="aa6d2-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="aa6d2-105">**Legge til og lisensiere brukeren**</span><span class="sxs-lookup"><span data-stu-id="aa6d2-105">**Add and license the user**</span></span>

<span data-ttu-id="aa6d2-106">Sikre at du [tilordner lisenser til brukere i Microsoft 365 for bedrifter](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="aa6d2-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="aa6d2-107">**Tilordne tillatelser**</span><span class="sxs-lookup"><span data-stu-id="aa6d2-107">**Assign Permissions**</span></span>

<span data-ttu-id="aa6d2-108">Hvis brukeren er tilordnet en SharePoint-lisens og likevel mottar meldingen ingen tilgang, må du forsikre deg om at de har det [riktige tilgangs nivået](https://docs.microsoft.com/sharepoint/understanding-permission-levels) som er tilordnet.</span><span class="sxs-lookup"><span data-stu-id="aa6d2-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="aa6d2-109">**Vurder å bruke funksjonen for tilgangs forespørsel**</span><span class="sxs-lookup"><span data-stu-id="aa6d2-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="aa6d2-110">Med [tilgangs forespørsels funksjonen](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) kan personer be om tilgang til innhold som de ikke har tillatelse til å se.</span><span class="sxs-lookup"><span data-stu-id="aa6d2-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="aa6d2-111">**Tillat egen definert skript kan føre til problemer som nektes tilgang**</span><span class="sxs-lookup"><span data-stu-id="aa6d2-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="aa6d2-112">Det finnes visse scenarioer der funksjonen *Tillat egen definerte skript* kanskje presenterer en tilgang nektet.</span><span class="sxs-lookup"><span data-stu-id="aa6d2-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="aa6d2-113">For en liste over funksjoner som påvirkes, sikkerhets hensyn og muligheten til å deaktivere funksjonen.</span><span class="sxs-lookup"><span data-stu-id="aa6d2-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="aa6d2-114">Gå til [tillate eller ikke Tillat egen definert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="aa6d2-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

