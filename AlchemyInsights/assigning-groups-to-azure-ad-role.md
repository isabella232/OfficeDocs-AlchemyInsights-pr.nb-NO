---
title: Tilordne grupper til Azure AD-rollen
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885392"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="6728d-102">Tilordne grupper til Azure AD-rollen</span><span class="sxs-lookup"><span data-stu-id="6728d-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="6728d-103">Hvis du vil tilordne en Azure AD-gruppe med kilde til autoritet i Azure AD til en Azure AD-rolle, utfører du følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="6728d-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="6728d-104">Opprette en ny gruppe – for å opprette en ny gruppe:</span><span class="sxs-lookup"><span data-stu-id="6728d-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="6728d-105">a.</span><span class="sxs-lookup"><span data-stu-id="6728d-105">a.</span></span> <span data-ttu-id="6728d-106">Logg deg på administrasjons senteret for Azure AD med **privilegert rolle administrator** eller **globale administrator** tillatelser.</span><span class="sxs-lookup"><span data-stu-id="6728d-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="6728d-107">b.</span><span class="sxs-lookup"><span data-stu-id="6728d-107">b.</span></span> <span data-ttu-id="6728d-108">Velg **Azure Active Directory > groups > alle grupper > ny gruppe**.</span><span class="sxs-lookup"><span data-stu-id="6728d-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="6728d-109">c.</span><span class="sxs-lookup"><span data-stu-id="6728d-109">c.</span></span> <span data-ttu-id="6728d-110">Opprett gruppen.</span><span class="sxs-lookup"><span data-stu-id="6728d-110">Create the group.</span></span>

2. <span data-ttu-id="6728d-111">Tilordne rollen til gruppen under opprettelse av grupper, eller etter at gruppen er opprettet.</span><span class="sxs-lookup"><span data-stu-id="6728d-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="6728d-112">a.</span><span class="sxs-lookup"><span data-stu-id="6728d-112">a.</span></span> <span data-ttu-id="6728d-113">Hvis du vil tilordne en rolle til gruppen når du oppretter en gruppe, kan du bytte til Aktiver/deaktiver **Azure ad-roller for å tilordne gruppen** og opprette gruppen.</span><span class="sxs-lookup"><span data-stu-id="6728d-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="6728d-114">b.</span><span class="sxs-lookup"><span data-stu-id="6728d-114">b.</span></span> <span data-ttu-id="6728d-115">Hvis du vil tilordne en rolle til gruppen etter at den er opprettet, går du til fanen **tilordnede roller** for den nylig opprettede gruppen og tilordner rollen til gruppen.</span><span class="sxs-lookup"><span data-stu-id="6728d-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="6728d-116">**Behandle medlemskap i en gruppe som er tilordnet til Azure AD-rollen**</span><span class="sxs-lookup"><span data-stu-id="6728d-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="6728d-117">Som standard kan bare privilegerte rolle administratorer og globale administratorer endre medlemskapet for en gruppe som er tilordnet en rolle, for å hindre heving av tilgangs nivåer.</span><span class="sxs-lookup"><span data-stu-id="6728d-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="6728d-118">De kan imidlertid velge å tilordne en eier for en slik gruppe og delegere denne oppgaven.</span><span class="sxs-lookup"><span data-stu-id="6728d-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="6728d-119">Hvis du vil ha mer informasjon om hvordan du tilordner Sky grupper til Azure AD-roller, kan du se [tilordne en annonse roller til Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="6728d-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="6728d-120">Hvis du vil ha mer informasjon om feil søking av roller som er tilordnet til Sky grupper, kan du se [Feilsøke roller tilordnet til Sky grupper](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="6728d-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





