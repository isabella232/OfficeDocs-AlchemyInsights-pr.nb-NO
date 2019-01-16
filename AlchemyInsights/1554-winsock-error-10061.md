---
title: 1554 Winsock-feil 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28302809"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="5dca3-102">Winsock-feil 10061</span><span class="sxs-lookup"><span data-stu-id="5dca3-102">Winsock error 10061</span></span>

<span data-ttu-id="5dca3-p101">Denne koden betyr at Office 365 ikke kan opprette en TCP socket (tilkobling) med verten. Den mest sannsynlige årsaken til denne feilen er et problem med brannmurkonfigurasjonen. Hvis du vil løse problemet, kontrollerer du disse innstillingene:</span><span class="sxs-lookup"><span data-stu-id="5dca3-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="5dca3-106">Kontroller konfigurasjonen av brannmur med informasjonen i [Office 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="5dca3-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="5dca3-107">Hvis feilen, er spesifikk for Exchange Online Protection (EOP), bør du har blitt tidligere melding til en endring i [Exchange Online beskyttelse IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5dca3-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="5dca3-108">Kontroller at Internett-leverandøren (ISP) ikke blokkerer porten.</span><span class="sxs-lookup"><span data-stu-id="5dca3-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="5dca3-109">Kontroller smart verts- og serverinnstillingene i koblingene.</span><span class="sxs-lookup"><span data-stu-id="5dca3-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="5dca3-110">Legg merke til at Office 365 ikke blokkerer *innkommende* tilkoblinger på denne måten.</span><span class="sxs-lookup"><span data-stu-id="5dca3-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

