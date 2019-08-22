---
title: Identifisere ekstern e-post videresending på postbokser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539110"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="78cdb-102">Identifisere når ekstern e-post videresending er konfigurert på postbokser</span><span class="sxs-lookup"><span data-stu-id="78cdb-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="78cdb-103">Når en bruker for Office 365 konfigurerer videresending av ekstern e-post på en postboks, er aktiviteten overvåket som en del av cmdleten **Set-postboks** .</span><span class="sxs-lookup"><span data-stu-id="78cdb-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="78cdb-104">Du kan vise aktiviteten ved hjelp av sporing Logg Søk i Security-& overholdelsessenteret.</span><span class="sxs-lookup"><span data-stu-id="78cdb-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="78cdb-105">Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="78cdb-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="78cdb-106">Gå til **Søk** > **Overvåk Logg Søk** -siden.</span><span class="sxs-lookup"><span data-stu-id="78cdb-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="78cdb-107">Velg datointervallet i feltene **Startdato** og **Sluttdato** .</span><span class="sxs-lookup"><span data-stu-id="78cdb-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="78cdb-108">Du trenger ikke å angi et brukernavn.</span><span class="sxs-lookup"><span data-stu-id="78cdb-108">You don't need to specify a username.</span></span> <span data-ttu-id="78cdb-109">Kontroller **aktiviteter** -feltet er satt til å **vise resultater for alle aktiviteter**.</span><span class="sxs-lookup"><span data-stu-id="78cdb-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="78cdb-110">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="78cdb-110">Click **Search**.</span></span>

<span data-ttu-id="78cdb-111">I resultatene klikker du **Filtreringsresultatene** og Skriv inn **Sett postboks** filterlisten for aktiviteten.</span><span class="sxs-lookup"><span data-stu-id="78cdb-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="78cdb-112">Velg et kontrollregister i resultatene.</span><span class="sxs-lookup"><span data-stu-id="78cdb-112">Select an audit record in the results.</span></span> <span data-ttu-id="78cdb-113">I **Detaljer** -undermeny, klikker du **vil ha mer informasjon**.</span><span class="sxs-lookup"><span data-stu-id="78cdb-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="78cdb-114">Du må se på detaljene for hver kontrollregister å finne ut om aktiviteten er knyttet til e-post videresending.</span><span class="sxs-lookup"><span data-stu-id="78cdb-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="78cdb-115">**ObjectId**: alias verdien av postboksen som ble endret.</span><span class="sxs-lookup"><span data-stu-id="78cdb-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="78cdb-116">**Parametere**: _ForwardingSmtpAddress_ angir måladressen for e-post.</span><span class="sxs-lookup"><span data-stu-id="78cdb-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="78cdb-117">**Bruker-ID**: brukeren som konfigurert videresending av e-post på postboksen i **objekt-ID** -feltet.</span><span class="sxs-lookup"><span data-stu-id="78cdb-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="78cdb-118">Hvis du vil ha mer informasjon, kan du se [Determining som konfigurere e-post videresending for en bestemt postboks](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="78cdb-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
