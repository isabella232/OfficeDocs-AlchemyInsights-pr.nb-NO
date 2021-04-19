---
title: Adressering av påloggingsfeil i Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821996"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="3406a-102">Adressering av påloggingsfeil i Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="3406a-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="3406a-103">Når du logger på Microsoft Teams, kan du få feilmeldingen: Beklager, men vi har problemer med å logge deg på **AADSTS9000411: Forespørselen er ikke riktig formatert. Parameteren "login_hint" er duplisert.**</span><span class="sxs-lookup"><span data-stu-id="3406a-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="3406a-104">For å løse dette problemet må du sørge for at Microsoft Teams-klientene er oppdatert.</span><span class="sxs-lookup"><span data-stu-id="3406a-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="3406a-105">Hvis du vil ha mer informasjon om hvordan du oppdaterer klienten, kan [du se Oppdatere Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="3406a-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="3406a-106">Hvis du av en eller annen grunn ikke kan oppdatere klienten, vil logging av klienten fjerne de fleste bufrede data.</span><span class="sxs-lookup"><span data-stu-id="3406a-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="3406a-107">Men hvis du fremdeles har problemer etter avlogging/pålogging, avslutter du Teams og tømmer klienthurtigbufferen ved å gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="3406a-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="3406a-108">Lukk Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3406a-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="3406a-109">Gå til: %appdata%\microsoft\teams, og slett alle filene.</span><span class="sxs-lookup"><span data-stu-id="3406a-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="3406a-110">Åpne Microsoft Teams på nytt.</span><span class="sxs-lookup"><span data-stu-id="3406a-110">Reopen Microsoft Teams.</span></span>
