---
title: Videresende e-postmeldinger via Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: e971593b7a67e1bb40243fc762bace6b87a35741
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745406"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="926a1-102">Konfigurere en enhet eller et program med flere funksjoner til å sende e-post ved hjelp av Office 365</span><span class="sxs-lookup"><span data-stu-id="926a1-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="926a1-103">Hvis du vil vite mer om alternativene og trinnene, kan du se [Slik konfigurerer du en enhet eller et program med flere funksjoner til å sende e-post ved hjelp av Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="926a1-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="926a1-104">**Merk:** Hvis du har en enhet eller et program som nylig sluttet å fungere, bør du være oppmerksom på at vi nylig begynte å [deaktivere 3DES-chiffrering](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) som planlagt.</span><span class="sxs-lookup"><span data-stu-id="926a1-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="926a1-105">Hvis du vil se de berørte enhetene, kan du gå til [rapporten SMTP AUTH-klienter](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="926a1-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="926a1-106">Eksempler på vanlige feil kan være: godkjenningsfeil, TLS-feil, feil med algoritme for chiffrering, algoritmekonflikt eller avbrutt tilkobling.</span><span class="sxs-lookup"><span data-stu-id="926a1-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="926a1-107">Slik løser du problemet:</span><span class="sxs-lookup"><span data-stu-id="926a1-107">To resolve the issue:</span></span>
 - <span data-ttu-id="926a1-108">**Windows Server 2003 IIS SMTP vil ikke lenger fungere – en nyere versjon av Windows kreves.**</span><span class="sxs-lookup"><span data-stu-id="926a1-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="926a1-109">Ta kontakt med leverandøren av programmet eller enheten for å se om en moderne chiffrering støttes, eller om det finnes en oppdatering.</span><span class="sxs-lookup"><span data-stu-id="926a1-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
