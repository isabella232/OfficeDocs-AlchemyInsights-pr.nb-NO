---
title: Bruk TeamViewer til å administrere Intune-enheter eksternt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555243"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="334d8-102">Bruk TeamViewer til å administrere Intune-enheter eksternt</span><span class="sxs-lookup"><span data-stu-id="334d8-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="334d8-103">Enheter som administreres av Intune, kan administreres eksternt ved hjelp av [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="334d8-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="334d8-104">Hvis du vil administrere Intune ved hjelp av TeamViewer, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="334d8-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="334d8-105">Begynn med å få legitimasjon fra TeamViewer til å konfigurere TeamViewer Connector på Intune.</span><span class="sxs-lookup"><span data-stu-id="334d8-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="334d8-106">Dette gjør det mulig for administratoren å angi legitimasjon i Brukergrensesnittet for TeamViewer Connector under Enheter, en engangsoperasjon for å opprette koblingen mellom Intune og TeamViewer-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="334d8-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="334d8-107">**Del 1: Starte en økt med en ekstern enhet**</span><span class="sxs-lookup"><span data-stu-id="334d8-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="334d8-108">Velg enheten du vil starte en ekstern økt med, under **Alle enheter.**</span><span class="sxs-lookup"><span data-stu-id="334d8-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="334d8-109">Fra **... Mer**velger du **Ny fjernhjelpsøkt**.</span><span class="sxs-lookup"><span data-stu-id="334d8-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="334d8-110">Velg **Ja** for å bekrefte at du vil opprette en ekstern økt.</span><span class="sxs-lookup"><span data-stu-id="334d8-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="334d8-111">Når forespørselen "Starte en ny ekstern økt" er bekreftet av TeamViewer-tjenesten, ser du et alternativ for å **starte fjernhjelp** under detaljene i Oversikt (eller Essentials)-ruten for enheten.</span><span class="sxs-lookup"><span data-stu-id="334d8-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="334d8-112">Velg **Se mer** for å utvide ruten og vise Fjernhjelp-statusen.</span><span class="sxs-lookup"><span data-stu-id="334d8-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="334d8-113">Velg **Start ekstern økt** for å starte økten på administratorsiden.</span><span class="sxs-lookup"><span data-stu-id="334d8-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="334d8-114">Velg å laste ned TeamViewer binære (Windows), og velg **Kjør**.</span><span class="sxs-lookup"><span data-stu-id="334d8-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="334d8-115">**Merk at** Du kan ignorere alle nettlesersider som er åpnet for TeamViewer-nettstedet.</span><span class="sxs-lookup"><span data-stu-id="334d8-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="334d8-116">Bekreft forespørselen om at TeamViewer-appen skal gjøre endringer på enheten (bare Windows).</span><span class="sxs-lookup"><span data-stu-id="334d8-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="334d8-117">TeamViewer-appen starter og inkluderer øktkoden for å godkjenne tilkoblingen til den eksterne enheten.</span><span class="sxs-lookup"><span data-stu-id="334d8-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="334d8-118">**Del 2: På enheten som målrettes mot en ekstern økt**</span><span class="sxs-lookup"><span data-stu-id="334d8-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="334d8-119">Åpne Intune-firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="334d8-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="334d8-120">Se etter et varselflagg: «IT-administratoren ber om kontroll over denne enheten for en ekstern assistanseøkt», og velg varselet.</span><span class="sxs-lookup"><span data-stu-id="334d8-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="334d8-121">Velg å laste ned TeamViewer-appen, eller erkjenn nedlasting av TeamViewer-appen fra appbutikken, og velg **Kjør**.</span><span class="sxs-lookup"><span data-stu-id="334d8-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="334d8-122">**Merk at** Du kan ignorere alle nettlesersider som er åpnet for TeamViewer-nettstedet.</span><span class="sxs-lookup"><span data-stu-id="334d8-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="334d8-123">Bekreft forespørselen om at TeamViewer-appen skal gjøre endringer på enheten (bare Windows).</span><span class="sxs-lookup"><span data-stu-id="334d8-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="334d8-124">TeamViewer-appen starter og inkluderer øktkoden for å godkjenne tilkoblingen til den eksterne enheten.</span><span class="sxs-lookup"><span data-stu-id="334d8-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="334d8-125">En popup spør om du vil tillate økten å starte.</span><span class="sxs-lookup"><span data-stu-id="334d8-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="334d8-126">**Merk at** Øktkodene som genereres av TeamViewer-tjenesten, er bare engangsbruk.</span><span class="sxs-lookup"><span data-stu-id="334d8-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="334d8-127">Hvis du mister tilkoblingen, må du:</span><span class="sxs-lookup"><span data-stu-id="334d8-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="334d8-128">Lukk forekomsten av TeamViewer-appen på den eksterne enheten og på administrasjonsarbeidsstasjonen.</span><span class="sxs-lookup"><span data-stu-id="334d8-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="334d8-129">Lukk firmaportalen på den eksterne enheten.</span><span class="sxs-lookup"><span data-stu-id="334d8-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="334d8-130">Start en ny "Ny fjernhjelp-økt" fra administrasjonsportalen.</span><span class="sxs-lookup"><span data-stu-id="334d8-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="334d8-131">Åpne firmaportalen på den eksterne enheten på nytt for å motta det nye varselet.</span><span class="sxs-lookup"><span data-stu-id="334d8-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="334d8-132">Last ned og åpne TeamViewer-appen på både den eksterne enheten og administrasjonsarbeidsstasjonen, som før.</span><span class="sxs-lookup"><span data-stu-id="334d8-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>