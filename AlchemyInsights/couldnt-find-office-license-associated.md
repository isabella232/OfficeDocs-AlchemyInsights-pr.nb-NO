---
title: Reparere Microsoft 365-apper Finner ikke tilknyttede office-lisenser
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816497"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="16717-102">Melding om at Microsoft 365-appene «Finner ikke tilknyttede office-lisenser»</span><span class="sxs-lookup"><span data-stu-id="16717-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="16717-103">Hvis du mottar denne meldingen, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="16717-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="16717-104">Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper.</span><span class="sxs-lookup"><span data-stu-id="16717-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="16717-105">Se [Nettadresser og IP-adresseområder for Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="16717-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="16717-106">Fjern og [tilordne Office-lisensen på nytt](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for den berørte brukeren.</span><span class="sxs-lookup"><span data-stu-id="16717-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="16717-107">Åpne en Office-app, [og logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eventuelle eksisterende brukerkontoer.</span><span class="sxs-lookup"><span data-stu-id="16717-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="16717-108">Gå til Windows-innstillinger > **kontoer**& kontoer , og fjern  >  alle jobbkontoer unntatt den berørte kontoen.</span><span class="sxs-lookup"><span data-stu-id="16717-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="16717-109">Gå til Windows-innstillinger > **Kontoer** Tilgang til jobb eller skole , og koble fra  >  alle jobbkontoer unntatt den berørte kontoen.</span><span class="sxs-lookup"><span data-stu-id="16717-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="16717-110">Tilbakestill aktiveringsstatusen for Office.</span><span class="sxs-lookup"><span data-stu-id="16717-110">Reset the Office activation state.</span></span> <span data-ttu-id="16717-111">[Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="16717-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="16717-112">[Logg på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte brukerkontoen.</span><span class="sxs-lookup"><span data-stu-id="16717-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="16717-113">Hvis du vil ha flere feilsøkingsløsninger, kan du [se Ulisensiert produkt og aktiveringsfeil i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="16717-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>