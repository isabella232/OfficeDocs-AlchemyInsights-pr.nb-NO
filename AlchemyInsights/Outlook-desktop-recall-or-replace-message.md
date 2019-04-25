---
title: Outlook stasjonære tilbakekalle eller erstatte en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389741"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="756be-102">Tilbakekalle eller erstatte en e-postmelding</span><span class="sxs-lookup"><span data-stu-id="756be-102">Recall or replace an email message</span></span>

- <span data-ttu-id="756be-103">Som administrator kan du **tilbakekalling av meldinger på vegne av brukere ved hjelp av PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="756be-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="756be-104">Du kan ikke tilbakekalle meldinger fra administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="756be-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="756be-105">Du kan **bare tilbakekalling av meldinger som sendes til personer i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="756be-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="756be-106">Hvis meldingen ble sendt til en Gmail-adresse, for eksempel du kan ikke kalle tilbake den.</span><span class="sxs-lookup"><span data-stu-id="756be-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="756be-107">Du kan **bare tilbakekalling av meldinger sendt fra Outlook-2016 på PCen**.</span><span class="sxs-lookup"><span data-stu-id="756be-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="756be-108">Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på World Wide web, kan du ikke kan huske den.</span><span class="sxs-lookup"><span data-stu-id="756be-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="756be-109">Tilbakekalle eller erstatte en e-postmelding:</span><span class="sxs-lookup"><span data-stu-id="756be-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="756be-110">Velg mappen Sendte elementer i mapper-ruten til venstre i Outlook-vinduet.</span><span class="sxs-lookup"><span data-stu-id="756be-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="756be-111">Dobbeltklikk meldingen du vil kalle tilbake for å åpne den.</span><span class="sxs-lookup"><span data-stu-id="756be-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="756be-112">Velg kategorien **melding** , og velg deretter **Handlinger** > **Kall tilbake denne meldingen**.</span><span class="sxs-lookup"><span data-stu-id="756be-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="756be-113">Velg **Slette uleste kopier av denne meldingen** , eller **Slette uleste kopier og erstatte dem med en ny melding**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="756be-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="756be-114">Hvis du sender en ny melding, meldingen, og deretter velger du **Send**.</span><span class="sxs-lookup"><span data-stu-id="756be-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="756be-115">Vellykket eller mislykket tilbakekalling av en melding, avhengig av mottakerens innstillinger i Outlook.</span><span class="sxs-lookup"><span data-stu-id="756be-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="756be-116">Fremgangsmåte å kontrollere tilbakekalling i [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="756be-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="756be-117">Søke etter og slette e-postmeldinger i organisasjonen</span><span class="sxs-lookup"><span data-stu-id="756be-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="756be-118">Hvis du ikke er en global admin, må kontoen legges til eDiscovery lederrolle eller overholdelse Søk management rollen til å søke etter meldinger.</span><span class="sxs-lookup"><span data-stu-id="756be-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="756be-119">Hvis du vil slette meldinger, må du koble til rollegruppen organisasjon Management eller rollen Søk og Tøm management.</span><span class="sxs-lookup"><span data-stu-id="756be-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="756be-120">Tillatelser for disse rollene tilordnes i [midten av sikkerhet og overholdelse](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="756be-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="756be-121">[Opprett en innhold Søk](https://docs.microsoft.com/office365/securitycompliance/content-search) til å finne meldingen for å slette.</span><span class="sxs-lookup"><span data-stu-id="756be-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="756be-122">[Koble til sikkerhet og overholdelse Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="756be-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="756be-123">Hvis du bruker multifaktorautentisering, kan du se [koble til Office 365-sikkerhet og overholdelse Center PowerShell ved hjelp av multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="756be-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>