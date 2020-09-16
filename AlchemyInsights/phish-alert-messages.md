---
title: 2491 varsle e-postmeldinger fra policyen «phish levert på grunn av leier eller bruker overstyring»
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728620"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="f8bcb-102">Varsle e-postmeldinger fra policyen «phish levert på grunn av leier eller bruker overstyring»</span><span class="sxs-lookup"><span data-stu-id="f8bcb-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="f8bcb-103">En standard varsel policy kalt «phish levert på grunn av leier eller bruker overstyring» er rullet ut til tenanter med Office 365 ATP P1-og P2-lisenser.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="f8bcb-104">Hvis du har mottatt dette varselet, kan du se følgende Fremgangs måte:</span><span class="sxs-lookup"><span data-stu-id="f8bcb-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="f8bcb-105">Fra varsel meldingen klikker du **Vis varsel** for å gå til **varsler** -siden i sikkerhets & samsvars senteret.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="f8bcb-106">Velg varselet for å se alternativet for å **vise meldings listen** eller **vise meldinger i Explorer**.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="f8bcb-107">Begge disse alternativene tar deg til detaljene i meldingen, som inkluderer meldings-ID.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="f8bcb-108">Vær oppmerksom på at trusselen Explorer-koblingen automatisk filtrerer meldingene som Sams varer med varslings kriteriene.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="f8bcb-109">Det kan hende du må justere dato filteret i Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="f8bcb-110">Phishing-meldingen ble levert på grunn av en manuelt konfigurert overstyring:</span><span class="sxs-lookup"><span data-stu-id="f8bcb-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="f8bcb-111">En tillatt avsender eller et domene angitt av brukeren.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="f8bcb-112">En tillatt avsender eller et domene angitt av administratoren i en retnings linje for søppel post.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="f8bcb-113">En tillatt IP-adresse i en policy for tilkoblings filter.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="f8bcb-114">En regel for e-postflyt (også kjent som en transport regel) som er konfigurert til å tillate meldinger i.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="f8bcb-115">Hvis du tror meldingen ble merket som phish, kan du bruke meldings [tillegget](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) i Outlook til å sende meldings eksempler til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f8bcb-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
