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
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716469"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="8083d-102">Identifisere når ekstern videresending av e-post er konfigurert på postbokser</span><span class="sxs-lookup"><span data-stu-id="8083d-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="8083d-103">Når en Microsoft 365-bruker konfigurerer ekstern videresending av e-post på en postboks, overvåkes aktiviteten som en del av cmdleten **Set-postboks.**</span><span class="sxs-lookup"><span data-stu-id="8083d-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="8083d-104">Du kan se aktiviteten ved hjelp av overvåkingsloggsøk i Sikkerhets& compliance Center.</span><span class="sxs-lookup"><span data-stu-id="8083d-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="8083d-105">Logg på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="8083d-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="8083d-106">Gå til**søkesiden for søkeloggen for søke etter** søk i **søkesiden for søkeetter søk.** > </span><span class="sxs-lookup"><span data-stu-id="8083d-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="8083d-107">Velg datoperioden i feltene **Startdato** og **Sluttdato.**</span><span class="sxs-lookup"><span data-stu-id="8083d-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="8083d-108">Du trenger ikke å angi et brukernavn.</span><span class="sxs-lookup"><span data-stu-id="8083d-108">You don't need to specify a username.</span></span> <span data-ttu-id="8083d-109">Kontroller **at Aktiviteter-feltet** er satt til **Vis resultater for alle aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="8083d-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="8083d-110">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="8083d-110">Click **Search**.</span></span>

<span data-ttu-id="8083d-111">Klikk **Filtrer resultater** i resultatene, og skriv inn **Set-postboks** i aktivitetsfilterboksen.</span><span class="sxs-lookup"><span data-stu-id="8083d-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="8083d-112">Velg en overvåkingspost i resultatene.</span><span class="sxs-lookup"><span data-stu-id="8083d-112">Select an audit record in the results.</span></span> <span data-ttu-id="8083d-113">Klikk **Mer informasjon**i undermenyen **Detaljer.**</span><span class="sxs-lookup"><span data-stu-id="8083d-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="8083d-114">Du må se på detaljene for hver revisjonsoppføring for å finne ut om aktiviteten er relatert til videresending av e-post.</span><span class="sxs-lookup"><span data-stu-id="8083d-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="8083d-115">**ObjectId**: Aliasverdien for postboksen som ble endret.</span><span class="sxs-lookup"><span data-stu-id="8083d-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="8083d-116">**Parametere**: _ForwardingSmtpAddress_ angir mål-e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="8083d-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="8083d-117">**UserId**: Brukeren som konfigurerte videresending av e-post på postboksen i **ObjectId-feltet.**</span><span class="sxs-lookup"><span data-stu-id="8083d-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="8083d-118">Hvis du vil ha mer informasjon, kan du se [Finne ut hvem som konfigurerer videresending av e-post for en postboks](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="8083d-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
