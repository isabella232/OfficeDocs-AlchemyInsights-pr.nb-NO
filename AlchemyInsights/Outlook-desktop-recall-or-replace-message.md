---
title: Tilbakekalling av Outlook-skrivebord eller erstatt en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687519"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="3660a-102">Tilbakekalle eller erstatte en Outlook-e-postmelding</span><span class="sxs-lookup"><span data-stu-id="3660a-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="3660a-103">Som administrator kan du **tilbakekalle meldinger på vegne av brukere som bruker PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="3660a-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="3660a-104">Du kan ikke hente meldinger fra administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="3660a-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="3660a-105">Du kan **bare hente meldinger som sendes til personer i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="3660a-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="3660a-106">Hvis meldingen ble sendt til en Gmail-adresse, kan du for eksempel ikke huske den.</span><span class="sxs-lookup"><span data-stu-id="3660a-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="3660a-107">Du kan **bare hente meldinger som sendes fra Outlook-2016 på PCen**.</span><span class="sxs-lookup"><span data-stu-id="3660a-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="3660a-108">Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på nettet, kan du ikke huske den.</span><span class="sxs-lookup"><span data-stu-id="3660a-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="3660a-109">Slik tilbakekaller eller erstatter du en e-postmelding:</span><span class="sxs-lookup"><span data-stu-id="3660a-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="3660a-110">Velg Mappen Sendte elementer i mapperuten til venstre i Outlook-vinduet.</span><span class="sxs-lookup"><span data-stu-id="3660a-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="3660a-111">Dobbeltklikk meldingen du vil huske for å åpne den.</span><span class="sxs-lookup"><span data-stu-id="3660a-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="3660a-112">Velg **kategorien Melding,** og velg deretter **Handlinger** > **tilbakekall denne meldingen**.</span><span class="sxs-lookup"><span data-stu-id="3660a-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="3660a-113">Velg **Slett uleste kopier av denne meldingen** eller Slett **uleste kopier, og erstatt med en ny melding**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="3660a-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="3660a-114">Hvis du sender en erstatningsmelding, skriver du meldingen, og deretter velger du **Send**.</span><span class="sxs-lookup"><span data-stu-id="3660a-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="3660a-115">Vellykket eller mislykket tilbakekalling av en melding avhenger av mottakerens innstillinger i Outlook.</span><span class="sxs-lookup"><span data-stu-id="3660a-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="3660a-116">Hvis du vil ha trinn for å se om tilbakekallingen, kan du se [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="3660a-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="3660a-117">Søke etter og slette e-postmeldinger i organisasjonen</span><span class="sxs-lookup"><span data-stu-id="3660a-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="3660a-118">Hvis du ikke er global administrator, må kontoen din legges til i rollen eDiscovery Manager eller rollen for administrasjon av samsvarsøk for å søke etter meldinger.</span><span class="sxs-lookup"><span data-stu-id="3660a-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="3660a-119">Hvis du vil slette meldinger, må du bli med i rollegruppen Organisasjonsstyring eller rollen Administrasjon for søk og tømming.</span><span class="sxs-lookup"><span data-stu-id="3660a-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="3660a-120">Tillatelser for disse rollene tilordnes i [sikkerhets- og samsvarssenteret](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="3660a-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="3660a-121">[Opprett et innholdssøk](https://docs.microsoft.com/office365/securitycompliance/content-search) for å finne meldingen som skal slettes.</span><span class="sxs-lookup"><span data-stu-id="3660a-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="3660a-122">[Koble til Sikkerhets- og samsvarssenter PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="3660a-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="3660a-123">Hvis du bruker godkjenning med flere faktorer, kan du se [Koble til Microsoft 365-sikkerhet og samsvarssenter PowerShell ved hjelp av godkjenning med flere faktorer](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="3660a-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>