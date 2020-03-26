---
title: Kan ikke logge på Teams på grunn av en feil autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932037"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="89057-102">Kan ikke logge på Teams på grunn av en feil autologon.microsoftazuread-sso dot.com:443</span><span class="sxs-lookup"><span data-stu-id="89057-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="89057-103">Hvis sømløst SSO er aktivert som O365-godkjenning, må kanskje URL-adressen «autologon.microsoftazuread-sso.com» bli lagt til i intranettområdene også.</span><span class="sxs-lookup"><span data-stu-id="89057-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="89057-104">Hvis den tidligere har blitt lagt til i klarerte områder og sømløst SSO er i bruk, bør den fjernes fra klarerte områder.</span><span class="sxs-lookup"><span data-stu-id="89057-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="89057-105">Hvis du vil ha mer informasjon, kan du gå igjennom [Sømløs kontrollliste for feilsøking av SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="89057-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="89057-106">Følg disse trinnene for å legge til en URL-adresse i listen over intranett områder:</span><span class="sxs-lookup"><span data-stu-id="89057-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="89057-107">Åpne Internet Explorer ved å klikke på **Start**-knappen.</span><span class="sxs-lookup"><span data-stu-id="89057-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="89057-108">I søkeboksen skriver du inn Internet Explorer, og deretter klikker du **Internet Explorer**i resultatlisten.</span><span class="sxs-lookup"><span data-stu-id="89057-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="89057-109">I **Verktøy**-menyen klikker du så på **Alternativer for Internett**.</span><span class="sxs-lookup"><span data-stu-id="89057-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="89057-110">Velg fanen for **Sikkerhet**.</span><span class="sxs-lookup"><span data-stu-id="89057-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="89057-111">Nå klikker du på **Lokale intranettområder** før du deretter klikker på **områder**-knappen og deretter **Avansert**-knappen.</span><span class="sxs-lookup"><span data-stu-id="89057-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="89057-112">Skriv inn URL-adressen til webområdet, og klikk **Legg til**.</span><span class="sxs-lookup"><span data-stu-id="89057-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="89057-113">Når du er ferdig, klikker du på **Lukk**.</span><span class="sxs-lookup"><span data-stu-id="89057-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="89057-114">Hvis du vil ha mer informasjon, kan du ta en titt på [Dokumentasjon for å distribuere sømløst SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inkluderer policybasert prosess for å legge til en URL-adresse i intranettområder i trinn 3).</span><span class="sxs-lookup"><span data-stu-id="89057-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
