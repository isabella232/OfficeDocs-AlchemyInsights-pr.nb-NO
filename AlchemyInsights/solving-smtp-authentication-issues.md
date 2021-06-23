---
title: Aktivere SMTP-godkjenning og feilsøking
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077660"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="0960a-102">Aktivere SMTP-godkjenning og feilsøking</span><span class="sxs-lookup"><span data-stu-id="0960a-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="0960a-103">Hvis du vil aktivere SMTP-godkjenning for en postboks eller får feilmeldingen «Klient ikke godkjent», «Godkjenning mislyktes» eller «SmtpClientAuthentication» med kode 5.7.57 eller 5.7.3 eller 5.7.139 når du prøver å videresende e-post ved å godkjenne en enhet eller et program med Microsoft 365, utfører du disse tre handlingene for å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="0960a-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="0960a-104">Deaktiver [sikkerhetsstandardene for Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ved å slå **Aktiver sikkerhetsstandarder** til **Nei**.</span><span class="sxs-lookup"><span data-stu-id="0960a-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="0960a-105">a.</span><span class="sxs-lookup"><span data-stu-id="0960a-105">a.</span></span> <span data-ttu-id="0960a-106">Logg deg på Azure-portalen som sikkerhetsadministrator, betinget tilgangsadministrator eller global administrator.</span><span class="sxs-lookup"><span data-stu-id="0960a-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="0960a-107">b.</span><span class="sxs-lookup"><span data-stu-id="0960a-107">b.</span></span> <span data-ttu-id="0960a-108">Bla til Azure Active Directory > **egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="0960a-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="0960a-109">c.</span><span class="sxs-lookup"><span data-stu-id="0960a-109">c.</span></span> <span data-ttu-id="0960a-110">Velg **Behandle sikkerhetsstandarder**.</span><span class="sxs-lookup"><span data-stu-id="0960a-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="0960a-111">d.</span><span class="sxs-lookup"><span data-stu-id="0960a-111">d.</span></span> <span data-ttu-id="0960a-112">Angi **Aktiver sikkerhetsstandarder** til **Nei**.</span><span class="sxs-lookup"><span data-stu-id="0960a-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="0960a-113">e.</span><span class="sxs-lookup"><span data-stu-id="0960a-113">e.</span></span> <span data-ttu-id="0960a-114">Velg **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="0960a-114">Select **Save**.</span></span>

2. <span data-ttu-id="0960a-115">[Aktiver SMTP-klientinnsending](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) på den lisensierte postboksen.</span><span class="sxs-lookup"><span data-stu-id="0960a-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="0960a-116">a.</span><span class="sxs-lookup"><span data-stu-id="0960a-116">a.</span></span> <span data-ttu-id="0960a-117">Fra Administrasjonssenter for Microsoft 365 går du til **Aktive brukere**, og velger brukeren.</span><span class="sxs-lookup"><span data-stu-id="0960a-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="0960a-118">b.</span><span class="sxs-lookup"><span data-stu-id="0960a-118">b.</span></span> <span data-ttu-id="0960a-119">Gå til E-post-fanen, og velg Behandle **e-postapper** under E-postapper . </span><span class="sxs-lookup"><span data-stu-id="0960a-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="0960a-120">d.</span><span class="sxs-lookup"><span data-stu-id="0960a-120">d.</span></span> <span data-ttu-id="0960a-121">Kontroller at **Godkjent SMTP er** avmerket (aktivert).</span><span class="sxs-lookup"><span data-stu-id="0960a-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="0960a-122">e.</span><span class="sxs-lookup"><span data-stu-id="0960a-122">e.</span></span> <span data-ttu-id="0960a-123">Velg **Lagre endringer**.</span><span class="sxs-lookup"><span data-stu-id="0960a-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="0960a-124">[Deaktiver godkjenning med flere faktorer (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) på den lisensierte postboksen.</span><span class="sxs-lookup"><span data-stu-id="0960a-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="0960a-125">a.</span><span class="sxs-lookup"><span data-stu-id="0960a-125">a.</span></span> <span data-ttu-id="0960a-126">Gå til Administrasjonssenter for Microsoft 365, og velg Brukere aktive brukere i navigasjonsmenyen  >  **til venstre.**</span><span class="sxs-lookup"><span data-stu-id="0960a-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="0960a-127">b.</span><span class="sxs-lookup"><span data-stu-id="0960a-127">b.</span></span> <span data-ttu-id="0960a-128">Velg **Godkjenning med flere faktorer**.</span><span class="sxs-lookup"><span data-stu-id="0960a-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="0960a-129">c.</span><span class="sxs-lookup"><span data-stu-id="0960a-129">c.</span></span> <span data-ttu-id="0960a-130">Velg brukeren, og deaktiver **godkjenning med flere faktorer**.</span><span class="sxs-lookup"><span data-stu-id="0960a-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
