---
title: Administrere en brukertilordnede administrert identitet
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
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177772"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="3c9db-102">Administrere en brukertilordnede administrert identitet</span><span class="sxs-lookup"><span data-stu-id="3c9db-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="3c9db-103">Administrasjon av en brukertilordet administrert identitet omfatter:</span><span class="sxs-lookup"><span data-stu-id="3c9db-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="3c9db-104">Tilordne roller til en brukertilordnet administrert identitet</span><span class="sxs-lookup"><span data-stu-id="3c9db-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="3c9db-105">Slette en brukertilordnet administrert identitet</span><span class="sxs-lookup"><span data-stu-id="3c9db-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="3c9db-106">Liste over en brukertilordet administrert identitet</span><span class="sxs-lookup"><span data-stu-id="3c9db-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="3c9db-107">Hvis du vil ha mer informasjon om oppgavene som er nevnt ovenfor, kan du se følgende artikler:</span><span class="sxs-lookup"><span data-stu-id="3c9db-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="3c9db-108">[Slik oppretter du en brukertilordnet administrert identitet](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) for å tilordne roller til en brukertilordnet administrert identitet</span><span class="sxs-lookup"><span data-stu-id="3c9db-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="3c9db-109">[Slik sletter du en brukertilordnet administrert identitet](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – for å slette en brukertilordnet administrert identitet</span><span class="sxs-lookup"><span data-stu-id="3c9db-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="3c9db-110">[Slik viser du en brukertilordnede administrert identitet](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) for oppføring av en brukertilordnet administrert identitet</span><span class="sxs-lookup"><span data-stu-id="3c9db-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="3c9db-111">Kontroller om du har **rolletilordningen** for bidragsyter med forvaltet identitet.</span><span class="sxs-lookup"><span data-stu-id="3c9db-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="3c9db-112">Denne rolletilordningen er nødvendig for å opprette/slette brukertilordnede administrerte identiteter.</span><span class="sxs-lookup"><span data-stu-id="3c9db-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
