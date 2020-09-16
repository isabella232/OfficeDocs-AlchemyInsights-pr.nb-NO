---
title: Løse ulisensiert produkt-feil
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737962"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="801f2-102">Forslag til å løse feil i «ulisensiert produkt»</span><span class="sxs-lookup"><span data-stu-id="801f2-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="801f2-103">Hvis du vil løse feil om et "ulisensiert produkt", kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="801f2-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="801f2-104">Kontroller om abonnements statusen er utløpt.</span><span class="sxs-lookup"><span data-stu-id="801f2-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="801f2-105">Kontroller at du har et abonnement som tillater klient lisenser, for eksempel Microsoft 365-apper for Business eller Business Premium, og [at brukeren har en lisens som er tilordnet](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="801f2-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="801f2-106">Kontroller at brukeren logger på Office med den samme kontoen som er tilordnet lisensen.</span><span class="sxs-lookup"><span data-stu-id="801f2-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="801f2-107">Kontroller [tjeneste tilstands IDen](https://docs.microsoft.com/office365/enterprise/view-service-health) for å se om det er noen kjente problemer med tjenesten.</span><span class="sxs-lookup"><span data-stu-id="801f2-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="801f2-108">Kontroller brann muren, antivirus program varen og proxy-innstillingene for å bekrefte at de ikke blokkerer Microsoft 365-apper tilgang til Internet t.</span><span class="sxs-lookup"><span data-stu-id="801f2-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="801f2-109">Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="801f2-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="801f2-110">Du kan også prøve følgende feil søkings handlinger:</span><span class="sxs-lookup"><span data-stu-id="801f2-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="801f2-111">Åpne en Office-app og [Logg](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) av eksisterende bruker kontoer.</span><span class="sxs-lookup"><span data-stu-id="801f2-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="801f2-112">[Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [Tilordne Office-](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) lisensen på nytt, og [Logg deg](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) deretter på Office ved hjelp av den berørte bruker kontoen.</span><span class="sxs-lookup"><span data-stu-id="801f2-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="801f2-113">Kjør [feil søkings verktøyet for aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="801f2-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="801f2-114">[Tilbakestill aktiveringsstatusen for Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="801f2-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="801f2-115">[Utføre en tilkoblet reparasjon av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="801f2-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="801f2-116">Hvis du trenger ytterligere feilsøkingsløsninger, kan du se:</span><span class="sxs-lookup"><span data-stu-id="801f2-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="801f2-117">Feil ved ulisensiert produkt og aktivering i Office</span><span class="sxs-lookup"><span data-stu-id="801f2-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="801f2-118">«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere»-feil når du aktiverer Office</span><span class="sxs-lookup"><span data-stu-id="801f2-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)