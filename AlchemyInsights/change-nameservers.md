---
title: Endre navneservere
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508097"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="297df-102">Oppdatere navneserveren til å peke til Microsoft</span><span class="sxs-lookup"><span data-stu-id="297df-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="297df-103">Obs! Noen ganger kan det ta opptil 48 timer før endringer i navneserverne overføres.</span><span class="sxs-lookup"><span data-stu-id="297df-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="297df-p101">For å konfigurere domenet i Microsoft 365 må navneserverne hos domeneregistratoren oppdateres. Opprette eller redigere navneserverpostene hos domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="297df-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="297df-106">Gå til domeneregistratorens nettsted og finn området der du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="297df-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="297df-107">Opprett eller rediger to navneserverposter slik at de samsvarer med disse verdiene:</span><span class="sxs-lookup"><span data-stu-id="297df-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="297df-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="297df-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="297df-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="297df-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="297df-110">Lagre endringer.</span><span class="sxs-lookup"><span data-stu-id="297df-110">Save changes.</span></span>

<span data-ttu-id="297df-111">Du kan også finne detaljerte instruksjoner i denne artikkelen: [Endre navneservere hos domeneregistratorer](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="297df-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  