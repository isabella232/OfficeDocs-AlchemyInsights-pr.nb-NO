---
title: Problemer med Yammer-lisensiering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148315"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="01fce-102">Problemer med Yammer-lisensiering</span><span class="sxs-lookup"><span data-stu-id="01fce-102">Yammer licensing issues</span></span>

<span data-ttu-id="01fce-103">Alle brukere må ha en lisens til å bruke Yammer Enterprise-tjenesten, men som standard krever ikke Yammer at brukere har en lisens for å få tilgang til tjenesten.</span><span class="sxs-lookup"><span data-stu-id="01fce-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="01fce-104">Når en administrator endrer innstillingen for å blokkere Microsoft 365-brukere uten Yammer-lisenser, får ikke brukere tilordnet en Yammer Enterprise-lisens tilgang til Yammer-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="01fce-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="01fce-105">Hvis du vil ha mer informasjon, kan du se [Administrere Yammer-brukerlisenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="01fce-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="01fce-106">Når lisenser fjernes fra brukere, Yammer-flisen vises ikke lenger, og andre tjenester kan bruke lisensfjerning til å skjule funksjoner.</span><span class="sxs-lookup"><span data-stu-id="01fce-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="01fce-107">I andre tilfeller kan funksjoner fortsatt vises, men krever lisenstilordning for å fungere.</span><span class="sxs-lookup"><span data-stu-id="01fce-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="01fce-108">**Lisensen blir ikke oppdatert for brukeren**</span><span class="sxs-lookup"><span data-stu-id="01fce-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="01fce-109">Noen ganger tilordnes en bruker en lisens, men får fortsatt ikke tilgang til Yammer.</span><span class="sxs-lookup"><span data-stu-id="01fce-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="01fce-110">Forsinkelser er mer sannsynlig å oppstå når en masselisenstilordning pågår.</span><span class="sxs-lookup"><span data-stu-id="01fce-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="01fce-111">Yammer-brukere kan ikke oppdateres i samme rekkefølge som lisenser endres i Azure AD fordi systemet kjører asynkront.</span><span class="sxs-lookup"><span data-stu-id="01fce-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="01fce-112">Vent opptil 24 timer før du åpner en støttesak for å rapportere problemer med lisenssynkronisering.</span><span class="sxs-lookup"><span data-stu-id="01fce-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="01fce-113">**Tildeling av masselisens**</span><span class="sxs-lookup"><span data-stu-id="01fce-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="01fce-114">Lisenser kan tilordnes via administrasjonssenteret eller PowerShell-skripting.</span><span class="sxs-lookup"><span data-stu-id="01fce-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="01fce-115">Hvis du vil ha mer informasjon, kan du se [Tilordne lisenser til brukere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og tilordne [lisenser til brukerkontoer med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="01fce-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="01fce-116">Microsoft Support gir ikke hjelp til å opprette skript, men dokumentasjon på Yammer-lisenstilordning er tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="01fce-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="01fce-117">Hvis du vil ha mer informasjon, kan du se [Administrere Yammer-lisenser ved hjelp av Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="01fce-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>