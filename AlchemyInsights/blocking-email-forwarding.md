---
title: 726 blokkere e-postvideresending
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219864"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="28c73-102">Blokkere eller fjerne blokkeringen av e-postvideresending</span><span class="sxs-lookup"><span data-stu-id="28c73-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="28c73-103">Hvis du vil aktivere eller deaktivere videre sending av e-post for en bestemt post boks, kan du se [konfigurere videre kobling](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="28c73-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="28c73-104">Kontroll over ekstern videre sending utføres på leier nivå ved hjelp av den utgående beskyttelses policyen for søppel post.</span><span class="sxs-lookup"><span data-stu-id="28c73-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="28c73-105">Hvis den er satt til av eller automatisk, kan det blokkere e-postvideresending med tilgangs meldingen "550 5.7.520 ingen tilgang, organisasjonen tillater ikke ekstern videre sending".</span><span class="sxs-lookup"><span data-stu-id="28c73-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="28c73-106">Hvis videre sending ble satt til blokkert, og det er feilen brukerne vil se.</span><span class="sxs-lookup"><span data-stu-id="28c73-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="28c73-107">Hvis videre sending blir blokkert, må du kontrollere at policyen er konfigurert til å aktivere ekstern automatisk videre sending.</span><span class="sxs-lookup"><span data-stu-id="28c73-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="28c73-108">Du kan kontrollere den utgående filter policyen for søppel post fra sikkerhets-og Samsvars senteret eller ved å kjøre kommandoen Get-HostedOutboundSpamFilterPolicy | fl-navn, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="28c73-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="28c73-109">Hvis du vil konfigurere automatisk videre sending, vil den samme kommandoen fortelle deg tilstanden til policyen nå.</span><span class="sxs-lookup"><span data-stu-id="28c73-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="28c73-110">Obs! det anbefales at du holder det eksterne alternativet videresendt automatisk i den standard utgående filter policyen for søppel post og aktiverer den bare for brukere som trenger ekstern videre sending ved å opprette en egen definert policy for disse brukerne.</span><span class="sxs-lookup"><span data-stu-id="28c73-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="28c73-111">Du kan lese mer i [konfigurere ekstern videre sending av e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="28c73-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>