---
title: Identifisere slette meldingshendelser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716505"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="00f52-102">Overvåkingslogger for slettede e-postmeldinger</span><span class="sxs-lookup"><span data-stu-id="00f52-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="00f52-103">Fra og med januar 2019 aktiverer Microsoft overvåkingslogging for postboks som standard.</span><span class="sxs-lookup"><span data-stu-id="00f52-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="00f52-104">Hvis du vil se gjennom slettemeldingshendelser for en bestemt bruker, må du aktivere slettehandlingene for sporing av endringer manuelt.</span><span class="sxs-lookup"><span data-stu-id="00f52-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="00f52-105">Hvis overvåkingslogging for postboksallerede er aktivert for organisasjonen eller for den bestemte brukeren, følger du fremgangsmåten nedenfor.</span><span class="sxs-lookup"><span data-stu-id="00f52-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="00f52-106">Logge på [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="00f52-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="00f52-107">Klikk **Søk og undersøkelse,** og velg **Søk etter overvåkingslogg**.</span><span class="sxs-lookup"><span data-stu-id="00f52-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="00f52-108">Velg datoperioden i feltene **Startdato** og **Sluttdato.**</span><span class="sxs-lookup"><span data-stu-id="00f52-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="00f52-109">Angi brukernavn for brukeren du vil undersøke (brukeren som slettet elementene).</span><span class="sxs-lookup"><span data-stu-id="00f52-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="00f52-110">Velg **Slettede meldinger fra Slettede elementer-mappen** i **Aktiviteter-feltet,** og **Flytt meldinger til Slettede elementer-mappen**.</span><span class="sxs-lookup"><span data-stu-id="00f52-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="00f52-111">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="00f52-111">Click **Search**.</span></span>

<span data-ttu-id="00f52-112">Velg en overvåkingspost i resultatene.</span><span class="sxs-lookup"><span data-stu-id="00f52-112">In the results, select an audit record.</span></span> <span data-ttu-id="00f52-113">Klikk **Mer informasjon**i undermenyen for detaljer.</span><span class="sxs-lookup"><span data-stu-id="00f52-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="00f52-114">Tilleggsinformasjon om det slettede elementet (for eksempel emnelinjen og plasseringen av elementet da det ble slettet) vises i **berørtelementer-feltet.**</span><span class="sxs-lookup"><span data-stu-id="00f52-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="00f52-115">Egenskapen **ClientInfoString** viser om slettingen oppstod i Outlook, Outlook på nettet (tidligere kjent som Outlook Web App) eller en annen enhet.</span><span class="sxs-lookup"><span data-stu-id="00f52-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="00f52-116">Hvis du vil ha mer informasjon, kan du se [Finne ut hvem som konfigurerer videresending av e-post for en postboks](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="00f52-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="00f52-117">**Merk:** Du kan ikke hente slettede elementer ved hjelp av funksjonen for overvåkingslogg.</span><span class="sxs-lookup"><span data-stu-id="00f52-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="00f52-118">Hvis du vil hente slettede meldinger i Outlook på nettet, kan du se [Gjenopprette slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="00f52-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
