---
title: Feilsøke feilkode AADSTS50011
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036671"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="d9c7c-102">Feilsøke feilkode AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="d9c7c-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="d9c7c-103">Hvis du vil løse AADSTS50011-feil, utfører du det anbefalte trinnet som er beskrevet nedenfor.</span><span class="sxs-lookup"><span data-stu-id="d9c7c-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="d9c7c-104">**AADSTS50011**: InvalidReplyTo – Svaradressen mangler, er feilkonfigurert eller samsvarer ikke med svaradressene som er konfigurert for appen.</span><span class="sxs-lookup"><span data-stu-id="d9c7c-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="d9c7c-105">Som en løsning sikrer du at du legger til denne manglende svaradressen i Azure Active Directory-appen (AD), eller at noen med tillatelse til å administrere programmet i AD gjør dette for deg.</span><span class="sxs-lookup"><span data-stu-id="d9c7c-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="d9c7c-106">Hvis du vil ha mer informasjon, kan du se feilsøkingsartikkelen for feil [AADSTS50011.](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch)</span><span class="sxs-lookup"><span data-stu-id="d9c7c-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>