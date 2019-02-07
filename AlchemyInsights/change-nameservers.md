---
title: Endre NameServers
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 61c4c5e43a247679bf18fd3861dd98fbe9a7b3eb
ms.sourcegitcommit: 5dee2fcb492bd922092a6de8045a95febe57b97e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/06/2019
ms.locfileid: "29758713"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="70b9d-102">Oppdatere navneserverne for domenet til Office 365</span><span class="sxs-lookup"><span data-stu-id="70b9d-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="70b9d-103">Merk: Nameserver endringer kan ta opptil 48 timer å overføre.</span><span class="sxs-lookup"><span data-stu-id="70b9d-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="70b9d-p101">Navneserverne hos registratoren må oppdateres hvis du skal konfigurere domenet i Office 365. Opprette eller redigere navneserverpostene hos domeneregistratoren.</span><span class="sxs-lookup"><span data-stu-id="70b9d-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="70b9d-106">Gå til domeneregistratorens nettsted og finn området der du kan redigere navneserverne.</span><span class="sxs-lookup"><span data-stu-id="70b9d-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="70b9d-107">Opprett eller rediger to navneserverposter slik at de samsvarer med disse verdiene:</span><span class="sxs-lookup"><span data-stu-id="70b9d-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="70b9d-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="70b9d-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="70b9d-109">ns2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="70b9d-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="70b9d-110">Lagre endringer.</span><span class="sxs-lookup"><span data-stu-id="70b9d-110">Save changes.</span></span>
    
<span data-ttu-id="70b9d-111">Du kan også finne detaljerte instruksjoner i denne artikkelen: [Endre navneservere for å konfigurere Office 365 med alle domeneregistratorer](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="70b9d-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

