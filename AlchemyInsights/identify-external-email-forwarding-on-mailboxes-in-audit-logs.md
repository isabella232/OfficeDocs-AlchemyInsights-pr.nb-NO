---
title: Identifisere ekstern videresending av e-post på postbokser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508961"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="9a159-102">Identifisere når ekstern videresending av e-post er konfigurert på postbokser</span><span class="sxs-lookup"><span data-stu-id="9a159-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="9a159-103">Når en Microsoft 365-bruker konfigurerer ekstern videresending av e-post på en postboks, overvåkes aktiviteten som en del av **cmdleten Set-Postboks.**</span><span class="sxs-lookup"><span data-stu-id="9a159-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="9a159-104">Du kan se aktiviteten ved hjelp av søk i overvåkingslogg i & samsvarssenter for sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="9a159-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="9a159-105">Logg på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="9a159-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="9a159-106">Gå til søkeloggen for søk i **søkeloggen for søk i søkeloggen for søk**  >  **Audit log search** i søke.</span><span class="sxs-lookup"><span data-stu-id="9a159-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="9a159-107">Velg datointervallet i feltene **Startdato** og **Sluttdato.**</span><span class="sxs-lookup"><span data-stu-id="9a159-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="9a159-108">Du trenger ikke å angi et brukernavn.</span><span class="sxs-lookup"><span data-stu-id="9a159-108">You don't need to specify a username.</span></span> <span data-ttu-id="9a159-109">Kontroller at **Aktiviteter-feltet** er satt til **Vis resultater for alle aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="9a159-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="9a159-110">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="9a159-110">Click **Search**.</span></span>

<span data-ttu-id="9a159-111">Klikk **Filtrer resultater** i resultatene, og skriv inn **Set-Mailbox** i aktivitetsfilterboksen.</span><span class="sxs-lookup"><span data-stu-id="9a159-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="9a159-112">Velg en overvåkingsoppføring i resultatene.</span><span class="sxs-lookup"><span data-stu-id="9a159-112">Select an audit record in the results.</span></span> <span data-ttu-id="9a159-113">Klikk **Mer informasjon**i **undermenyen Detaljer.**</span><span class="sxs-lookup"><span data-stu-id="9a159-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="9a159-114">Du må se på detaljene for hver overvåkingsoppføring for å finne ut om aktiviteten er relatert til videresending av e-post.</span><span class="sxs-lookup"><span data-stu-id="9a159-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="9a159-115">**ObjectId**: Aliasverdien for postboksen som ble endret.</span><span class="sxs-lookup"><span data-stu-id="9a159-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="9a159-116">**Parametere:** _VideresendingSmtpAddress_ angir mål-e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="9a159-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="9a159-117">**UserId**: Brukeren som konfigurerte videresending av e-post på postboksen i **ObjectId-feltet.**</span><span class="sxs-lookup"><span data-stu-id="9a159-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="9a159-118">Hvis du vil ha mer informasjon, kan du se [Finne ut hvem som konfigurerte videresending av e-post for en postboks](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="9a159-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
