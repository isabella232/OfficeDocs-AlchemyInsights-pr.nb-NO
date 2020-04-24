---
title: Duplisert enhetspost i portalen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790166"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="6a6ff-102">Duplisert enhetspost i portalen</span><span class="sxs-lookup"><span data-stu-id="6a6ff-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="6a6ff-103">Det kan hende du ser to oppføringer for en enhet i portalen hvis enheten ikke rapporterer riktig delt administrasjonsstatus til nettstedet for konfigurasjonsbehandling.</span><span class="sxs-lookup"><span data-stu-id="6a6ff-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="6a6ff-104">Hvis du vil kontrollere statusen for en enhet, kan du se gjennom **delt administrasjon**-kolonnen for enheten i konfigurasjonsbehandling-konsollen.</span><span class="sxs-lookup"><span data-stu-id="6a6ff-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="6a6ff-105">Hvis kolonnen ikke vises, kan du legge den til ved å høyreklikke på en av kolonneoverskriftene og velge den fra listen.</span><span class="sxs-lookup"><span data-stu-id="6a6ff-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="6a6ff-106">Den verdien Delt administrasjon må være **Ja**.</span><span class="sxs-lookup"><span data-stu-id="6a6ff-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="6a6ff-107">Hvis verdien er **Nei**, åpner du klient-appleten for konfigurasjonsbehandling på klientenheten og merker av for **Delt administrasjon**-egenskapen i Generelt-fanen.</span><span class="sxs-lookup"><span data-stu-id="6a6ff-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="6a6ff-108">Hvis verdien er **Aktivert**, indikerer dette problemer med klientkommunikasjon ved administrasjonspunktet.</span><span class="sxs-lookup"><span data-stu-id="6a6ff-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="6a6ff-109">Se gjennom **CcmMessaging.log** på enheten for å undersøke mulige tilkoblingsproblemer.</span><span class="sxs-lookup"><span data-stu-id="6a6ff-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="6a6ff-110">Hvis verdien er**Deaktivert**, og enheten er registrert i Intune, må du kontrollere at enheten har mottatt policyen for delt administrasjon ved å gå gjennom **CoManagementHandler.log** på enheten.</span><span class="sxs-lookup"><span data-stu-id="6a6ff-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
