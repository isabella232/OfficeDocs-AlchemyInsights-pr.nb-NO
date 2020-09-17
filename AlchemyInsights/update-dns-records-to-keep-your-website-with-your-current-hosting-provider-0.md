---
title: Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815794"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="97214-102">Oppdater DNS-poster for å beholde nettstedet hos gjeldende vert</span><span class="sxs-lookup"><span data-stu-id="97214-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="97214-103">Gå til siden **Konfigurer**domener i administrasjons senteret for Microsoft 365,  >  [Domains](https://admin.microsoft.com/Adminportal#/Domains) og velg domenet du bruker for nettstedet, i listen over domener.</span><span class="sxs-lookup"><span data-stu-id="97214-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="97214-104">Velg **+ Ny egendefinert post** og angi følgende:</span><span class="sxs-lookup"><span data-stu-id="97214-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="97214-105">Angi **A (Adresse)** for **DNS-type**</span><span class="sxs-lookup"><span data-stu-id="97214-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="97214-106">Skriv inn følgende for **verts navn eller alias**: **@**</span><span class="sxs-lookup"><span data-stu-id="97214-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="97214-107">Skriv inn den statiske IP-adressen for nettstedet ditt der den driftes for øyeblikket (for eksempel: 172.16.140.1), for **IP-adresse**</span><span class="sxs-lookup"><span data-stu-id="97214-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="97214-p101">Dette må være en  *statisk*  IP-adresse for nettstedet, ikke en  *dynamisk*  IP-adresse. Undersøk området der nettstedet driftes for å være sikker på at du kan få en statisk IP-adresse for det offentlige nettstedet.</span><span class="sxs-lookup"><span data-stu-id="97214-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="97214-110">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="97214-110">Select **Save**.</span></span>

<span data-ttu-id="97214-111">Du kan i tillegg opprette en CNAME-post som lar kundene finne nettstedet.</span><span class="sxs-lookup"><span data-stu-id="97214-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="97214-112">Velg **+ Ny egendefinert post** og angi følgende:</span><span class="sxs-lookup"><span data-stu-id="97214-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="97214-113">Angi **CNAME (Alias)** for **DNS-type**</span><span class="sxs-lookup"><span data-stu-id="97214-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="97214-114">Skriv inn **www** for **Vertsnavn eller alias**</span><span class="sxs-lookup"><span data-stu-id="97214-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="97214-115">Skriv inn det fullt kvalifiserte domenenavnet (FQDN) for nettstedet for **Peker til adresse** (for eksempel: contoso.com).</span><span class="sxs-lookup"><span data-stu-id="97214-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="97214-116">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="97214-116">Select **Save**.</span></span>
