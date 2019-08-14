---
title: 2491 varsel e-postmeldinger fra Phish leveres på grunn av leier eller bruker overstyre policyen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391420"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="821fc-102">Varsle e-postmeldinger fra Phish leveres på grunn av leier eller bruker overstyre policyen</span><span class="sxs-lookup"><span data-stu-id="821fc-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="821fc-103">Et varsel som policy kalt "Phish levert på grunn av leier eller bruker overstyring" har blitt rullet til leiere med Office 365 ATP P1 og P2 lisenser.</span><span class="sxs-lookup"><span data-stu-id="821fc-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="821fc-104">Hvis du mottok varslet, er her fremgangsmåten for å undersøke:</span><span class="sxs-lookup"><span data-stu-id="821fc-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="821fc-105">Fra varselmeldingen, klikker du **Vis varsel** for å gå til siden **varsler** i Security-& overholdelsessenteret.</span><span class="sxs-lookup"><span data-stu-id="821fc-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="821fc-106">Velg varselet for å se alternativet for å **vise meldingslisten** eller **vise meldinger i Explorer**.</span><span class="sxs-lookup"><span data-stu-id="821fc-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="821fc-107">Begge disse alternativene tar deg til detaljer om meldingen, som inkluderer melding-ID.</span><span class="sxs-lookup"><span data-stu-id="821fc-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="821fc-108">Vær oppmerksom på at koblingen trusselen Explorer automatisk filtrere meldinger som samsvarer med varslingskriteriene.</span><span class="sxs-lookup"><span data-stu-id="821fc-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="821fc-109">Du må kanskje justere datofilteret i trusselen Explorer.</span><span class="sxs-lookup"><span data-stu-id="821fc-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="821fc-110">Phishing-melding ble levert på grunn av en overstyring av manuelt konfigurerte:</span><span class="sxs-lookup"><span data-stu-id="821fc-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="821fc-111">Tillatte avsenderen eller domenet som er angitt av brukeren.</span><span class="sxs-lookup"><span data-stu-id="821fc-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="821fc-112">Tillatte avsenderen eller domenet som er angitt av administrator i en policy for beskyttelse mot søppelpost.</span><span class="sxs-lookup"><span data-stu-id="821fc-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="821fc-113">En tillatte IP-adresse i en tilkobling filter-policy.</span><span class="sxs-lookup"><span data-stu-id="821fc-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="821fc-114">En flyt-post (også kjent som regel transport) som er konfigurert for å tillate meldinger i.</span><span class="sxs-lookup"><span data-stu-id="821fc-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="821fc-115">Hvis du mener at meldingen var feilaktig merket som phish bruke Outlook [rapportmelding-tillegg](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til å sende meldingen-eksempler til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="821fc-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
