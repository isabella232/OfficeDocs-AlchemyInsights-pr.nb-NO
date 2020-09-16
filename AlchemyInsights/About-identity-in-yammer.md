---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664179"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="0125a-102">Om identitet i Yammer</span><span class="sxs-lookup"><span data-stu-id="0125a-102">About identity in Yammer</span></span>

<span data-ttu-id="0125a-103">Det anbefales at alle nettverk utfører følgende trinn for å unngå identitets relaterte problemer:</span><span class="sxs-lookup"><span data-stu-id="0125a-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="0125a-104">Tving Office 365-identitet etter klar gjøring av Microsoft 365-kontoer for brukere i Azure AD for å sikre at alle brukere logger på ved hjelp av den primære Microsoft 365-kontoen.</span><span class="sxs-lookup"><span data-stu-id="0125a-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="0125a-105">Hvis du vil ha mer informasjon, kan du se [tvinge Office 365-identitet for Yammer-brukere](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="0125a-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="0125a-106">Konsolider flere Yammer-nettverk.</span><span class="sxs-lookup"><span data-stu-id="0125a-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="0125a-107">Eldre Yammer-konfigurasjoner tillater at flere Yammer-nettverk kobles til én Tenant.</span><span class="sxs-lookup"><span data-stu-id="0125a-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="0125a-108">Hvis du vil ha mer informasjon, kan du se [nettverks overføring – Konsolider flere Yammer-nettverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="0125a-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="0125a-109">Du kan også håndheve lisensiering for Yammer for å blokkere brukere fra Yammer hvis de ikke har en lisens.</span><span class="sxs-lookup"><span data-stu-id="0125a-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="0125a-110">Hvis du vil ha mer informasjon, kan du se [administrere bruker lisenser for Yammer i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="0125a-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="0125a-111">Til slutt kan du overvåke bruker listen for eldre Yammer-nettverk og utsette eldre brukere.</span><span class="sxs-lookup"><span data-stu-id="0125a-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="0125a-112">Det anbefales at du deaktiverer (deaktiverer) brukere i stedet for å slette dem, for du kan ikke slette.</span><span class="sxs-lookup"><span data-stu-id="0125a-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="0125a-113">Hvis du vil ha mer informasjon, kan du se [overvåke Yammer-brukere i nettverk som er koblet til Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) og [fjerne brukere](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="0125a-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="0125a-114">Ved å konfigurere Yammer ved hjelp av disse trinnene, er du også klar til å konfigurere Yammer-nettverket for opprinnelig modus for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0125a-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="0125a-115">Hvis du vil ha mer informasjon, kan du se [konfigurere Yammer-nettverket for opprinnelig modus for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="0125a-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>