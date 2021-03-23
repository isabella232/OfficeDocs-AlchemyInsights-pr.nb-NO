---
title: Varsel AAD Connect
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036106"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="fec6e-102">Varsel AAD Connect</span><span class="sxs-lookup"><span data-stu-id="fec6e-102">Notification AAD Connect</span></span>

- <span data-ttu-id="fec6e-103">Kontroller at du er autorisert til å utføre operasjonen.</span><span class="sxs-lookup"><span data-stu-id="fec6e-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="fec6e-104">Globale administratorer har tilgang som standard.</span><span class="sxs-lookup"><span data-stu-id="fec6e-104">Global Admins have access by default.</span></span> <span data-ttu-id="fec6e-105">I tillegg kan du bruke rollebasert [tilgangskontroll til](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) å delegere registreringstillatelse til bidragsyter.</span><span class="sxs-lookup"><span data-stu-id="fec6e-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="fec6e-106">Kontroller at de nødvendige endepunktene er aktivert, og ikke blokkert på grunn av brannmuren.</span><span class="sxs-lookup"><span data-stu-id="fec6e-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="fec6e-107">Hvis du vil ha mer informasjon, kan du se [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="fec6e-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="fec6e-108">Registreringen kan mislykkes på grunn av at utgående kommunikasjon blir utsatt for SSL-inspeksjon av nettverkslaget.</span><span class="sxs-lookup"><span data-stu-id="fec6e-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="fec6e-109">Kontroller at du har bekreftet varslingsinnstillingene for Azure AD Connect Health og se gjennom innstillingen.</span><span class="sxs-lookup"><span data-stu-id="fec6e-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="fec6e-110">Hvis du vil forstå hvordan du konfigurerer varslingsinnstillingene for Azure AD Connect-tilstandsvarsler, kan du se denne [veiledningen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="fec6e-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="fec6e-111">Hvis du vil lære mer om rapporten om AAD Connect Health-synkronisering og hvordan du laster den ned, kan du se Rapport om synkronisering [på objektnivå](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="fec6e-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="fec6e-112">Hvis du vil feilsøke tilstandsvarsler for AAD Connect, følger du feilsøkingsveiledningen for AAD Connect Health [data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see Common [AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="fec6e-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
