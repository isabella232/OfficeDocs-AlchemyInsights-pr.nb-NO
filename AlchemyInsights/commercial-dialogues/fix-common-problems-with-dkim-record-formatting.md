---
title: Løse vanlige problemer med DKIM-postformatering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750762"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="7a029-102">Løse vanlige problemer med DKIM-postformatering</span><span class="sxs-lookup"><span data-stu-id="7a029-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="7a029-103">De fleste DKIM-oppsettproblemer er relatert til feil DNS-poster.</span><span class="sxs-lookup"><span data-stu-id="7a029-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="7a029-104">Kontroller at DKIM CNAME-posten **(ikke** en TXT-post) er riktig formatert for å løse DKIM-oppsettsproblemene.</span><span class="sxs-lookup"><span data-stu-id="7a029-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="7a029-105">Hvis du vil ha mer informasjon, kan du se Hva du må gjøre for å [konfigurere DKIM manuelt i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="7a029-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="7a029-106">Hvis du trenger hjelp med DNS-poster generelt, kan du se [Opprette DNS-poster hos en DNS-vertsleverandør for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="7a029-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="7a029-107">Når du har opprettet eller oppdatert DKIM DNS-postene hos DNS-vertstjenesten for domenet, må du vente på at DNS-postene skal overføres.</span><span class="sxs-lookup"><span data-stu-id="7a029-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
