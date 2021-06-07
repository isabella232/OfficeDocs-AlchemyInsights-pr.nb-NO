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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798689"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="4da6b-102">Kan ikke aktivere Office</span><span class="sxs-lookup"><span data-stu-id="4da6b-102">Unable to activate Office</span></span>

<span data-ttu-id="4da6b-103">**Obs!** Hvis du bruker en eldre versjon av Windows (for eksempel Windows 7), må du kontrollere at TLS 1.2 er aktivert som standard.</span><span class="sxs-lookup"><span data-stu-id="4da6b-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="4da6b-104">Hvis du vil ha mer informasjon, kan du se Oppdatere for å aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP i Windows .</span><span class="sxs-lookup"><span data-stu-id="4da6b-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="4da6b-105">Kontroller om abonnementet har utløpt.</span><span class="sxs-lookup"><span data-stu-id="4da6b-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="4da6b-106">Kontroller at du har et abonnement som tillater klientlisenser, som for eksempel Office 365 Business eller Business Premium, og [kontroller at brukeren har en tilordnet lisens](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="4da6b-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="4da6b-107">Forsikre deg om at brukeren logger på Office med samme konto som lisensen er tildelt til.</span><span class="sxs-lookup"><span data-stu-id="4da6b-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="4da6b-108">Sjekk [siden for Office 365-tjenestetilstand](/office365/enterprise/view-service-health) for å se om det finnes kjente problemer med tjenesten.</span><span class="sxs-lookup"><span data-stu-id="4da6b-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="4da6b-109">Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Microsoft 365-apper sin tilgang til internett.</span><span class="sxs-lookup"><span data-stu-id="4da6b-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="4da6b-110">Se [URL-adresser og IP-adresseområder for Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL-adresser og IP-adresseområder for Office 365").</span><span class="sxs-lookup"><span data-stu-id="4da6b-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="4da6b-111">**Tips** På Windows-maskiner kan vi diagnostisere og ordne flere vanlige problemer med pålogging til Office for deg.</span><span class="sxs-lookup"><span data-stu-id="4da6b-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="4da6b-112">Last ned og kjør **[assistent for støtte og gjenoppretting](https://aka.ms/SaRA-OfficeSignInScenario)** for å bruke vårt automatiserte verktøy.</span><span class="sxs-lookup"><span data-stu-id="4da6b-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="4da6b-113">Bruk følgende feilsøkingshandlinger:</span><span class="sxs-lookup"><span data-stu-id="4da6b-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="4da6b-114">Åpne et Office-program og [logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eksisterende brukerkontoer.</span><span class="sxs-lookup"><span data-stu-id="4da6b-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="4da6b-115">[Fjern](/microsoft-365/admin/manage/remove-licenses-from-users) og [tilordne](/microsoft-365/admin/manage/assign-licenses-to-users) Office-lisens på nytt, og deretter [logge på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ved hjelp av den berørte brukerkontoen.</span><span class="sxs-lookup"><span data-stu-id="4da6b-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="4da6b-116">Kjør feilsøkingsverktøyet for [Aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="4da6b-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="4da6b-117">Tilbakestill aktiveringsstatusen for Office</span><span class="sxs-lookup"><span data-stu-id="4da6b-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Tilbakestill aktiveringsstatusen for Office")
- [<span data-ttu-id="4da6b-118">Utfør en Tilkoblet reparasjon av Office</span><span class="sxs-lookup"><span data-stu-id="4da6b-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="4da6b-119">Hvis du trenger ytterligere feilsøkingsløsninger, kan du se:</span><span class="sxs-lookup"><span data-stu-id="4da6b-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="4da6b-120">Feil ved ulisensiert produkt og aktivering i Office</span><span class="sxs-lookup"><span data-stu-id="4da6b-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="4da6b-121">«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere»-feil når du aktiverer Office</span><span class="sxs-lookup"><span data-stu-id="4da6b-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)