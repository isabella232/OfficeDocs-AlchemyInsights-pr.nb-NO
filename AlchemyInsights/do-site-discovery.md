---
title: Gjøre nettstedsoppdaging
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694563"
---
# <a name="do-site-discovery"></a><span data-ttu-id="8e9eb-102">Gjøre nettstedsoppdaging</span><span class="sxs-lookup"><span data-stu-id="8e9eb-102">Do site discovery</span></span>

<span data-ttu-id="8e9eb-103">Hvis organisasjonen fremdeles bruker eldre nettprogrammer og planer til å bruke Internet Explorer-modus (som de fleste kunder gjør), bør du gjøre noe ekstra nettstedsoppdaging.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="8e9eb-104">**Du har allerede distribuert en eldre versjon av Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="8e9eb-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="8e9eb-105">Hvis du allerede har konfigurert listen over virksomhetsnettsteder til å fungere for den eldre versjonen av Microsoft Edge, er nettstedssøk nesten ferdig.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="8e9eb-106">Det du kanskje må gjøre, er å legge til nøytrale nettsteder.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="8e9eb-107">Nøytrale nettsteder er vanligvis nettsteder som gir enkel pålogging (SSO).</span><span class="sxs-lookup"><span data-stu-id="8e9eb-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="8e9eb-108">Hvis du går til et nøytralt nettsted fra Microsoft Edge, ønsker du å bli i Microsoft Edge for å godkjenne.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="8e9eb-109">Hvis du går til et nøytralt nettsted i Internet Explorer-modus, må du være i Internet Explorer-modus for å godkjenne.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="8e9eb-110">Identifiser eventuelle SSO-er eller andre nøytrale nettsteder du bruker, og legg dem til i listen over virksomhetsnettsteder.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="8e9eb-111">**Internet Explorer er standardleseren din**</span><span class="sxs-lookup"><span data-stu-id="8e9eb-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="8e9eb-112">Hvis du bare bruker Internet Explorer nå, vet du kanskje ikke hvilke nettsteder som har oppgradert til moderne nettstandarder, og som fremdeles krever Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="8e9eb-113">Du kan finne og legge til disse nettstedene i listen over virksomhetsnettsteder, slik at du bare kan bruke Internet Explorer-modus for disse nettstedene.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="8e9eb-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) oppdager nettsteder som kanskje trenger Internet Explorer-modus.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="8e9eb-115">Den kan samle inn data på datamaskiner som kjører Windows Internet Explorer 8 via Internet Explorer 11 på Windows 10, Windows 8.1 eller Windows 7.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="8e9eb-116">**Analysere dataene**</span><span class="sxs-lookup"><span data-stu-id="8e9eb-116">**Analyze the data**</span></span>

<span data-ttu-id="8e9eb-117">Når du har samlet inn nettstedsdata, anbefaler vi følgende firetrinns prosess for å analysere dataene:</span><span class="sxs-lookup"><span data-stu-id="8e9eb-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="8e9eb-118">Sorter dataene etter domene, og deretter etter URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="8e9eb-119">Definer grensene for en app for å konfigurere for Internet Explorer-modus.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="8e9eb-120">Du vil inkludere alle nettstedene og nettkontrollene som definerer appen, men du vil ikke inkludere ekstra nettsteder og kontroller.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="8e9eb-121">Noen nettsteder kan være så enkle som, mens andre kan kreve at du *https://contoso.com/app1* definerer flere nettsteder og sider.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="8e9eb-122">Test appen for å bekrefte at den ikke fungerer opprinnelig.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="8e9eb-123">Mange nettsteder tilbyr moderne innhold når de oppdager en moderne nettleser og bare tilbyr eldre innhold når de oppdager Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="8e9eb-124">Legg til appen i listen over virksomhetsnettsteder hvis den ikke tester.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="8e9eb-125">Den beste praksisen er å gruppere alle nettstedene som utgjør en app.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="8e9eb-126">Når du oppgraderer en app, er det på denne måten enklere å fjerne hele nettstedet fra Internet Explorer-modus og begynne å bruke en moderne nettleser for appen.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="8e9eb-127">Når du er ferdig med nettstedsoppdagingen og du har analysert dataene, er du klar til å begynne å se på kanalstrategien.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

