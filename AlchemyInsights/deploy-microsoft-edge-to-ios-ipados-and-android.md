---
title: Distribuere Microsoft Edge til iOS, iPadOS og Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194517"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="562e0-102">Distribuere Microsoft Edge til iOS, iPadOS og Android</span><span class="sxs-lookup"><span data-stu-id="562e0-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="562e0-103">Veiledningsscenarioet oppsummert nedenfor hjelper deg med å tilordne Microsoft Edge til brukere av iOS-, iPadOS- og Android-enheter.</span><span class="sxs-lookup"><span data-stu-id="562e0-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="562e0-104">Hvis du har blokkert brukere fra å registrere mobile enheter, vil ikke dette veiledede scenarioet fungere, og brukerne må installere Microsoft Edge på egen hånd.</span><span class="sxs-lookup"><span data-stu-id="562e0-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="562e0-105">Veiledet scenario omfatter følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="562e0-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="562e0-106">Forutsetninger</span><span class="sxs-lookup"><span data-stu-id="562e0-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="562e0-107">Innledning</span><span class="sxs-lookup"><span data-stu-id="562e0-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="562e0-108">Grunnleggende</span><span class="sxs-lookup"><span data-stu-id="562e0-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="562e0-109">Konfigurasjon</span><span class="sxs-lookup"><span data-stu-id="562e0-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="562e0-110">Oppgaver</span><span class="sxs-lookup"><span data-stu-id="562e0-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="562e0-111">Se gjennom og oppretting</span><span class="sxs-lookup"><span data-stu-id="562e0-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="562e0-112">Når du har fullført trinnene i det veiledede scenarioet, aktiverer Microsoft Intune-policyer følgende funksjoner i Microsoft Edge for bedrifter:</span><span class="sxs-lookup"><span data-stu-id="562e0-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="562e0-113">To identiteter</span><span class="sxs-lookup"><span data-stu-id="562e0-113">Dual identity</span></span>
- <span data-ttu-id="562e0-114">Integrering med beskyttelsespolicy for Microsoft Intune-appen</span><span class="sxs-lookup"><span data-stu-id="562e0-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="562e0-115">Integrasjon med Azure Active Directory-programproxy</span><span class="sxs-lookup"><span data-stu-id="562e0-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="562e0-116">Administrerte favoritter og snarveier på startsiden</span><span class="sxs-lookup"><span data-stu-id="562e0-116">Managed favorites and home page shortcuts</span></span>
