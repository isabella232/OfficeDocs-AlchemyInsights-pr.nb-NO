---
title: Problemer med å bruke Intune admin console
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555387"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="8093c-102">Problemer med å bruke Intune admin console</span><span class="sxs-lookup"><span data-stu-id="8093c-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="8093c-103">**"Ingen tilgang" når du navigerer i administrasjonsportalen for Intune.**</span><span class="sxs-lookup"><span data-stu-id="8093c-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="8093c-104">Hvis du er medlem av en egendefinert intune-rolle, må du kontrollere at en Intune- eller Enterprise Mobility Suite (EMS)-lisens er tilordnet kontoen din.</span><span class="sxs-lookup"><span data-stu-id="8093c-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="8093c-105">Hvis du bruker Configuration Manager til å administrere enheter, må du kontrollere at du ikke er en del av Intune-brukersamlingen for Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="8093c-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="8093c-106">Kontroller at du er tilordnet de riktige rollebaserte administrasjonskontrolltillatelsene (RBAC) i intune-rollebladet.</span><span class="sxs-lookup"><span data-stu-id="8093c-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="8093c-107">Kontroller at gruppen som brukes, ikke er en distribusjonsliste.</span><span class="sxs-lookup"><span data-stu-id="8093c-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="8093c-108">Intune i Azure-portalen støtter bare brukerkontoer som tilhører Azure Active Directory-sikkerhetsgrupper.</span><span class="sxs-lookup"><span data-stu-id="8093c-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="8093c-109">Se gjennom gruppene i Azure-portalen > **Intune**  >  **Groups**eller i Azure-portalen > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="8093c-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="8093c-110">**Brukeren har for mange tillatelser for tilordnet Intune-rolle**</span><span class="sxs-lookup"><span data-stu-id="8093c-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="8093c-111">Råder brukeren til å gå til **Intune**  >  **Intune roller**  >  **Mine tillatelser**  >  **Eksporter** for å se gjennom gitte tillatelser.</span><span class="sxs-lookup"><span data-stu-id="8093c-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="8093c-112">**Jeg har lagt til en omfangsgruppe i en rolle, men brukere i denne rollen ser fortsatt andre brukere eller enheter.**</span><span class="sxs-lookup"><span data-stu-id="8093c-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="8093c-113">Omfangsgrupper filtrerer ikke ut brukere eller enheter.</span><span class="sxs-lookup"><span data-stu-id="8093c-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="8093c-114">Omfangsgrupper:</span><span class="sxs-lookup"><span data-stu-id="8093c-114">Scope groups:</span></span>

- <span data-ttu-id="8093c-115">Begrens hvem brukere kan tilordne policyer eller programmer til.</span><span class="sxs-lookup"><span data-stu-id="8093c-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="8093c-116">Tillat bare bestemte brukere å kjøre eksterne oppgaver på enheter.</span><span class="sxs-lookup"><span data-stu-id="8093c-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="8093c-117">Hvis du vil ha mer informasjon om omfangsgrupper, kan du se [Rollebasert tilgangskontroll (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="8093c-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="8093c-118">**Jeg har lagt til en bruker i en Intune-rolle, men de har fortsatt full tilgang til Intune admin console.**</span><span class="sxs-lookup"><span data-stu-id="8093c-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="8093c-119">Naviger til Intune > **brukere** i Azure-portalen, og kontroller at brukeren ikke er tilordnet til noen av følgende roller i Azure-portalen:</span><span class="sxs-lookup"><span data-stu-id="8093c-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="8093c-120">Global administrator</span><span class="sxs-lookup"><span data-stu-id="8093c-120">Global administrator</span></span>
- <span data-ttu-id="8093c-121">Intune-tjenesteadministrator</span><span class="sxs-lookup"><span data-stu-id="8093c-121">Intune service administrator</span></span>
- <span data-ttu-id="8093c-122">SharePoint-administrator</span><span class="sxs-lookup"><span data-stu-id="8093c-122">SharePoint administrator</span></span>

<span data-ttu-id="8093c-123">Hvis du vil ha mer informasjon, kan du se [Rollebasert tilgangskontroll (RBAC) med Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="8093c-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="8093c-124">**Problemer med tilgang**</span><span class="sxs-lookup"><span data-stu-id="8093c-124">**Access Issues**</span></span>

<span data-ttu-id="8093c-125">Hvis du vil ha mer informasjon, kan du se [Du kan ikke logge på Office 365, Azure eller Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="8093c-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>