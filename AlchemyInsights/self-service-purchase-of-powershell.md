---
title: Selvbetjent kjøp av PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797730"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="7a5e0-102">Selvbetjent kjøp av PowerShell</span><span class="sxs-lookup"><span data-stu-id="7a5e0-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="7a5e0-103">Hvis du vil bruke MSCommerce PowerShell-modulen, må du installere den på en Windows 10-enhet med TLS 1.2 (lokale administratortillatelser kreves).</span><span class="sxs-lookup"><span data-stu-id="7a5e0-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="7a5e0-104">Importer og koble til MSCommerce-modulen.</span><span class="sxs-lookup"><span data-stu-id="7a5e0-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="7a5e0-105">Når du blir bedt om å logge på, må du bruke rollen Global eller Faktureringsadministrator.</span><span class="sxs-lookup"><span data-stu-id="7a5e0-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="7a5e0-106">Hvis du ikke har TLS 1.2, kan du få følgende feilmelding når du prøver å hente eller oppdatere policyen:</span><span class="sxs-lookup"><span data-stu-id="7a5e0-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="7a5e0-107">*ErrorMessage -Den underliggende tilkoblingen ble lukket: Det oppstod* en uventet feil under sending.</span><span class="sxs-lookup"><span data-stu-id="7a5e0-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



