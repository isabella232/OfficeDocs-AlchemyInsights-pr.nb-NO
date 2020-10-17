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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478326"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="19f17-102">Blokkere eller fjerne blokkeringen av e-postvideresending</span><span class="sxs-lookup"><span data-stu-id="19f17-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="19f17-103">Hvis du vil aktivere eller deaktivere videre sending av e-post for en bestemt post boks, kan du se [konfigurere videre kobling](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="19f17-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="19f17-104">Kontroll over ekstern videre sending utføres på leier nivå ved hjelp av den utgående søppel post policyen.</span><span class="sxs-lookup"><span data-stu-id="19f17-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="19f17-105">Du kan kontrollere den utgående filter policyen for søppel post fra sikkerhets-og Samsvars senteret [her](https://protection.office.com/antispam) eller ved å bruke [Get-HostedOutboundSpamFilterPolicy-kommandoen](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="19f17-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="19f17-106">Hvis du får følgende feil melding: **«550 5.7.520 tilgang nektet, organisasjonen tillater ikke ekstern videre sending»**, må du sørge for at policyen er konfigurert til å aktivere ekstern automatisk videre sending.</span><span class="sxs-lookup"><span data-stu-id="19f17-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="19f17-107">**Obs!** Det anbefales at du holder det eksterne alternativet videresendt automatisk i den standard utgående filter policyen for søppel post og aktiverer den bare for brukere som trenger ekstern videre kobling ved å opprette en egen definert policy for disse brukerne.</span><span class="sxs-lookup"><span data-stu-id="19f17-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="19f17-108">Du kan lese mer i [konfigurere ekstern videre sending av e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="19f17-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>