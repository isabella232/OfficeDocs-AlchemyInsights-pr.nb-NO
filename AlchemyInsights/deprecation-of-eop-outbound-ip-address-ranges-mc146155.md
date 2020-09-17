---
title: 1065 avskrevet av EOP utgående IP-adresse rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806804"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="0df0f-102">Avskrevet av utgående IP-adresseområder for EOP</span><span class="sxs-lookup"><span data-stu-id="0df0f-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="0df0f-103">Vi har oppdaget et mulig problem med organisasjonen din som (hvis den ikke er rettet opp av oktober 26th, 2018) kan bryte e-postflyten til de lokale eller eksterne stedene.</span><span class="sxs-lookup"><span data-stu-id="0df0f-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="0df0f-104">Som tidligere kommunisert, konsoliderer vi IP-adresseområder for Exchange Online Protection (EOP) som brukes til å sende og motta e-post utenfor Microsoft 365, for å forenkle behandling av IP-adresseområde.</span><span class="sxs-lookup"><span data-stu-id="0df0f-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="0df0f-105">Vår analyse indikerer at én eller flere av de eksterne e-postkildene eller-målene som du har konfigurert i e-postflyt-koblinger, ikke godtar tilkoblinger fra IP-adresseområder som vises [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0df0f-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="0df0f-106">Act før oktober 26th for å sikre at disse kildene og målene vil godta tilkoblinger til og fra alle [PUBLISERTE EoP-IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="0df0f-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="0df0f-107">Hvis du vil ha mer informasjon om denne endringen, kan du se meldings senter inn Legg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="0df0f-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="0df0f-108">**Obs**! hvis du tidligere har brukt IP-eller URL-publisering via HTML, XML og RSS for ende punkt oppdateringer, bør du også overføre til de nye nett tjenestene for automatisering av disse typene oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="0df0f-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="0df0f-109">Hvis du vil ha mer informasjon, kan du se [microsoft 365 Endpoint Categories og microsoft 365 IP Address og URL-webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="0df0f-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
