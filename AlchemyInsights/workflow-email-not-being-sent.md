---
title: E-post for arbeidsflyt sendes ikke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766142"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="64235-102">Arbeidsflyt-e-post sendes ikke for en SharePoint-liste eller et bibliotek</span><span class="sxs-lookup"><span data-stu-id="64235-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="64235-103">E-post fra arbeidsflyter sendes ikke til alle brukere eller bare bestemte brukere, eller du ser feilen **E-postmeldingen kan ikke sendes. Kontroller at e-posten har en gyldig mottaker**.</span><span class="sxs-lookup"><span data-stu-id="64235-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="64235-104">Kontroller om brukeren finnes i gruppen **Alle personertillatelser** (brukerinformasjonsliste) for denne områdesamlingen.</span><span class="sxs-lookup"><span data-stu-id="64235-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="64235-105">Eksempel på direkte<tenant>URL-adresse: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MedlemskapGruppeId=0</span><span class="sxs-lookup"><span data-stu-id="64235-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="64235-106">Hvis brukeren ikke finnes, må du kontrollere at brukeren er logget på siden.</span><span class="sxs-lookup"><span data-stu-id="64235-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="64235-107">Hvis det er en ekstern bruker, må du kontrollere at invitasjonen er godtatt.</span><span class="sxs-lookup"><span data-stu-id="64235-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="64235-108">Hvis brukeren finnes i tillatelsesgruppen, må du kontrollere at e-postadressen er riktig.</span><span class="sxs-lookup"><span data-stu-id="64235-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="64235-109">Hvis brukernes e-postadresse ikke er angitt her, oppretter du et eksempelvarsel for brukeren som tvinger synkroniseringen av denne brukerkontoen fra brukerprofiler i SharePoint til denne områdesamlingen.</span><span class="sxs-lookup"><span data-stu-id="64235-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="64235-110">E-post fra arbeidsflyter sendes til administratorer for områdesamling, men ikke til andre brukere og se feilen **HTTP forbudt å <span>https:</span>//URL/_vti_bin/client.xvc.sp.ilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="64235-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="64235-111">Se [Ingen tilgang når du sender en e-post til en SharePoint-gruppe](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="64235-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="64235-112">Kontroller også at funksjonen for **begrenset tilgang til brukertillatelse lockdown modus** områdesamling ikke er aktiv.</span><span class="sxs-lookup"><span data-stu-id="64235-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="64235-113">Beslektede emner</span><span class="sxs-lookup"><span data-stu-id="64235-113">Related topics</span></span>
<span data-ttu-id="64235-114">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="64235-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="64235-115">Opprett flyt</span><span class="sxs-lookup"><span data-stu-id="64235-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="64235-116">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="64235-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


