---
title: 2491 Varsle e-postmeldinger fra policyen «Phish Delivered på grunn av tenant eller brukeroverstyring»
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544587"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="f2193-102">Varsle e-postmeldinger fra policyen «Phish Delivered på grunn av tenant eller brukeroverstyring»</span><span class="sxs-lookup"><span data-stu-id="f2193-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="f2193-103">En standard varslingspolicy kalt «Phish Delivered på grunn av leier eller brukeroverstyring» er rullet ut til leiere med Microsoft Defender for Office 365 P1- og P2-lisenser.</span><span class="sxs-lookup"><span data-stu-id="f2193-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="f2193-104">Hvis du har mottatt dette varselet, følger du fremgangsmåten nedenfor for å undersøke:</span><span class="sxs-lookup"><span data-stu-id="f2193-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="f2193-105">Klikk Vis varsel i **varselmeldingen**  for å gå til Varsler-siden i sikkerhetssenteret & samsvarssenteret.</span><span class="sxs-lookup"><span data-stu-id="f2193-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="f2193-106">Velg varselet for å se alternativet For **å vise meldingslisten** **eller Vise meldinger i Explorer**.</span><span class="sxs-lookup"><span data-stu-id="f2193-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="f2193-107">Begge disse alternativene tar deg til detaljene i meldingen, som inkluderer meldings-ID-en.</span><span class="sxs-lookup"><span data-stu-id="f2193-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="f2193-108">Vær oppmerksom på at Trusselutforsker-koblingen automatisk filtrerer meldingene som samsvarer med varselkriteriene.</span><span class="sxs-lookup"><span data-stu-id="f2193-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="f2193-109">Du må kanskje justere datofilteret i Trusselutforsker.</span><span class="sxs-lookup"><span data-stu-id="f2193-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="f2193-110">Phishing-meldingen ble levert på grunn av en manuelt konfigurert overstyring:</span><span class="sxs-lookup"><span data-stu-id="f2193-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="f2193-111">En tillatt avsender eller et domene angitt av brukeren.</span><span class="sxs-lookup"><span data-stu-id="f2193-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="f2193-112">En tillatt avsender eller et domene angitt av administratoren i en policy for søppelpost.</span><span class="sxs-lookup"><span data-stu-id="f2193-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="f2193-113">En tillatt IP-adresse i en policy for tilkoblingsfilter.</span><span class="sxs-lookup"><span data-stu-id="f2193-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="f2193-114">En regel for e-postflyt (også kalt en transportregel) som er konfigurert til å tillate meldinger i.</span><span class="sxs-lookup"><span data-stu-id="f2193-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="f2193-115">Hvis du mener at meldingen ble feil merket som phish, bruker du Outlook [Rapportmelding-tillegget](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til å sende meldingseksempler til Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2193-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
