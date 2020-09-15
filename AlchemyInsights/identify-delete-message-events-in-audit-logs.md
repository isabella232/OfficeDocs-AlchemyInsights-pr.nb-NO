---
title: Identifisere slette meldings hendelser i overvåkings logger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696522"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="c88df-102">Overvåke logger for slettede e-postmeldinger</span><span class="sxs-lookup"><span data-stu-id="c88df-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="c88df-103">Microsoft slår på post boks overvåkings logging som standard i januar 2019.</span><span class="sxs-lookup"><span data-stu-id="c88df-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="c88df-104">Hvis du vil se gjennom slette meldings hendelser for en bestemt bruker, må du aktivere slette handlingene for overvåking manuelt.</span><span class="sxs-lookup"><span data-stu-id="c88df-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="c88df-105">Hvis overvåkings logging for post boks allerede er aktivert for organisasjonen eller for den bestemte brukeren, følger du Fremgangs måten nedenfor.</span><span class="sxs-lookup"><span data-stu-id="c88df-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="c88df-106">Logg på [sikkerhets & samsvars senter for Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c88df-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c88df-107">Klikk **Søk og undersøkelser** , og velg **Søk i overvåkings Logg**.</span><span class="sxs-lookup"><span data-stu-id="c88df-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="c88df-108">Velg dato området i feltene **Start dato** og **slutt dato** .</span><span class="sxs-lookup"><span data-stu-id="c88df-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c88df-109">Angi bruker navnet for brukeren du vil undersøke (brukeren som slettet elementene).</span><span class="sxs-lookup"><span data-stu-id="c88df-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="c88df-110">I **aktiviteter** -feltet velger du **slettede meldinger fra Slettede elementer-mappen** og **flyttede meldinger til Slettede elementer-mappen**.</span><span class="sxs-lookup"><span data-stu-id="c88df-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="c88df-111">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="c88df-111">Click **Search**.</span></span>

<span data-ttu-id="c88df-112">Velg en overvåkings post i resultatene.</span><span class="sxs-lookup"><span data-stu-id="c88df-112">In the results, select an audit record.</span></span> <span data-ttu-id="c88df-113">Klikk **mer informasjon**i under menyen detaljer.</span><span class="sxs-lookup"><span data-stu-id="c88df-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c88df-114">Tilleggs informasjon om det slettede elementet (for eksempel Emne linjen og plasseringen av elementet når det er slettet) vises i **AffectedItems** -feltet.</span><span class="sxs-lookup"><span data-stu-id="c88df-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="c88df-115">**ClientInfoString** -egenskapen vises hvis slettingen ble utført i Outlook, Outlook på nettet (tidligere kjent som Outlook Web App) eller en annen enhet.</span><span class="sxs-lookup"><span data-stu-id="c88df-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="c88df-116">Hvis du vil ha mer informasjon, kan du se [finne ut hvem som konfigurerte videre sendingen av e-post](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)</span><span class="sxs-lookup"><span data-stu-id="c88df-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="c88df-117">**Obs!** du kan ikke hente slettede elementer ved hjelp av funksjonen for overvåkings logg.</span><span class="sxs-lookup"><span data-stu-id="c88df-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="c88df-118">Hvis du vil hente slettede meldinger i Outlook på nettet, kan du se [gjenopprette slettede elementer i Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="c88df-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
