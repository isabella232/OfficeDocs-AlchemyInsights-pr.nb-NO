---
title: Fiks feilen Appen ble ikke funnet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810492"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="6c793-102">Fiks feilen «Appen ble ikke funnet»</span><span class="sxs-lookup"><span data-stu-id="6c793-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="6c793-103">Appinstallasjonsfeilen «Appen ble ikke funnet etter fullført installasjon», rapportert av Intune, kan oppstå på alle de store OS-plattformene (Windows, iOS og Android).</span><span class="sxs-lookup"><span data-stu-id="6c793-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="6c793-104">De vanligste scenarioene som genererer denne feilen inkluderer:</span><span class="sxs-lookup"><span data-stu-id="6c793-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="6c793-105">Appen er oppdatert utenfor Intune (fra en tredjeparts appbutikk) etter den første distribusjonen.</span><span class="sxs-lookup"><span data-stu-id="6c793-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="6c793-106">Noen apper, for eksempel Google Chrome, kan utføre automatiske oppdateringer.</span><span class="sxs-lookup"><span data-stu-id="6c793-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="6c793-107">En bruker har avinstallert appen etter den første installasjonen.</span><span class="sxs-lookup"><span data-stu-id="6c793-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="6c793-108">Løs dette problemet ved å først uføre en gjennomgang av enhetene som er påvirket for å fastslå scenarioet der problemet oppstår.</span><span class="sxs-lookup"><span data-stu-id="6c793-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="6c793-109">Hvis appen har blitt oppdatert utenfor Intune, kan du angi at appdistribusjonen skal ignorere appversjonen.</span><span class="sxs-lookup"><span data-stu-id="6c793-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="6c793-110">Dette gjør du ved å gå til **Appkonfigurasjon > Appinformasjon** og angi **Ignorer app**-versjon til **Ja**.</span><span class="sxs-lookup"><span data-stu-id="6c793-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="6c793-111">Når du angir klienten, kan det være hensiktsmessig å distribuere appen som «obligatorisk» samt sikre at det er den nyeste versjonen som distribueres.</span><span class="sxs-lookup"><span data-stu-id="6c793-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="6c793-112">Eventuelt kan du, på iOS-plattformen, bruke funksjonaliteten **automatisk oppdatering** som er tilknyttet Apple Volume Purchaase Program som kan konfigureres til å oppdatere seg automatisk til nye appversjoner når de blir tilgjengelige.</span><span class="sxs-lookup"><span data-stu-id="6c793-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="6c793-113">Hvis du vil ha mer informasjon om feilsøking av appinstallasjonsproblemer, kan du ta en titt på [Feilsøke problemer med appinstallasjoner](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="6c793-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
