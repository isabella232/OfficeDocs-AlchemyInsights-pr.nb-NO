---
title: 1554 Winsock-feil 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859149"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="31dfe-102">Winsock-feil 10061</span><span class="sxs-lookup"><span data-stu-id="31dfe-102">Winsock error 10061</span></span>

<span data-ttu-id="31dfe-103">Denne koden betyr at Office 365 ikke kan opprette en TCP socket (tilkobling) med verten.</span><span class="sxs-lookup"><span data-stu-id="31dfe-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="31dfe-104">Den mest sannsynlige årsaken til denne feilen er et problem med brannmurkonfigurasjonen.</span><span class="sxs-lookup"><span data-stu-id="31dfe-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="31dfe-105">Hvis du vil løse problemet, kontrollerer du disse innstillingene:</span><span class="sxs-lookup"><span data-stu-id="31dfe-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="31dfe-106">Kontroller konfigurasjonen av brannmur med informasjonen i [Office 365 URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="31dfe-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="31dfe-107">Hvis feilen, er spesifikk for Exchange Online Protection (EOP), bør du har blitt tidligere melding til en endring i [Exchange Online beskyttelse IP-adresser](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="31dfe-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="31dfe-108">Kontroller at Internett-leverandøren (ISP) ikke blokkerer porten.</span><span class="sxs-lookup"><span data-stu-id="31dfe-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="31dfe-109">Kontroller smart verts- og serverinnstillingene i koblingene.</span><span class="sxs-lookup"><span data-stu-id="31dfe-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="31dfe-110">Legg merke til at Office 365 ikke blokkerer *innkommende* tilkoblinger på denne måten.</span><span class="sxs-lookup"><span data-stu-id="31dfe-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
