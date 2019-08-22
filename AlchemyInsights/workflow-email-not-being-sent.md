---
title: Arbeidsflyt for e-post blir ikke sendt
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530892"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="30581-102">Arbeidsflyt for e-post blir ikke sendt til en SharePoint-liste eller et bibliotek</span><span class="sxs-lookup"><span data-stu-id="30581-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="30581-103">E-post fra arbeidsflyter er ikke sendt til alle brukere eller bare bestemte brukere, eller du ser feil **i e-postmeldingen ikke kan sendes. Kontroller at e-postmeldingen har en gyldig mottaker**.</span><span class="sxs-lookup"><span data-stu-id="30581-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="30581-104">Kontroller om brukeren finnes i **Alle** tillatelsene gruppen (Brukerinformasjonsliste) for denne områdesamlingen.</span><span class="sxs-lookup"><span data-stu-id="30581-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="30581-105">Eksempel på direkte URL-adressen: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="30581-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="30581-106">Hvis brukeren ikke finnes, kontrollerer du at brukeren er logget inn på siden.</span><span class="sxs-lookup"><span data-stu-id="30581-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="30581-107">Hvis det er en ekstern bruker, må du kontrollere at deres invitasjonen er godtatt.</span><span class="sxs-lookup"><span data-stu-id="30581-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="30581-108">Hvis brukeren finnes i gruppen tillatelser, må du kontrollere e-postadressen er riktig.</span><span class="sxs-lookup"><span data-stu-id="30581-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="30581-109">Hvis e-postadressen som brukerne ikke er angitt her, oppretter du et eksempel på varselet for brukeren som fremtvinger synkronisering av brukerkontoen fra profiler av SharePoint for denne områdesamlingen.</span><span class="sxs-lookup"><span data-stu-id="30581-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="30581-110">E-post fra arbeidsflyter er sendt til administratorene for områdesamling, men ikke til andre brukere, og se feilen **HTTP forbudt å <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="30581-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="30581-111">Se [Tilgang når du sender en e-post til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="30581-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="30581-112">Kontroller også at funksjonen **begrenset tilgang tillatelse lockdown brukermodus** samlingen ikke er aktiv.</span><span class="sxs-lookup"><span data-stu-id="30581-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="30581-113">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="30581-113">Related topics</span></span>
<span data-ttu-id="30581-114">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="30581-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="30581-115">Opprette flyt</span><span class="sxs-lookup"><span data-stu-id="30581-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="30581-116">SharePoint og flyt</span><span class="sxs-lookup"><span data-stu-id="30581-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


