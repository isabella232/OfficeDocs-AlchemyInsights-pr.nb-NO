---
title: Tilordne en rolle i overvåkingsloggen i sikkerhets- & i Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749517"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="917b3-102">Tilordne en rolle i overvåkingsloggen i sikkerhets- & i Office 365</span><span class="sxs-lookup"><span data-stu-id="917b3-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="917b3-103">Hvis du vil søke i office 365-overvåkingsloggen, må en administrator tilordnes rollen Bare **overvåkingslogger** eller rollen **Overvåkingslogger** i Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="917b3-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="917b3-104">Disse rollene er som standard tilordnet rollegruppene Samsvarsbehandling og Organisasjonsbehandling.</span><span class="sxs-lookup"><span data-stu-id="917b3-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="917b3-105">Globale administratorer i Office 365 og Microsoft 365 legges automatisk til som medlemmer av rollegruppen organisasjonsbehandling.</span><span class="sxs-lookup"><span data-stu-id="917b3-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="917b3-106">Hvis du vil at en bruker skal kunne søke med minimum tilgangsnivå, oppretter du en egendefinert rollegruppe i Exchange Online, legger til rollen Bare overvåkingslogger eller **Overvåkingslogger,** og deretter legger du til brukeren som medlem av den nye rollegruppen. </span><span class="sxs-lookup"><span data-stu-id="917b3-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="917b3-107">Hvis du vil ha mer informasjon, kan du se Administrere [rollegrupper i Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) og Søke i overvåkingsloggen [i sikkerhets- & samsvarssenteret](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="917b3-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>