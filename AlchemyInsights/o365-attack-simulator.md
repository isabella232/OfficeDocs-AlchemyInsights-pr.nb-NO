---
title: 2681 Attack Simulator i Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545735"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="5825f-102">Angrepssimulator i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5825f-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="5825f-103">Mangler du Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="5825f-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="5825f-104">Attack Simulator krever **Microsoft Defender for Office 365 Plan 2** **eller Office 365 Enterprise E5.**</span><span class="sxs-lookup"><span data-stu-id="5825f-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="5825f-105">Attack Simulator er **ikke** inkludert i Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3 eller Microsoft 365 Apps for business abonnementer.</span><span class="sxs-lookup"><span data-stu-id="5825f-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="5825f-106">Kontoen du bruker til å starte simulerte angrep, krever globale administrator- eller sikkerhetsadministratortillatelser og godkjenning med flere faktorer (MFA).</span><span class="sxs-lookup"><span data-stu-id="5825f-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="5825f-107">Hvis du vil ha mer informasjon om angrepssimulatorkrav, kan du [se dette emnet](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="5825f-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="5825f-108">Viktige ting du må vite om **Angrepssimuleringer for Brute Force-passord:**</span><span class="sxs-lookup"><span data-stu-id="5825f-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="5825f-109">Hvis målkontoen har aktivert MFA og passordet ble gjettet riktig, vises ikke kontoen som kompromittert (den andre godkjenningsfaktoren vil være ufullstendig).</span><span class="sxs-lookup"><span data-stu-id="5825f-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="5825f-110">Passordfilen kan ikke være større enn 10 MB.</span><span class="sxs-lookup"><span data-stu-id="5825f-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="5825f-111">Bruk ett passord per linje, og inkluder en tom linje (retur) etter det siste passordet i listen.</span><span class="sxs-lookup"><span data-stu-id="5825f-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="5825f-112">Viktige ting du må vite om å legge ved **simulasjoner for Phishing-phishing:**</span><span class="sxs-lookup"><span data-stu-id="5825f-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="5825f-113">Som utforming kan du ikke angi en egendefinert verdi for nettadressen for **phishing-påloggingsserveren**.</span><span class="sxs-lookup"><span data-stu-id="5825f-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="5825f-114">Hvis en mottaker bruker [tillegget](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Aktiver rapportmelding til å rapportere meldingen som phishing, mottar du kanskje ikke varsler for meldingen (fordi dette er et simulert angrep).</span><span class="sxs-lookup"><span data-stu-id="5825f-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="5825f-115">Rapporter: Når det simulerte angrepet er fullført, kan du klikke **Angrepsdetaljer** for å se rapporten.</span><span class="sxs-lookup"><span data-stu-id="5825f-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="5825f-116">Hvis du vil ha detaljerte instruksjoner og nye funksjoner i Attack Simulator, kan du se [Angrepssimulator i Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="5825f-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
