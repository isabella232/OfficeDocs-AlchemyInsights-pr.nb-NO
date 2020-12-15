---
title: Microsoft Edge konfigurere person vern innstillinger
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677797"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="5ffca-102">Microsoft Edge konfigurere person vern innstillinger</span><span class="sxs-lookup"><span data-stu-id="5ffca-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="5ffca-103">Hvis Microsoft Edge distribueres på ikke-Windows-plattformer som standard, sendes ikke diagnose data og område informasjon til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5ffca-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="5ffca-104">Hvis imidlertid Microsoft Edge distribueres på Windows 10, sendes diagnose data og område informasjon i henhold til brukernes [Windows diagnose data innstillinger](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="5ffca-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="5ffca-105">Hvis du vil konfigurere hvordan Microsoft Edge behandler data innsamling for organisasjonen, bruker du følgende gruppe policyer:</span><span class="sxs-lookup"><span data-stu-id="5ffca-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="5ffca-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): denne policyen muliggjør rapportering av bruk og krasj relaterte data.</span><span class="sxs-lookup"><span data-stu-id="5ffca-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="5ffca-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): denne policyen sender nettsteds informasjon som brukes til å forbedre Microsoft-tjenester.</span><span class="sxs-lookup"><span data-stu-id="5ffca-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="5ffca-108">Hvis du vil ha mer informasjon, kan du se [konfigurere policy innstillinger](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="5ffca-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>