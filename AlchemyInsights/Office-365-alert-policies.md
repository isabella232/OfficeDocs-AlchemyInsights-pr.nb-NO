---
title: 1385-Office-365-varslings policyer
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664035"
---
# <a name="alert-policies"></a><span data-ttu-id="bfccd-102">Varslings policyer</span><span class="sxs-lookup"><span data-stu-id="bfccd-102">Alert policies</span></span>

<span data-ttu-id="bfccd-103">Samsvars senteret for sikkerhets & i Microsoft 365 tilbyr [standard varslings policyer](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) som utløser varsler for organisasjoner med en Office 365 Enterprise-eller office-365 for eksempel offentlige E1-/G1-, E3/G3-eller E5/G5-abonnement.</span><span class="sxs-lookup"><span data-stu-id="bfccd-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="bfccd-104">Derfor kan det hende at administratorer mottar varsler om e-post sendt av Office365Alerts@microsoft.com med en Emne linje, for eksempel et lav Alvors varsel: *navn på varsel policy*.</span><span class="sxs-lookup"><span data-stu-id="bfccd-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="bfccd-105">Varsel varsler sendes når varsler utløses for vanlige aktiviteter, for eksempel når brukere:</span><span class="sxs-lookup"><span data-stu-id="bfccd-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="bfccd-106">Opprette regler for innboksen som videre sender e-post.</span><span class="sxs-lookup"><span data-stu-id="bfccd-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="bfccd-107">Tilordne tillatelser til post boksen.</span><span class="sxs-lookup"><span data-stu-id="bfccd-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="bfccd-108">Dele eller slette et stort antall filer i fil deling i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bfccd-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="bfccd-109">Opprette eDiscovery-søk og eksportere søke resultater.</span><span class="sxs-lookup"><span data-stu-id="bfccd-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="bfccd-110">Slik kan du se gjennom og handle på et varsel:</span><span class="sxs-lookup"><span data-stu-id="bfccd-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="bfccd-111">Gå til [sikkerhets & samsvars senter](https://protection.office.com) , og Logg på.</span><span class="sxs-lookup"><span data-stu-id="bfccd-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="bfccd-112">Klikk **varsler**  >  **Vis varsler**.</span><span class="sxs-lookup"><span data-stu-id="bfccd-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="bfccd-113">Klikk et varsel for å vise en under meny med informasjon om varselet.</span><span class="sxs-lookup"><span data-stu-id="bfccd-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="bfccd-114">Du kan gjøre noe med et varsel, for eksempel ved å [fjerne en mistenkelig målregel](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="bfccd-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="bfccd-115">Eller du kan ganske enkelt lukke varselet ved å klikke på **løs** på under menyen varsel.</span><span class="sxs-lookup"><span data-stu-id="bfccd-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="bfccd-116">Hvis du vil ha mer informasjon om konfigurasjon og behandling av varslings policyer, kan du se  [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="bfccd-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="bfccd-117">**Viktig**: varsle e-postvarsler fra Microsoft vil aldri be deg om å gjøre følgende:</span><span class="sxs-lookup"><span data-stu-id="bfccd-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="bfccd-118">Angi et passord</span><span class="sxs-lookup"><span data-stu-id="bfccd-118">Provide a password</span></span>
- <span data-ttu-id="bfccd-119">Kontroller sikkerhets detaljene for kontoen din</span><span class="sxs-lookup"><span data-stu-id="bfccd-119">Verify the security details of your account</span></span>
- <span data-ttu-id="bfccd-120">Godkjenn på nytt selv</span><span class="sxs-lookup"><span data-stu-id="bfccd-120">Re-authenticate yourself</span></span>

<span data-ttu-id="bfccd-121">Hvis du mottar en e-postmelding som dette, ble den ikke sendt av Microsoft og bør anses som en phishing-svindel.</span><span class="sxs-lookup"><span data-stu-id="bfccd-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="bfccd-122">Hvis dette skjer, kan du [rapportere den til Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="bfccd-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>