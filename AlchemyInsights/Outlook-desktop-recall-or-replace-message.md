---
title: Outlook desktop tilbakekalle eller erstatte en e-postmelding
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496120"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="ff2c9-102">Tilbakekalle eller erstatte en Outlook-e-postmelding</span><span class="sxs-lookup"><span data-stu-id="ff2c9-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="ff2c9-103">Som administrator kan du **tilbakekalle meldinger på vegne av brukere som bruker PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="ff2c9-104">Du kan ikke tilbakekalle meldinger fra administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="ff2c9-105">Du kan **bare tilbakekalle meldinger som er sendt til personer i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ff2c9-106">Hvis meldingen for eksempel ble sendt til en Gmail-adresse, kan du ikke huske den.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="ff2c9-107">Du kan **bare tilbakekalle meldinger som er sendt fra Outlook 2016 på PC**-en.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="ff2c9-108">Hvis en bruker sender en melding ved hjelp av Outlook for Mac eller Outlook på weben, kan du ikke tilbakekalle den.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="ff2c9-109">Slik tilbakekaller eller erstatter du en e-postmelding:</span><span class="sxs-lookup"><span data-stu-id="ff2c9-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="ff2c9-110">I mapperuten til venstre i Outlook-vinduet velger du sendte elementer-mappen.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="ff2c9-111">Dobbeltklikk meldingen du vil tilbakekalle, for å åpne den.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="ff2c9-112">Velg kategorien **melding** , og velg deretter **handlinger** > **tilbakekall denne meldingen**.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="ff2c9-113">Velg **Slett uleste kopier av denne meldingen** eller **Slett uleste kopier og Erstatt med en ny melding**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="ff2c9-114">Hvis du skal sende en ny melding, skriver du meldingen og velger **Send**.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="ff2c9-115">Mottakerens innstillinger i Outlook er vellykket eller mislykket av en tilbakekalling av melding.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="ff2c9-116">Hvis du vil ha trinn for hvordan du ser tilbakekallingen, kan du se [denne artikkelen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="ff2c9-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ff2c9-117">Søke etter og slette e-postmeldinger i organisasjonen</span><span class="sxs-lookup"><span data-stu-id="ff2c9-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="ff2c9-118">Hvis du ikke er en global administrator, må kontoen din legges til rollen eDiscovery Manager eller kontroll av Samsvars søk for å søke etter meldinger.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="ff2c9-119">Hvis du vil slette meldinger, må du bli med i rollegruppen for organisasjonsadministrasjon eller administrasjons rollen for søk og fjerning.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ff2c9-120">Tillatelser for disse rollene er tilordnet i [sikkerhets-og samsvarssenteret](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="ff2c9-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="ff2c9-121">[Opprett et innholdssøk](https://docs.microsoft.com/office365/securitycompliance/content-search) for å finne meldingen som skal slettes.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="ff2c9-122">[Koble til PowerShell for sikkerhets-og samsvarssenter](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ff2c9-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="ff2c9-123">Hvis du bruker multifaktorautentisering, kan du se [Koble til Office 365 sikkerhet og kompatibilitet Center PowerShell ved hjelp av multi-faktor-godkjenning](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ff2c9-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>