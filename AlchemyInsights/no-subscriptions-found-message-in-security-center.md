---
title: Finner ingen abonnementer-melding i sikkerhetssenteret
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544117"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="71265-102">Finner ingen abonnementer-melding i sikkerhetssenteret</span><span class="sxs-lookup"><span data-stu-id="71265-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="71265-103">Hvis du får meldingen «Ingen abonnementer funnet» når du åpner Microsoft Defender Sikkerhetssenter, betyr det at Azure Active Directory (AAD) som brukes til å logge på brukeren til portalen, ikke har en Microsoft Defender ATP lisens.</span><span class="sxs-lookup"><span data-stu-id="71265-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="71265-104">Lisensene Windows E5 og Office E5 er separate lisenser.</span><span class="sxs-lookup"><span data-stu-id="71265-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="71265-105">Åpne en støttesak hvis lisensen ble kjøpt, men ikke klargjort for denne AAD-forekomsten.</span><span class="sxs-lookup"><span data-stu-id="71265-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="71265-106">Enten har du:</span><span class="sxs-lookup"><span data-stu-id="71265-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="71265-107">Et mulig problem med klargjøring av lisens.</span><span class="sxs-lookup"><span data-stu-id="71265-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="71265-108">Du klargjorte utilsiktet lisensen til en annen Microsoft AAD enn den som ble brukt for godkjenning i tjenesten.</span><span class="sxs-lookup"><span data-stu-id="71265-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>