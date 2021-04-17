---
title: Moderne e-postfakturering i Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820835"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="6f93b-102">E-postfakturering i Azure</span><span class="sxs-lookup"><span data-stu-id="6f93b-102">Email invoicing in Azure</span></span>

<span data-ttu-id="6f93b-103">Du må ha rollen eier eller bidragsyter på faktureringsprofilen eller faktureringskontoen for å oppdatere innstillingen for e-postfakturering.</span><span class="sxs-lookup"><span data-stu-id="6f93b-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="6f93b-104">Når du har aktivert dette, får alle brukere som har rollene eier, bidragsyter, lesere og fakturaansvarlig på en faktureringsprofil, faktura på e-post.</span><span class="sxs-lookup"><span data-stu-id="6f93b-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="6f93b-105">Logg på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6f93b-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6f93b-106">Søk etter **Kostnadsadministrasjon + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="6f93b-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="6f93b-107">Velg **Fakturaer** fra venstre side, og velg deretter **E-postfaktura** fra toppen av siden.</span><span class="sxs-lookup"><span data-stu-id="6f93b-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="6f93b-108">Hvis du har flere faktureringsprofiler, velger du en faktureringsprofil og deretter **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="6f93b-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="6f93b-109">Velg **Oppdater**.</span><span class="sxs-lookup"><span data-stu-id="6f93b-109">Select **Update**.</span></span>
6. <span data-ttu-id="6f93b-110">Hvis du har flere faktureringsprofiler, velger du en faktureringsprofil og deretter **Aktiver**.</span><span class="sxs-lookup"><span data-stu-id="6f93b-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="6f93b-111">Du gir andre tilgang til å vise, laste ned og betale fakturaer ved å tilordne dem rollen fakturaansvarlig for en MCA- eller MPA-faktureringsprofil.</span><span class="sxs-lookup"><span data-stu-id="6f93b-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="6f93b-112">Hvis du har aktivert å få faktura på e-post, får brukerne også fakturaene på e-post.</span><span class="sxs-lookup"><span data-stu-id="6f93b-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="6f93b-113">Logg på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="6f93b-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="6f93b-114">Søk etter **Kostnadsadministrasjon + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="6f93b-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="6f93b-115">Velg **Faktureringsprofiler** fra venstre side.</span><span class="sxs-lookup"><span data-stu-id="6f93b-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="6f93b-116">Velg en faktureringsprofil som du vil tilordne rollen fakturaansvarlig, fra listen over faktureringsprofiler.</span><span class="sxs-lookup"><span data-stu-id="6f93b-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="6f93b-117">Velg **Tilgangskontroll (IAM)** fra venstre side, og velg deretter **Legg til** fra toppen av siden.</span><span class="sxs-lookup"><span data-stu-id="6f93b-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="6f93b-118">Velg **Fakturaansvarlig** i rullegardinlisten Rolle.</span><span class="sxs-lookup"><span data-stu-id="6f93b-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="6f93b-119">Angi e-postadressen til brukeren for å gi tilgang.</span><span class="sxs-lookup"><span data-stu-id="6f93b-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="6f93b-120">Velg **Lagre** for å tilordne rollen.</span><span class="sxs-lookup"><span data-stu-id="6f93b-120">Select **Save** to assign the role.</span></span>
