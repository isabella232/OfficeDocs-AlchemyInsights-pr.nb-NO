---
title: Duplisert enhetspost i portalen
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814525"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="f3baa-102">Duplisert enhetspost i portalen</span><span class="sxs-lookup"><span data-stu-id="f3baa-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="f3baa-103">Det kan hende du ser to oppføringer for en enhet i portalen hvis enheten ikke rapporterer riktig delt administrasjonsstatus til nettstedet for konfigurasjonsbehandling.</span><span class="sxs-lookup"><span data-stu-id="f3baa-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="f3baa-104">Hvis du vil kontrollere statusen for en enhet, kan du se gjennom **delt administrasjon**-kolonnen for enheten i konfigurasjonsbehandling-konsollen.</span><span class="sxs-lookup"><span data-stu-id="f3baa-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="f3baa-105">Hvis kolonnen ikke vises, kan du legge den til ved å høyreklikke på en av kolonneoverskriftene og velge den fra listen.</span><span class="sxs-lookup"><span data-stu-id="f3baa-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="f3baa-106">Den verdien Delt administrasjon må være **Ja**.</span><span class="sxs-lookup"><span data-stu-id="f3baa-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="f3baa-107">Hvis verdien er **Nei**, åpner du klient-appleten for konfigurasjonsbehandling på klientenheten og merker av for **Delt administrasjon**-egenskapen i Generelt-fanen.</span><span class="sxs-lookup"><span data-stu-id="f3baa-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="f3baa-108">Hvis verdien er **Aktivert**, indikerer dette problemer med klientkommunikasjon ved administrasjonspunktet.</span><span class="sxs-lookup"><span data-stu-id="f3baa-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="f3baa-109">Se gjennom **CcmMessaging.log** på enheten for å undersøke mulige tilkoblingsproblemer.</span><span class="sxs-lookup"><span data-stu-id="f3baa-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="f3baa-110">Hvis verdien er **Deaktivert**, og enheten er registrert i Intune, må du kontrollere at enheten har mottatt policyen for delt administrasjon ved å gå gjennom **CoManagementHandler.log** på enheten.</span><span class="sxs-lookup"><span data-stu-id="f3baa-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
