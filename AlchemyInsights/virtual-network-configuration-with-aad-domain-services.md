---
title: Virtuell konfigurasjon med AAD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885644"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="6d5ef-102">Virtuell konfigurasjon med AAD Domain Services</span><span class="sxs-lookup"><span data-stu-id="6d5ef-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="6d5ef-103">Virtuell konfigurasjon med AAD Domain Services omfatter følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="6d5ef-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="6d5ef-104">Kontrollere domenets tilstand på Azure-portalen https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="6d5ef-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="6d5ef-105">Kontrollere NSG for regler som blokkerer porter som er nødvendige for å synkronisere i Azure AD Domain Services på portalen https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="6d5ef-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="6d5ef-106">Sørge for at det virtuelle nettverket er distribuert i samme Azure-område som Azure AD Domain Services-administrert domene.</span><span class="sxs-lookup"><span data-stu-id="6d5ef-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="6d5ef-107">Sikre at du ikke har et eksisterende domene med samme domene navn som er tilgjengelig på det virtuelle nettverket.</span><span class="sxs-lookup"><span data-stu-id="6d5ef-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="6d5ef-108">Hvis du vil ha mer informasjon om utformings hensyn for Azure virtuelt nettverk for å støtte AAD Domain Services, kan du se [virtuelt nettverks vurdering](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="6d5ef-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

