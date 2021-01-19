---
title: Feilsøke eier problemer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901283"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="2f522-102">Feilsøke eier problemer</span><span class="sxs-lookup"><span data-stu-id="2f522-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="2f522-103">Hvis du vil feilsøke eier relaterte problemer, utfører du følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="2f522-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="2f522-104">[Legge til eller endre Azure-abonnements administratorer](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory-grupper (Azure ad) som eies og administreres av gruppe eiere.</span><span class="sxs-lookup"><span data-stu-id="2f522-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="2f522-105">Gruppe eiere kan være brukere eller tjeneste sikkerhetskontohavere, og de kan administrere gruppen, inkludert medlemskap.</span><span class="sxs-lookup"><span data-stu-id="2f522-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="2f522-106">Bare eksisterende gruppe eiere eller gruppe administrasjons administratorer kan tilordne gruppe eiere.</span><span class="sxs-lookup"><span data-stu-id="2f522-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="2f522-107">Gruppe eiere må ikke være medlemmer av gruppen.</span><span class="sxs-lookup"><span data-stu-id="2f522-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="2f522-108">[Legg til eller endre Azure-abonnements administratorer](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): denne artikkelen beskriver hvordan du legger til eller endrer Administrator rollen for en bruker ved hjelp av Azure RBAC i abonnements området.</span><span class="sxs-lookup"><span data-stu-id="2f522-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="2f522-109">Bruk PowerShell til å legge til en gruppe eier eller en program eier.</span><span class="sxs-lookup"><span data-stu-id="2f522-109">Use PowerShell to add a group owner or an application owner.</span></span>
