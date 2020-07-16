---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148308"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="c08a5-102">Om identitet i Yammer</span><span class="sxs-lookup"><span data-stu-id="c08a5-102">About identity in Yammer</span></span>

<span data-ttu-id="c08a5-103">Det anbefales at alle nettverk tar følgende trinn for å unngå identitetsrelaterte problemer:</span><span class="sxs-lookup"><span data-stu-id="c08a5-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="c08a5-104">Fremtving Office 365-identitet etter klargjøring av Microsoft 365-kontoer for brukere i Azure AD for å sikre at alle brukere logger på ved hjelp av sin primære Microsoft 365-konto.</span><span class="sxs-lookup"><span data-stu-id="c08a5-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="c08a5-105">Hvis du vil ha mer informasjon, kan du se [Fremtving Office 365-identitet for Yammer-brukere](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="c08a5-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="c08a5-106">Konsolidere flere Yammer-nettverk.</span><span class="sxs-lookup"><span data-stu-id="c08a5-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="c08a5-107">Eldre Yammer-konfigurasjoner tillater at flere Yammer-nettverk er koblet til én leier.</span><span class="sxs-lookup"><span data-stu-id="c08a5-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="c08a5-108">Hvis du vil ha mer informasjon, kan du se [Nettverksoverføring – Konsolidere flere Yammer-nettverk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="c08a5-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="c08a5-109">Du kan eventuelt fremtvinge lisensiering for Yammer for å blokkere brukere fra Yammer hvis de ikke har en lisens.</span><span class="sxs-lookup"><span data-stu-id="c08a5-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="c08a5-110">Hvis du vil ha mer informasjon, kan du se [Administrere Yammer-brukerlisenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="c08a5-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="c08a5-111">Til slutt kan du overvåke brukerlisten for eldre Yammer-nettverk og suspendere eldre brukere.</span><span class="sxs-lookup"><span data-stu-id="c08a5-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="c08a5-112">Det anbefales at du suspenderer (deaktiverer) brukere i stedet for å slette dem, fordi sletting er irreversibel.</span><span class="sxs-lookup"><span data-stu-id="c08a5-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="c08a5-113">Hvis du vil ha mer informasjon, kan du se [Overvåke Yammer-brukere i nettverk som er koblet til Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) og [Fjerne brukere](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="c08a5-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="c08a5-114">Ved å konfigurere Yammer ved hjelp av disse trinnene, er du også klar til å konfigurere Yammer-nettverket for opprinnelig modus for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c08a5-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="c08a5-115">Hvis du vil ha mer informasjon, kan du se [Konfigurere Yammer-nettverket for opprinnelig modus for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="c08a5-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>