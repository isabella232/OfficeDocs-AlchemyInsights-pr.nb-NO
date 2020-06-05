---
title: Fikse Microsoft 365-apper Finner ikke tilknyttet melding om Office-lisenser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580450"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="26a22-102">Fikse Microsoft 365-appene "Finner ikke tilknyttede office-lisenser"</span><span class="sxs-lookup"><span data-stu-id="26a22-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="26a22-103">Hvis du får denne meldingen, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="26a22-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="26a22-104">Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper.</span><span class="sxs-lookup"><span data-stu-id="26a22-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="26a22-105">Se [Url-adresser for Microsoft 365 og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="26a22-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="26a22-106">Fjern og [tilordne Office-lisensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) på nytt for den berørte brukeren.</span><span class="sxs-lookup"><span data-stu-id="26a22-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="26a22-107">Åpne en Office-app, og [logg](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) av eventuelle eksisterende brukerkontoer.</span><span class="sxs-lookup"><span data-stu-id="26a22-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="26a22-108">Gå til Windows-innstillinger > **kontoer**  >  **e-& kontoer**, og fjern alle arbeidskontoer unntatt den berørte kontoen.</span><span class="sxs-lookup"><span data-stu-id="26a22-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="26a22-109">Gå til Windows-innstillinger > **Kontoer**  >  **Få tilgang til arbeid eller skole**, og koble fra alle arbeidskontoer unntatt den berørte kontoen.</span><span class="sxs-lookup"><span data-stu-id="26a22-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="26a22-110">Tilbakestill aktiveringsstatusen for Office.</span><span class="sxs-lookup"><span data-stu-id="26a22-110">Reset the Office activation state.</span></span> <span data-ttu-id="26a22-111">[Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="26a22-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="26a22-112">[Logg på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte brukerkontoen.</span><span class="sxs-lookup"><span data-stu-id="26a22-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="26a22-113">Hvis du vil ha flere feilsøkingsløsninger, kan du se [Ulisensiert produkt- og aktiveringsfeil i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="26a22-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>