---
title: Kalender ikonet vises ikke i Microsoft Teams-klienten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583921"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="ce3b3-102">Kalender ikonet vises ikke i Microsoft Teams-klienten</span><span class="sxs-lookup"><span data-stu-id="ce3b3-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="ce3b3-103">Kategorien **Kalender** i Teams krever tilgang til en Exchange-postboks via Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="ce3b3-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="ce3b3-104">Exchange-postboksen kan være tilkoblet eller lokalt.</span><span class="sxs-lookup"><span data-stu-id="ce3b3-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="ce3b3-105">For brukere på nettet som ikke ser **Kalender** -fanen, må du kontrollere at de [er lisensiert for en Exchange Online-postboks og at post boksen er aktivert](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="ce3b3-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="ce3b3-106">Hvis brukerne dine er privat lokalt, må du bekrefte at hybrid konfigurasjonen er OK.</span><span class="sxs-lookup"><span data-stu-id="ce3b3-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="ce3b3-107">Bruk [Veiviseren for hybridkonfigurasjon](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) for å feilsøke.</span><span class="sxs-lookup"><span data-stu-id="ce3b3-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="ce3b3-108">Vær obs på at [Teams krever Exchange 2016 CU3 eller nyere](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="ce3b3-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="ce3b3-109">Hvis du vil ha mer informasjon og feil søkings trinn, kan du se [Feilsøke problemer med Microsoft Teams og Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="ce3b3-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
