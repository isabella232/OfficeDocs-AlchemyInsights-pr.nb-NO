---
title: Identifisere Slett melding hendelser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909421"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="f689e-102">Overvåkingsloggen for slettede e-postmeldinger</span><span class="sxs-lookup"><span data-stu-id="f689e-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="f689e-103">Starter i januar 2019, slås Microsoft på postboks-sporing logger som standard.</span><span class="sxs-lookup"><span data-stu-id="f689e-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="f689e-104">Ellers, hvis du vil se gjennom Slett melding hendelser for en bestemt bruker, må du aktivere manuelt slette-aksjoner for overvåking.</span><span class="sxs-lookup"><span data-stu-id="f689e-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="f689e-105">Hvis postboksen overvåkes logging allerede er aktivert for organisasjonen, eller for en bestemt bruker, følger du fremgangsmåten nedenfor.</span><span class="sxs-lookup"><span data-stu-id="f689e-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="f689e-106">Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="f689e-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="f689e-107">Klikk **Søk og undersøkelser** , og velg **Overvåk Logg Søk**.</span><span class="sxs-lookup"><span data-stu-id="f689e-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="f689e-108">Velg datointervallet i feltene **Startdato** og **Sluttdato** .</span><span class="sxs-lookup"><span data-stu-id="f689e-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="f689e-109">Angi brukernavnet for brukeren som du vil undersøke (brukeren som slettet elementene).</span><span class="sxs-lookup"><span data-stu-id="f689e-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="f689e-110">Velg **Slettede meldinger fra Slettede elementer-mappen** og **Moved meldinger til Slettede elementer-mappen**i **aktiviteter** -feltet.</span><span class="sxs-lookup"><span data-stu-id="f689e-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="f689e-111">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="f689e-111">Click **Search**.</span></span>

<span data-ttu-id="f689e-112">I resultatene, velger du et kontrollregister.</span><span class="sxs-lookup"><span data-stu-id="f689e-112">In the results, select an audit record.</span></span> <span data-ttu-id="f689e-113">Klikk **Mer informasjon**i detaljer-undermeny.</span><span class="sxs-lookup"><span data-stu-id="f689e-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="f689e-114">Hvis du vil ha mer informasjon om slettet element (for eksempel Emne-linjen, og plasseringen av elementet når det ble slettet) vises i feltet **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="f689e-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="f689e-115">Egenskapen **ClientInfoString** viser Hvis slettingen oppstod i Outlook, Outlook på weben (tidligere kjent som Outlook Web App) eller andre enheter.</span><span class="sxs-lookup"><span data-stu-id="f689e-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="f689e-116">Hvis du vil ha mer informasjon, kan du se [Determining som konfigurere e-post videresending for en bestemt postboks](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="f689e-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="f689e-117">**Merk**: du kan ikke gjenopprette slettede elementer ved hjelp av funksjonen for overvåkingspolicy logg.</span><span class="sxs-lookup"><span data-stu-id="f689e-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="f689e-118">Hvis du vil hente slettede meldinger i Outlook på World Wide web, kan du se [Gjenopprett slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="f689e-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>