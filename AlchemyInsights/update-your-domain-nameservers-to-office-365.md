---
title: Oppdatere domenenavnserverne slik at de peker til Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720002"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="abc2e-102">Oppdatere domenenavnserverne slik at de peker til Microsoft</span><span class="sxs-lookup"><span data-stu-id="abc2e-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="abc2e-103">Obs! Noen ganger kan det ta opptil 48 timer før endringer i navneserverne overføres.</span><span class="sxs-lookup"><span data-stu-id="abc2e-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="abc2e-104">Hvis du vil konfigurere domenet med Microsoft, må navneserverne hos registraren oppdateres.</span><span class="sxs-lookup"><span data-stu-id="abc2e-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="abc2e-105">Opprette eller redigere navneserverpostene hos domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="abc2e-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="abc2e-106">Gå til domeneregistratorens nettsted og finn området der du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="abc2e-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="abc2e-107">Opprett eller rediger to navneserverposter slik at de samsvarer med disse verdiene:</span><span class="sxs-lookup"><span data-stu-id="abc2e-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="abc2e-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="abc2e-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="abc2e-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="abc2e-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="abc2e-110">Lagre endringer.</span><span class="sxs-lookup"><span data-stu-id="abc2e-110">Save changes.</span></span>

<span data-ttu-id="abc2e-111">Du finner også detaljerte instruksjoner i denne artikkelen: [Endre navneservere for å konfigurere Microsoft 365 med en hvilken som helst domeneregistrator](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="abc2e-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  