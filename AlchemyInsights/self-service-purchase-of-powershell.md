---
title: Selv betjent kjøp av PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739979"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="d3cb2-102">Selv betjent kjøp av PowerShell</span><span class="sxs-lookup"><span data-stu-id="d3cb2-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="d3cb2-103">Hvis du vil bruke MSCommerce PowerShell-modulen, må du installere den på en Windows 10-enhet med TLS 1,2 (krever lokale administrator tillatelser).</span><span class="sxs-lookup"><span data-stu-id="d3cb2-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="d3cb2-104">Importer og koble til MSCommerce-modulen.</span><span class="sxs-lookup"><span data-stu-id="d3cb2-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="d3cb2-105">Når du blir bedt om å logge på, må du bruke rolle legitimasjonen global eller fakturering for administratorer.</span><span class="sxs-lookup"><span data-stu-id="d3cb2-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="d3cb2-106">Hvis du ikke har TLS 1,2, kan du få følgende feil melding når du prøver å hente eller oppdatere policyen:</span><span class="sxs-lookup"><span data-stu-id="d3cb2-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="d3cb2-107">*ErrorMessage – den underliggende tilkoblingen ble lukket: Det oppstod en uventet feil under sendingen*.</span><span class="sxs-lookup"><span data-stu-id="d3cb2-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



