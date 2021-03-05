---
title: Problem med AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482072"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="54443-102">Problem med AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="54443-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="54443-103">Kontroller at du er autorisert til å utføre operasjonen.</span><span class="sxs-lookup"><span data-stu-id="54443-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="54443-104">Globale administratorer har tilgang som standard.</span><span class="sxs-lookup"><span data-stu-id="54443-104">Global Admins have access by default.</span></span> <span data-ttu-id="54443-105">I tillegg kan du bruke [rollebasert](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) tilgangskontroll til å delegere registreringstillatelse til Bidragsyter.</span><span class="sxs-lookup"><span data-stu-id="54443-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="54443-106">Sikre at de nødvendige endepunktene er aktivert, og at de ikke blokkeres på grunn av brannmuren.</span><span class="sxs-lookup"><span data-stu-id="54443-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="54443-107">Hvis du vil ha mer informasjon, kan du [se krav.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="54443-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="54443-108">Registrering kan mislykkes på grunn av at utgående kommunikasjon er underlagt SSL-inspeksjon av nettverkslaget.</span><span class="sxs-lookup"><span data-stu-id="54443-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="54443-109">Kontroller at du har bekreftet varslingsinnstillingene for Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="54443-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="54443-110">Se gjennom innstillingen.</span><span class="sxs-lookup"><span data-stu-id="54443-110">Please review your setting.</span></span> <span data-ttu-id="54443-111">Denne [veiledningen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) kan hjelpe deg med å forstå hvordan du konfigurerer varslingsinnstillingene for azure AD Connect-tilstandsvarsler.</span><span class="sxs-lookup"><span data-stu-id="54443-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="54443-112">Hvis du vil lære mer om rapporten om AAD Connect-tilstandssynkronisering og hvordan du laster den ned, kan du se [synkroniseringsrapport på objektnivå.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="54443-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="54443-113">Hvis du vil feilsøke tilstandsvarsler for AAD Connect, kan du følge feilsøkingsveiledningen for varsler om tilstandsoppdretting for [AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Health og se vanlige spørsmål om [AAD Connect Health-installasjon.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="54443-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
