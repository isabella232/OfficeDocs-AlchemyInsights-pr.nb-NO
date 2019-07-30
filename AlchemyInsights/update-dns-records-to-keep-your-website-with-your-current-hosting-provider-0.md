---
title: Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e437015d476c1417fa37e1b1c250e2205e9ce4d9
ms.sourcegitcommit: b825ced7b66d452b0f3874a57e033e690ec41c93
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/29/2019
ms.locfileid: "35925294"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="7b739-102">Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert</span><span class="sxs-lookup"><span data-stu-id="7b739-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="7b739-103">Velg domenet du bruker for webområdet ditt i listen over domener, på [domener](https://portal.office.com/adminportal/home#/Domains) -siden.</span><span class="sxs-lookup"><span data-stu-id="7b739-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="7b739-104">Velg **+ Ny egendefinert post** og angi følgende:</span><span class="sxs-lookup"><span data-stu-id="7b739-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="7b739-105">Angi **A (Adresse)** for **DNS-type**</span><span class="sxs-lookup"><span data-stu-id="7b739-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="7b739-106">**Vertsnavn eller et Alias**, skriver du inn følgende:**@**</span><span class="sxs-lookup"><span data-stu-id="7b739-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="7b739-107">Skriv inn den statiske IP-adressen for nettstedet ditt der den driftes for øyeblikket (for eksempel: 172.16.140.1), for **IP-adresse**</span><span class="sxs-lookup"><span data-stu-id="7b739-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="7b739-p101">Dette må være en  *statisk*  IP-adresse for nettstedet, ikke en  *dynamisk*  IP-adresse. Undersøk området der nettstedet driftes for å være sikker på at du kan få en statisk IP-adresse for det offentlige nettstedet.</span><span class="sxs-lookup"><span data-stu-id="7b739-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="7b739-110">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="7b739-110">Select **Save**.</span></span>

<span data-ttu-id="7b739-111">Du kan i tillegg opprette en CNAME-post som lar kundene finne nettstedet.</span><span class="sxs-lookup"><span data-stu-id="7b739-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="7b739-112">Velg **+ Ny egendefinert post** og angi følgende:</span><span class="sxs-lookup"><span data-stu-id="7b739-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="7b739-113">Angi **CNAME (Alias)** for **DNS-type**</span><span class="sxs-lookup"><span data-stu-id="7b739-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="7b739-114">Skriv inn **www** for **Vertsnavn eller alias**</span><span class="sxs-lookup"><span data-stu-id="7b739-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="7b739-115">Skriv inn det fullt kvalifiserte domenenavnet (FQDN) for nettstedet for **Peker til adresse** (for eksempel: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7b739-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="7b739-116">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="7b739-116">Select **Save**.</span></span>
