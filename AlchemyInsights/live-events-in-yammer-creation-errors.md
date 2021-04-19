---
title: Feil ved opprettelse av direktesendte arrangementer i Yammer
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825524"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="2e75a-102">Feil ved opprettelse av direktesendte arrangementer i Yammer</span><span class="sxs-lookup"><span data-stu-id="2e75a-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="2e75a-103">**Opprettelse av direktesendte arrangementer i Yammer**</span><span class="sxs-lookup"><span data-stu-id="2e75a-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="2e75a-104">Yammer viser til enhver tid alternativet for å opprette et direktesendt arrangement.</span><span class="sxs-lookup"><span data-stu-id="2e75a-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="2e75a-105">I noen tilfeller kan det hende at en bruker ikke oppfyller kravene for å kunne opprette et direktesendt arrangement og får en feilmelding når de prøver å opprette det.</span><span class="sxs-lookup"><span data-stu-id="2e75a-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="2e75a-106">Nedenfor finner du de vanligste årsakene til dette problemet, og måter å løse det for sluttbrukere.</span><span class="sxs-lookup"><span data-stu-id="2e75a-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="2e75a-107">**Hvem kan opprette direktesendte arrangementer**</span><span class="sxs-lookup"><span data-stu-id="2e75a-107">**Who can create live events**</span></span>
- <span data-ttu-id="2e75a-108">En Office 365 Enterprise E1-, E3-eller E5-lisens eller en Office-365 A3-eller A5-lisens.</span><span class="sxs-lookup"><span data-stu-id="2e75a-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="2e75a-109">Tillatelse til å opprette direktesendte arrangementer i administrasjonssenteret for Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2e75a-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="2e75a-110">Tillatelse til å opprette direktesendte arrangementer i Microsoft Stream (for hendelser som produseres ved bruk av en ekstern kringkastingsapp eller enhet).</span><span class="sxs-lookup"><span data-stu-id="2e75a-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="2e75a-111">Fullstendig gruppemedlemskap i organisasjonen (kan ikke være en gjest eller fra en annen organisasjon).</span><span class="sxs-lookup"><span data-stu-id="2e75a-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="2e75a-112">Privat møtetidsplan, skjermdeling og deling av IP-video, aktivert i gruppemøtepolicyen.</span><span class="sxs-lookup"><span data-stu-id="2e75a-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="2e75a-113">**Policyer for opprettelse av direktesendte arrangementer**</span><span class="sxs-lookup"><span data-stu-id="2e75a-113">**Live event creation policies**</span></span>

<span data-ttu-id="2e75a-114">Yammer følger policyer for direktesendte arrangementer som er angitt i Office 365-tenant for Stream.</span><span class="sxs-lookup"><span data-stu-id="2e75a-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="2e75a-115">Alle i organisasjonen kan opprette direktesendte arrangementer som standard.</span><span class="sxs-lookup"><span data-stu-id="2e75a-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="2e75a-116">Administratorer kan [gjøre endringer i denne innstillingen, noe som kan hindre brukere i å opprette et direktesendt arrangement](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="2e75a-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="2e75a-117">Det er viktig å kontrollere at brukerne har tillatelse til å opprette direktesendte arrangementer hvis de får en policy-feil.</span><span class="sxs-lookup"><span data-stu-id="2e75a-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
