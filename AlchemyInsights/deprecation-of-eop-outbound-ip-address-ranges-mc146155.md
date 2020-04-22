---
title: 1065 Nedgradering av EOP utgående IP-adresseområderMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704606"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="60b96-102">Nedgradering av EOP utgående IP-adresseområder</span><span class="sxs-lookup"><span data-stu-id="60b96-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="60b96-103">Vi har oppdaget et potensielt problem med organisasjonen din som (hvis ikke korrigert innen 26. oktober 2018) kan bryte e-postflyten til lokale eller eksterne destinasjoner.</span><span class="sxs-lookup"><span data-stu-id="60b96-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="60b96-104">Som tidligere kommunisert, for å forenkle administrasjon av IP-adresseområde, konsoliderer vi IP-adresseområdene Exchange Online Protection (EOP) som brukes til å sende og motta e-post utenfor Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="60b96-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="60b96-105">Vår analyse indikerer at én eller flere av de eksterne e-postkildene eller målene du har konfigurert i e-postflytkoblinger, ikke godtar tilkoblinger fra IP-adresseområdene som vises [her](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="60b96-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="60b96-106">Handle før 26 oktober for å sikre at disse kildene og destinasjonene vil akseptere tilkoblinger til og fra alle [publiserte EOP IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="60b96-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="60b96-107">Hvis du vil ha mer informasjon om denne endringen, kan du se Message Center innlegg [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)eller [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="60b96-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="60b96-108">**Merk:** Hvis du tidligere har brukt IP- eller URL-publisering via HTML-, XML- og RSS-adresse for endepunktoppdateringer, bør du også overføre til de nye webtjenestene for å automatisere denne typen oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="60b96-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="60b96-109">Hvis du vil ha mer informasjon, kan du se [Microsoft 365 endepunktkategorier og Microsoft 365 IP-adresse og URL-webtjeneste](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="60b96-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
