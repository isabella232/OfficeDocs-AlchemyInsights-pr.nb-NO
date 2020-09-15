---
title: Manglende e-postmeldinger i karantene
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673723"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="08bd1-102">Manglende e-postmeldinger i karantene</span><span class="sxs-lookup"><span data-stu-id="08bd1-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="08bd1-103">Administratorer kan [vise, frigi eller slette disse meldingene.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="08bd1-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="08bd1-104">Hvis du vil åpne sikkerhets & Samsvars senteret, går du til [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="08bd1-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="08bd1-105">Hvis du vil åpne karantene siden direkte, går du til [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="08bd1-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="08bd1-106">Du kan søke etter følgende verdier:</span><span class="sxs-lookup"><span data-stu-id="08bd1-106">You can search by the following values:</span></span>  

- <span data-ttu-id="08bd1-107">**Meldings-ID**: den globalt unike identifikatoren for meldingen.</span><span class="sxs-lookup"><span data-stu-id="08bd1-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="08bd1-108">Hvis du velger en melding i listen, vises  **meldings-ID**  -verdien i ruten  **detaljer**  under meny som vises.</span><span class="sxs-lookup"><span data-stu-id="08bd1-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="08bd1-109">Administratorer kan bruke [meldings sporing](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) til å finne meldinger og tilsvarende meldings-ID-verdier.</span><span class="sxs-lookup"><span data-stu-id="08bd1-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="08bd1-110">**Avsender-e**-postadresse: en enkelt avsenderens e-postadresse.</span><span class="sxs-lookup"><span data-stu-id="08bd1-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="08bd1-111">**Mottakerens e-postadresse**: en enkelt mottakers e-postadresse.</span><span class="sxs-lookup"><span data-stu-id="08bd1-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="08bd1-112">**Emne**: Bruk hele emnet i meldingen.</span><span class="sxs-lookup"><span data-stu-id="08bd1-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="08bd1-113">Søket skiller ikke mellom store og små bokstaver.</span><span class="sxs-lookup"><span data-stu-id="08bd1-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="08bd1-114">Når du har skrevet inn søke kriteriene, klikker du Oppdater ![ knappe ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **oppdatering** for å filtrere resultatene.  </span><span class="sxs-lookup"><span data-stu-id="08bd1-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="08bd1-115">Cmdletene du bruker til å vise og administrere meldinger og filer i karantene, er:</span><span class="sxs-lookup"><span data-stu-id="08bd1-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="08bd1-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="08bd1-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="08bd1-117">Eksporter-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="08bd1-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="08bd1-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="08bd1-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="08bd1-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Vær oppmerksom på at denne cmdleten bare er for meldinger, ikke filer med skadelig program vare fra ATP for SharePoint Online, OneDrive for Business eller Teams.</span><span class="sxs-lookup"><span data-stu-id="08bd1-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="08bd1-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="08bd1-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)