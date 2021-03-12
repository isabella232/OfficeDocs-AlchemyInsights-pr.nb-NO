---
title: Melding om at ingen abonnementer blir funnet i sikkerhetssenteret
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713960"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="25077-102">Melding om at ingen abonnementer blir funnet i sikkerhetssenteret</span><span class="sxs-lookup"><span data-stu-id="25077-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="25077-103">Hvis du får meldingen «Ingen abonnementer funnet» når du åpner Microsoft Defender Sikkerhetssenter, betyr det at Azure Active Directory (AAD) som brukes til å logge brukeren på portalen, ikke har en Microsoft Defender ATP-lisens.</span><span class="sxs-lookup"><span data-stu-id="25077-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="25077-104">Lisensene for Windows E5 og Office E5 er separate lisenser.</span><span class="sxs-lookup"><span data-stu-id="25077-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="25077-105">Åpne en kundestøttesak hvis lisensen ble kjøpt, men ikke klargjort for denne AAD-forekomsten.</span><span class="sxs-lookup"><span data-stu-id="25077-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="25077-106">Enten har du:</span><span class="sxs-lookup"><span data-stu-id="25077-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="25077-107">Et mulig problem med klargjøring av lisens.</span><span class="sxs-lookup"><span data-stu-id="25077-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="25077-108">Du klargjorte utilsiktet lisensen til en annen Microsoft AAD enn den som ble brukt for godkjenning i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="25077-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>