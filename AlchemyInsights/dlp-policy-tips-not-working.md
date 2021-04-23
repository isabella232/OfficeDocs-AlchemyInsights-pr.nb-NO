---
title: DLP-policytips fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 68387bf6f5f91657f1d853b9d67bdea6fac21bde
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952201"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="16638-102">Problemer med DLP-policytips</span><span class="sxs-lookup"><span data-stu-id="16638-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="16638-103">**Viktig**: I disse enestående tidene tar vi grep for å sikre at SharePoint Online-og OneDrive-tjenester forblir svært tilgjengelige – Gå til [Midlertidige SharePoint Online-funksjoner](https://aka.ms/ODSPAdjustments) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="16638-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="16638-104">Hvis du vil konfigurere policytips for DLP-policyen i sikkerhetssenteret & samsvarssenteret i full håndhevelsesmodus, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="16638-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="16638-105">Kontroller at policytips er **aktivert** på DLP-regelen.</span><span class="sxs-lookup"><span data-stu-id="16638-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="16638-106">Hvis du vil ha mer informasjon, kan du se [Sende e-postvarsler og vise policytips for DLP-policyer](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="16638-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="16638-107">Kontroller at innholdet samsvarer med det som kreves for å utløse regelen som er beskrevet i enhetsdefinisjoner [for Sensitiv informasjonstype](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="16638-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

<span data-ttu-id="16638-108">Policytips vises i både OWA og Outlook.</span><span class="sxs-lookup"><span data-stu-id="16638-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="16638-109">Når du bruker Outlook 2013 eller nyere, vises imidlertid policytips bare under visse betingelser.</span><span class="sxs-lookup"><span data-stu-id="16638-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="16638-110">Hvis du vil se listen over bestemte betingelser, kan du se Støttede betingelser [for Outlook 2013 eller nyere for å vise policytips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="16638-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="16638-111">Hvis du vil ha informasjon om tips for DLP-policyer, kan du se Tips for [DLP-policytips Og](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) [støttematrise for tips for DLP-policy.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="16638-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>