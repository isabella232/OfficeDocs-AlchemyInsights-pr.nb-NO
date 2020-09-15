---
title: Skrive bords kall fra Outlook eller erstatte en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663999"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="b4991-102">Tilbakekalle eller erstatte en e-postmelding i Outlook</span><span class="sxs-lookup"><span data-stu-id="b4991-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="b4991-103">Som administrator kan du **tilbakekalle meldinger på vegne av brukere som bruker PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="b4991-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="b4991-104">Du kan ikke tilbakekalle meldinger fra administrasjons senteret.</span><span class="sxs-lookup"><span data-stu-id="b4991-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="b4991-105">Du kan **bare tilbakekalle meldinger som sendes til personer i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="b4991-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="b4991-106">Hvis meldingen for eksempel ble sendt til en Gmail-adresse, kan du ikke tilbakekalle den.</span><span class="sxs-lookup"><span data-stu-id="b4991-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="b4991-107">Du kan **bare tilbakekalle meldinger som er sendt fra Outlook 2016 på PC-en**.</span><span class="sxs-lookup"><span data-stu-id="b4991-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="b4991-108">Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke tilbakekalle den.</span><span class="sxs-lookup"><span data-stu-id="b4991-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="b4991-109">Slik tilbakekaller eller erstatter du en e-postmelding:</span><span class="sxs-lookup"><span data-stu-id="b4991-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="b4991-110">Velg sendte elementer-mappen i mappe ruten til venstre i Outlook-vinduet.</span><span class="sxs-lookup"><span data-stu-id="b4991-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="b4991-111">Dobbelt Klikk meldingen du vil kalle tilbake for å åpne den.</span><span class="sxs-lookup"><span data-stu-id="b4991-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="b4991-112">Velg **melding** -fanen, og velg deretter **handlinger**for å  >  **tilbakekalle denne meldingen**.</span><span class="sxs-lookup"><span data-stu-id="b4991-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="b4991-113">Velg **Slett uleste kopier av denne meldingen** , eller **Slett uleste kopier og Erstatt med en ny melding**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="b4991-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="b4991-114">Hvis du sender en erstatnings melding, skriver du meldingen, og deretter velger du **Send**.</span><span class="sxs-lookup"><span data-stu-id="b4991-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="b4991-115">Om en tilbake melding er vellykket eller mislykket, avhenger av mottakerens innstillinger i Outlook.</span><span class="sxs-lookup"><span data-stu-id="b4991-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="b4991-116">Hvis du vil ha informasjon om hvordan du sjekker tilbake kallingen, kan du se [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="b4991-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="b4991-117">Søke etter og slette e-postmeldinger i organisasjonen</span><span class="sxs-lookup"><span data-stu-id="b4991-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="b4991-118">Hvis du ikke er en global administrator, må kontoen legges til i rollen for administrasjon av eDiscovery-administrator og søke etter meldinger.</span><span class="sxs-lookup"><span data-stu-id="b4991-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="b4991-119">Hvis du vil slette meldinger, må du bli med i rolle gruppen organisasjons behandling eller søke og fjerne administrasjons rollen.</span><span class="sxs-lookup"><span data-stu-id="b4991-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="b4991-120">Tillatelser for disse rollene er tilordnet i [sikkerhets-og samsvars senteret](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="b4991-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="b4991-121">[Opprett et innholds søk](https://docs.microsoft.com/microsoft-365/compliance/content-search) for å finne meldingen som skal slettes.</span><span class="sxs-lookup"><span data-stu-id="b4991-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="b4991-122">[Koble til sikkerhets-og samsvars senteret PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b4991-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="b4991-123">Hvis du bruker godkjenning med flere faktorer, kan du se [Koble til Microsoft 365 Security and revisjons senteret PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="b4991-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>