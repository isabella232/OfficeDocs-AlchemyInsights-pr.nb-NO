---
title: Problem med sikkerhetsgrupper
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177628"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="c4283-102">Problem med sikkerhetsgrupper</span><span class="sxs-lookup"><span data-stu-id="c4283-102">Issue with security groups</span></span>

<span data-ttu-id="c4283-103">**Hvis du får nettverksfeil AADDS104**</span><span class="sxs-lookup"><span data-stu-id="c4283-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="c4283-104">Ugyldige grupperegler for nettverkssikkerhet er den vanligste årsaken til nettverksfeil for Azure Active Directory Domain Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="c4283-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="c4283-105">Sikkerhetsgruppen for nettverket for det virtuelle nettverket må tillate tilgang til bestemte porter og protokoller.</span><span class="sxs-lookup"><span data-stu-id="c4283-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="c4283-106">Hvis disse portene er blokkert, kan ikke Azure-plattformen overvåke eller oppdatere det administrerte domenet.</span><span class="sxs-lookup"><span data-stu-id="c4283-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="c4283-107">Synkroniseringen mellom Azure AD og Azure AD DS påvirkes også.</span><span class="sxs-lookup"><span data-stu-id="c4283-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="c4283-108">Sørg for at standardportene er åpne for å unngå avbrudd i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="c4283-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="c4283-109">Hvis du vil forstå og løse vanlige varsler om konfigurasjonsproblemer for nettverkssikkerhetsgrupper, kan du se [Legge til og bekrefte sikkerhetsgrupper.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="c4283-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
