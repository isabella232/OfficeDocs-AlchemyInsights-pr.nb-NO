---
title: Oppdatere navneserveren til å peke til Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734920"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="1fa4c-102">Oppdatere navneserveren til å peke til Microsoft</span><span class="sxs-lookup"><span data-stu-id="1fa4c-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="1fa4c-103">Obs! Noen ganger kan det ta opptil 48 timer før endringer i navneserverne overføres.</span><span class="sxs-lookup"><span data-stu-id="1fa4c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="1fa4c-104">Hvis du vil konfigurere domenet med Microsoft, må du oppdatere navneservere hos registra ren.</span><span class="sxs-lookup"><span data-stu-id="1fa4c-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="1fa4c-105">Opprette eller redigere navneserverpostene hos domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="1fa4c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="1fa4c-106">Gå til domeneregistratorens nettsted og finn området der du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="1fa4c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="1fa4c-107">Opprett eller rediger to navneserverposter slik at de samsvarer med disse verdiene:</span><span class="sxs-lookup"><span data-stu-id="1fa4c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="1fa4c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1fa4c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="1fa4c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1fa4c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="1fa4c-110">Lagre endringer.</span><span class="sxs-lookup"><span data-stu-id="1fa4c-110">Save changes.</span></span>

<span data-ttu-id="1fa4c-111">Du kan også finne detaljerte instruksjoner i denne artikkelen: [endre navneservere for å konfigurere Microsoft 365 med alle domene registre ring](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="1fa4c-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  