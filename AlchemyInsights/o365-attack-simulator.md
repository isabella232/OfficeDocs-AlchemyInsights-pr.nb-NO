---
title: 2681 Attack Simulator i Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713475"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="0292f-102">Attack Simulator i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0292f-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="0292f-103">Mangler du Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="0292f-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="0292f-104">Attack Simulator krever **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** eller **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="0292f-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="0292f-105">Attack Simulator er **ikke** inkludert i Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 eller noen Microsoft 365 Apps for business-abonnementer.</span><span class="sxs-lookup"><span data-stu-id="0292f-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="0292f-106">Kontoen du bruker til å starte simulerte angrep, krever globale administrator- eller sikkerhetsadministratortillatelser og multifaktorautentisering (MFA).</span><span class="sxs-lookup"><span data-stu-id="0292f-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="0292f-107">Hvis du vil ha mer informasjon om kravene til Attack Simulator, kan du se [dette emnet](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="0292f-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="0292f-108">Viktige ting å vite om **Brute Force Passord** angrep simuleringer:</span><span class="sxs-lookup"><span data-stu-id="0292f-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="0292f-109">Hvis målkontoen har MFA aktivert og passordet ble gjettet riktig, vises ikke kontoen som kompromittert (den andre godkjenningsfaktoren vil være ufullstendig).</span><span class="sxs-lookup"><span data-stu-id="0292f-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="0292f-110">Passordfilen kan ikke være større enn 10 MB.</span><span class="sxs-lookup"><span data-stu-id="0292f-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="0292f-111">Bruk ett passord per linje, og inkluder en tom linje (vognretur) etter det siste passordet i listen.</span><span class="sxs-lookup"><span data-stu-id="0292f-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="0292f-112">Viktige ting å vite om **Spear Phishing** feste simuleringer:</span><span class="sxs-lookup"><span data-stu-id="0292f-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="0292f-113">Etter utforming kan du ikke oppgi en egendefinert verdi for **URL-adressen til phishing-påloggingsserveren**.</span><span class="sxs-lookup"><span data-stu-id="0292f-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="0292f-114">Hvis en mottaker bruker [tillegget Aktiver rapportmelding](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) til å rapportere meldingen som phishing, kan det hende du ikke mottar varsler for meldingen (fordi dette er et simulert angrep).</span><span class="sxs-lookup"><span data-stu-id="0292f-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="0292f-115">Rapporter: Når det simulerte angrepet er fullført, kan du klikke **på Angrepsdetaljer** for å se rapporten.</span><span class="sxs-lookup"><span data-stu-id="0292f-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="0292f-116">Hvis du vil ha detaljerte instruksjoner og nye funksjoner i Attack Simulator, kan du se [Attack Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="0292f-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
