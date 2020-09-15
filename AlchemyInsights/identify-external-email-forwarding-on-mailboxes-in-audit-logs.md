---
title: Identifisere eksterne e-postvideresending på post bokser i overvåkings logger
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696306"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c3ac5-102">Identifisere når ekstern e-postvideresending konfigureres på post bokser</span><span class="sxs-lookup"><span data-stu-id="c3ac5-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c3ac5-103">Når en Microsoft 365-bruker konfigurerer ekstern e-postvideresending på en post boks, overvåkes aktiviteten som en del av cmdleten **Set-post boks** .</span><span class="sxs-lookup"><span data-stu-id="c3ac5-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c3ac5-104">Du kan se aktiviteten ved hjelp av overvåkings Logg søk i sikkerhets & Samsvars senteret.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c3ac5-105">Logg på [sikkerhets & samsvars senteret til Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c3ac5-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c3ac5-106">Gå til **Search**  >  **søke siden for overvåkings Logg** for søk.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c3ac5-107">Velg dato området i feltene **Start dato** og **slutt dato** .</span><span class="sxs-lookup"><span data-stu-id="c3ac5-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c3ac5-108">Du trenger ikke angi et bruker navn.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-108">You don't need to specify a username.</span></span> <span data-ttu-id="c3ac5-109">Kontroller at **aktiviteter** -feltet er satt til å **vise resultater for alle aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c3ac5-110">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-110">Click **Search**.</span></span>

<span data-ttu-id="c3ac5-111">I resultatene klikker du **Filtrer resultater** og skriv inn **Set-postboks** i aktivitets Filter-boksen.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c3ac5-112">Velg en overvåkings post i resultatene.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-112">Select an audit record in the results.</span></span> <span data-ttu-id="c3ac5-113">Klikk **mer informasjon**i under menyen **detaljer** .</span><span class="sxs-lookup"><span data-stu-id="c3ac5-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c3ac5-114">Du må se på detaljene for hver overvåkings post for å avgjøre om aktiviteten er relatert til videre sending av e-post.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c3ac5-115">**ObjectID**: alias-verdien til post boksen som ble endret.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c3ac5-116">**Parametere**: _ForwardingSmtpAddress_ angir mål-e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c3ac5-117">**Userid**: brukeren som konfigurerte e-postvideresending på post boksen i **objectID** -feltet.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c3ac5-118">Hvis du vil ha mer informasjon, kan du se [finne ut hvem som konfigurerte videre sendingen av e-post](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)</span><span class="sxs-lookup"><span data-stu-id="c3ac5-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
