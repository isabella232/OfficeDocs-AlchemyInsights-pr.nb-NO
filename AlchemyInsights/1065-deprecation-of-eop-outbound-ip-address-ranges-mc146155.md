---
title: 1065 nedgraderingen EOP utgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482030"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="2557c-102">Nedgraderingen av EOP utgående IP-adresseområder</span><span class="sxs-lookup"><span data-stu-id="2557c-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="2557c-p101">Vi har oppdaget et mulig problem med organisasjonen som (Hvis ikke korrigert av oktober 26th, 2018) kan bryte e-postflyt til lokale eller eksterne mål. Som tidligere formidlet for å forenkle behandling av IP-adressen området konsoliderer vi Exchange Online Protection (EOP) IP-adresseområder som brukes til å sende og motta e-post utenfor Office 365. Vår analyse viser at ett eller flere av e-post for eksterne kilder eller mål du har konfigurert i e-post flyt koblinger ikke godtar tilkoblinger fra de IP-adresse områdene vist [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="2557c-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="2557c-106">Utføre en handling før oktober 26th å sikre disse kilder og mål skal godta tilkoblinger til og fra alle [publiserte EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="2557c-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="2557c-107">Hvis du vil ha mer informasjon om denne endringen, kan du se Meldingssentral innlegg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="2557c-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="2557c-p102">**Merk**: Hvis du tidligere brukte URL-adresse eller IP-publisering via HTML, XML og RSS-oppdateringer for sluttpunktet, også bør du oppdatere til de nye web-tjenestene for å automatisere disse typene oppdateringer. Hvis du vil ha mer informasjon, kan du se [Office 365 endepunktet kategorier og Office 365-IP-adresse og URL-adressen for webtjenesten](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="2557c-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

