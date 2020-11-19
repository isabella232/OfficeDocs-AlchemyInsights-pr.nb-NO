---
title: Kalle tilbake eller erstatte en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353515"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="1bd56-102">Kalle tilbake eller erstatte en e-postmelding i Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1bd56-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="1bd56-103">Du kan **bare tilbakekalle meldinger som sendes til personer i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="1bd56-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="1bd56-104">Hvis meldingen for eksempel ble sendt til en Gmail-adresse, kan du ikke tilbakekalle den.</span><span class="sxs-lookup"><span data-stu-id="1bd56-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="1bd56-105">Du kan **bare tilbakekalle meldinger som er sendt fra Outlook for PC-en**.</span><span class="sxs-lookup"><span data-stu-id="1bd56-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="1bd56-106">Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke tilbakekalle den.</span><span class="sxs-lookup"><span data-stu-id="1bd56-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="1bd56-107">Som leier administrator kan du **tilbakekalle meldinger på vegne av brukere ved hjelp av PowerShell** (Hvis du vil ha mer informasjon, se: [søke etter og slette e-postmeldinger](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="1bd56-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="1bd56-108">Du kan ikke tilbakekalle meldinger fra administrasjons senteret.</span><span class="sxs-lookup"><span data-stu-id="1bd56-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="1bd56-109">Rull ned til søk etter og slett e-postmeldinger i organisasjonen for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="1bd56-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="1bd56-110">**Tilbakekalle eller erstatte en e-postmelding du har sendt**</span><span class="sxs-lookup"><span data-stu-id="1bd56-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="1bd56-111">I mappe ruten til venstre i Outlook-vinduet velger du sendte elementer-mappen.</span><span class="sxs-lookup"><span data-stu-id="1bd56-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="1bd56-112">Åpne meldingen du vil kalle tilbake.</span><span class="sxs-lookup"><span data-stu-id="1bd56-112">Open the message that you want to recall.</span></span> <span data-ttu-id="1bd56-113">Du må dobbeltklikke for å åpne meldingen.</span><span class="sxs-lookup"><span data-stu-id="1bd56-113">You must double-click to open the message.</span></span> <span data-ttu-id="1bd56-114">Hvis du velger meldingen slik at den vises i lese ruten, kan du ikke kalle tilbake meldingen.</span><span class="sxs-lookup"><span data-stu-id="1bd56-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="1bd56-115">På melding-fanen velger du **handlinger** for å  >  **tilbakekalle denne meldingen**.</span><span class="sxs-lookup"><span data-stu-id="1bd56-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="1bd56-116">Velg **Slett uleste kopier av denne meldingen** , eller **Slett uleste kopier og Erstatt med en ny melding**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="1bd56-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="1bd56-117">Hvis du sender en erstatnings melding, skriver du meldingen og velger **Send**.</span><span class="sxs-lookup"><span data-stu-id="1bd56-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="1bd56-118">Mottakerens innstillinger i Outlook er vellykket eller mislykket tilbake kalling av meldingen.</span><span class="sxs-lookup"><span data-stu-id="1bd56-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="1bd56-119">Hvis du vil ha mer informasjon, inkludert hvordan du sjekker tilbake kallingen, kan [du se kalle tilbake eller erstatte en e-postmelding du har sendt](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="1bd56-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="1bd56-120">Hvis du **_vil søke etter og slette e-postmeldinger i organisasjonen_**, er det enklest hvis du er en global administrator. Hvis du ikke er global administrator, må kontoen legges til i rolle gruppen eDiscovery Manager, eller i rollen som søke behandling for samsvar.</span><span class="sxs-lookup"><span data-stu-id="1bd56-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="1bd56-121">Hvis du vil slette meldinger, må du bli med i rolle gruppen organisasjons behandling eller søke og fjerne administrasjons rollen.</span><span class="sxs-lookup"><span data-stu-id="1bd56-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="1bd56-122">Tillatelser til disse rollene er tilordnet i [sikkerhets & samsvars senteret](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="1bd56-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="1bd56-123">[Opprett et innholds søk](https://docs.microsoft.com/microsoft-365/compliance/content-search) for å finne meldingen som skal slettes.</span><span class="sxs-lookup"><span data-stu-id="1bd56-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="1bd56-124">[Koble til sikkerhets & samsvars senteret PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="1bd56-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="1bd56-125">Hvis du bruker MFA (godkjenning med flere faktorer), kan du se [Koble til Microsoft 365 sikkerhets & samsvars senteret PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="1bd56-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
