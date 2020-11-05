---
title: Moderne Azure e-postfakturering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922138"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="14075-102">E-postfakturering i Azure</span><span class="sxs-lookup"><span data-stu-id="14075-102">Email invoicing in Azure</span></span>

<span data-ttu-id="14075-103">Du må ha en eier eller en bidrags yter rolle på fakturerings profilen eller fakturerings kontoen for å kunne oppdatere innstillingen for e-postfakturaene.</span><span class="sxs-lookup"><span data-stu-id="14075-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="14075-104">Når du har valgt – alle brukere med roller for eier, bidrags yter, lesere og faktura behandling på en fakturerings profil, blir fakturaen i e-post.</span><span class="sxs-lookup"><span data-stu-id="14075-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="14075-105">Logg deg på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="14075-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="14075-106">Søke etter **kostnads administrasjon + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="14075-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="14075-107">Velg **fakturaer** fra venstre side, og velg deretter **e-faktura** fra toppen av siden.</span><span class="sxs-lookup"><span data-stu-id="14075-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="14075-108">Hvis du har flere fakturerings profiler, velger du en fakturerings profil og velger deretter Velg **i**.</span><span class="sxs-lookup"><span data-stu-id="14075-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="14075-109">Velg **Oppdater**.</span><span class="sxs-lookup"><span data-stu-id="14075-109">Select **Update**.</span></span>
6. <span data-ttu-id="14075-110">Hvis du har flere fakturerings profiler, velger du en fakturerings profil og velger deretter Velg **i**.</span><span class="sxs-lookup"><span data-stu-id="14075-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="14075-111">Du gir andre tilgang til å vise, laste ned og betale fakturaer ved å tilordne faktura behandlings rollen til en MCA-eller MPA-fakturerings profil.</span><span class="sxs-lookup"><span data-stu-id="14075-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="14075-112">Hvis du har valgt å få fakturaen i e-post, får brukerne også fakturaene i e-post.</span><span class="sxs-lookup"><span data-stu-id="14075-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="14075-113">Logg deg på [Azure-portalen](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="14075-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="14075-114">Søke etter **kostnads administrasjon + fakturering**.</span><span class="sxs-lookup"><span data-stu-id="14075-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="14075-115">Velg **fakturerings profiler** fra venstre side.</span><span class="sxs-lookup"><span data-stu-id="14075-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="14075-116">Velg en fakturerings profil som du vil tilordne en faktura behandlings rolle fra listen fakturerings profiler.</span><span class="sxs-lookup"><span data-stu-id="14075-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="14075-117">Velg **tilgangs kontroll (iam)** fra venstre side, og velg deretter **Legg til** fra toppen av siden.</span><span class="sxs-lookup"><span data-stu-id="14075-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="14075-118">Velg **faktura behandling** i rulle gardin listen rolle.</span><span class="sxs-lookup"><span data-stu-id="14075-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="14075-119">Skriv inn e-postadressen til brukeren for å gi tilgang.</span><span class="sxs-lookup"><span data-stu-id="14075-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="14075-120">Velg **Lagre** for å tilordne rollen.</span><span class="sxs-lookup"><span data-stu-id="14075-120">Select **Save** to assign the role.</span></span>
