---
title: DLP Policy Tips fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932595"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="ec91d-102">Problemer med dlp policy tips</span><span class="sxs-lookup"><span data-stu-id="ec91d-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="ec91d-103">**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen.</span><span class="sxs-lookup"><span data-stu-id="ec91d-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ec91d-104">Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger.</span><span class="sxs-lookup"><span data-stu-id="ec91d-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ec91d-105">I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.</span><span class="sxs-lookup"><span data-stu-id="ec91d-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ec91d-106">Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene.</span><span class="sxs-lookup"><span data-stu-id="ec91d-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ec91d-107">Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider.</span><span class="sxs-lookup"><span data-stu-id="ec91d-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ec91d-108">I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.</span><span class="sxs-lookup"><span data-stu-id="ec91d-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ec91d-109">**Tips om DLP-retningslinjer**</span><span class="sxs-lookup"><span data-stu-id="ec91d-109">**DLP policy tips**</span></span>

<span data-ttu-id="ec91d-110">Når du bruker **DLP-policyer,** kan brukere bli varslet om et brudd på retningslinjene med **policytips**.</span><span class="sxs-lookup"><span data-stu-id="ec91d-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="ec91d-111">Administratorer kan konfigurere policytips som skal vises mens de tester DLP-policyen eller når policyen er i full håndhevelsesmodus.</span><span class="sxs-lookup"><span data-stu-id="ec91d-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="ec91d-112">Hvis du vil konfigurere policytips for DLP-policyen i sikkerhets- og samsvarssenteret i full håndhevelsesmodus, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="ec91d-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="ec91d-113">Kontroller at policytips er **aktivert** i DLP-regelen ved hjelp av trinnene [her](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="ec91d-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="ec91d-114">Sørg for at **innholdet samsvarer med** det som **kreves** for å utløse regelen som er beskrevet i denne artikkelen [her](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="ec91d-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="ec91d-115">Policytips vises i både OWA og Outlook.</span><span class="sxs-lookup"><span data-stu-id="ec91d-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="ec91d-116">Når du bruker **Outlook 2013 eller senere**, vises imidlertid policytips bare under visse forhold.</span><span class="sxs-lookup"><span data-stu-id="ec91d-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="ec91d-117">Disse betingelsene er oppført her: [Støttede betingelser for Outlook 2013 eller nyere for visning av policytips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="ec91d-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="ec91d-118">Hvis du vil ha mer informasjon om tips om DLP-policy, kan du se: [Vise policytips for DLP-policyer](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="ec91d-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  