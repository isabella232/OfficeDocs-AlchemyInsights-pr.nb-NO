---
title: Problemer med Yammer-lisensiering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657285"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="b2b83-102">Problemer med Yammer-lisensiering</span><span class="sxs-lookup"><span data-stu-id="b2b83-102">Yammer licensing issues</span></span>

<span data-ttu-id="b2b83-103">Alle brukere må ha en lisens for å bruke Yammer Enterprise-tjenesten, men som standard er Yammer ikke nødvendig for at brukere har en lisens for å få tilgang til tjenesten.</span><span class="sxs-lookup"><span data-stu-id="b2b83-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="b2b83-104">Når en administrator endrer innstillingen for å blokkere Microsoft 365-brukere uten Yammer-lisenser, får ikke brukere tilordnet en Yammer Enterprise-lisens til å få tilgang til Yammer-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="b2b83-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="b2b83-105">Hvis du vil ha mer informasjon, kan du se [administrere bruker lisenser for Yammer i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="b2b83-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="b2b83-106">Når lisenser er fjernet fra brukere, vises ikke lenger Yammer-delark, og andre tjenester kan bruke fjerning av lisenser til å skjule funksjoner.</span><span class="sxs-lookup"><span data-stu-id="b2b83-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="b2b83-107">I andre tilfeller kan funksjoner fortsatt vises, men krever lisens tilordning for å fungere.</span><span class="sxs-lookup"><span data-stu-id="b2b83-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="b2b83-108">**Lisensen blir ikke oppdatert for brukeren**</span><span class="sxs-lookup"><span data-stu-id="b2b83-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="b2b83-109">Noen ganger er en bruker tilordnet en lisens, men har fremdeles ikke tilgang til Yammer.</span><span class="sxs-lookup"><span data-stu-id="b2b83-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="b2b83-110">Det er mer sannsynlig at forsinkelser oppstår når en masse lisens tildeling pågår.</span><span class="sxs-lookup"><span data-stu-id="b2b83-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="b2b83-111">Yammer-brukere blir kanskje ikke oppdatert i samme rekkefølge som lisenser endres i Azure AD fordi systemet kjører asynkront.</span><span class="sxs-lookup"><span data-stu-id="b2b83-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="b2b83-112">Vent opptil 24 timer før du åpner en støtte sak for å rapportere synkroniserings problemer med lisenser.</span><span class="sxs-lookup"><span data-stu-id="b2b83-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="b2b83-113">**Masse lisens tilordning**</span><span class="sxs-lookup"><span data-stu-id="b2b83-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="b2b83-114">Lisenser kan tildeles gjennom administrasjons senteret eller PowerShell-skript.</span><span class="sxs-lookup"><span data-stu-id="b2b83-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="b2b83-115">Hvis du vil ha mer informasjon, kan du se [Tilordne lisenser til brukere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og [Tilordne lisenser til bruker kontoer med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="b2b83-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="b2b83-116">Microsoft kunde støtte gir ikke hjelp til å opprette skript, men dokumentasjon om Yammer-lisens tildeling er tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="b2b83-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="b2b83-117">Hvis du vil ha mer informasjon, kan du se [administrere Yammer-lisenser ved hjelp av Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="b2b83-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>