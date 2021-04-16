---
title: Kan ikke aktivere Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812581"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="df320-102">Kan ikke aktivere Office</span><span class="sxs-lookup"><span data-stu-id="df320-102">Unable to activate Office</span></span>

- <span data-ttu-id="df320-103">Kontroller om abonnementet har utløpt.</span><span class="sxs-lookup"><span data-stu-id="df320-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="df320-104">Kontroller at du har et abonnement som tillater klientlisenser, som for eksempel Office 365 Business eller Business Premium, og [kontroller at brukeren har en tilordnet lisens](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="df320-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="df320-105">Forsikre deg om at brukeren logger på Office med samme konto som lisensen er tildelt til.</span><span class="sxs-lookup"><span data-stu-id="df320-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="df320-106">Sjekk [siden for Office 365-tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for å se om det finnes kjente problemer med tjenesten.</span><span class="sxs-lookup"><span data-stu-id="df320-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="df320-107">Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Microsoft 365-apper sin tilgang til internett.</span><span class="sxs-lookup"><span data-stu-id="df320-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="df320-108">Se [URL-adresser og IP-adresseområder for Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-adresser og IP-adresseområder for Office 365").</span><span class="sxs-lookup"><span data-stu-id="df320-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="df320-109">**Tips** På Windows-maskiner kan vi diagnostisere og ordne flere vanlige problemer med pålogging til Office for deg.</span><span class="sxs-lookup"><span data-stu-id="df320-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="df320-110">Last ned og kjør **[assistent for støtte og gjenoppretting](https://aka.ms/SaRA-OfficeSignInScenario)** for å bruke vårt automatiserte verktøy.</span><span class="sxs-lookup"><span data-stu-id="df320-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="df320-111">Bruk følgende feilsøkingshandlinger:</span><span class="sxs-lookup"><span data-stu-id="df320-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="df320-112">Åpne et Office-program og [logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eksisterende brukerkontoer.</span><span class="sxs-lookup"><span data-stu-id="df320-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="df320-113">[Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [tilordne](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-lisens på nytt, og deretter [logge på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ved hjelp av den berørte brukerkontoen.</span><span class="sxs-lookup"><span data-stu-id="df320-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="df320-114">Kjør feilsøkingsverktøyet for [Aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="df320-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="df320-115">Tilbakestill aktiveringsstatusen for Office</span><span class="sxs-lookup"><span data-stu-id="df320-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Tilbakestill aktiveringsstatusen for Office")
- [<span data-ttu-id="df320-116">Utfør en Tilkoblet reparasjon av Office</span><span class="sxs-lookup"><span data-stu-id="df320-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="df320-117">Hvis du trenger ytterligere feilsøkingsløsninger, kan du se:</span><span class="sxs-lookup"><span data-stu-id="df320-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="df320-118">Feil ved ulisensiert produkt og aktivering i Office</span><span class="sxs-lookup"><span data-stu-id="df320-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="df320-119">«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere»-feil når du aktiverer Office</span><span class="sxs-lookup"><span data-stu-id="df320-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)