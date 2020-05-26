---
title: Løse teams påloggingsfeil AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357875"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="a817c-102">Løse teams påloggingsfeil AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="a817c-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="a817c-103">Når du logger på Microsoft Teams, kan du få feilmeldingen: **Beklager, men vi har problemer med å logge deg på AADSTS9000411: Forespørselen er ikke riktig formatert. Parameteren "login_hint" dupliseres.**</span><span class="sxs-lookup"><span data-stu-id="a817c-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="a817c-104">Hvis du vil løse dette problemet, må du kontrollere at Microsoft Teams-klientene dine er oppdatert.</span><span class="sxs-lookup"><span data-stu-id="a817c-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="a817c-105">Hvis du vil ha mer informasjon om hvordan du oppdaterer klienten, kan du se [Oppdatere Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a817c-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="a817c-106">Hvis du av en eller annen grunn ikke kan oppdatere klienten, fjerner du de fleste hurtigbufrede dataene når du logger av klienten.</span><span class="sxs-lookup"><span data-stu-id="a817c-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="a817c-107">Hvis du fortsatt har problemer etter avlogging/pålogging, avslutter du Teams og fjerner klientbufferen ved å gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="a817c-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="a817c-108">Lukk Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a817c-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="a817c-109">Gå til: %appdata%\microsoft\teams, og slett alle filene.</span><span class="sxs-lookup"><span data-stu-id="a817c-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="a817c-110">Åpne Microsoft Teams på nytt.</span><span class="sxs-lookup"><span data-stu-id="a817c-110">Reopen Microsoft Teams.</span></span>
