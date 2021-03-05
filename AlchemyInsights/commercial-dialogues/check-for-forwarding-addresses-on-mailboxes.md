---
title: Se etter videresendingsadresser for postbokser
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482777"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="30ede-102">Se etter videresendingsadresser for postbokser</span><span class="sxs-lookup"><span data-stu-id="30ede-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="30ede-103">Noen ganger hackere videresender brukernes e-postmeldinger til seg selv, så først må vi se etter videresending av adresser og regler på postboksen.</span><span class="sxs-lookup"><span data-stu-id="30ede-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="30ede-104">Deretter kontrollerer vi overvåkingsloggene.</span><span class="sxs-lookup"><span data-stu-id="30ede-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="30ede-105">Slik ser du etter adresser som videresender:</span><span class="sxs-lookup"><span data-stu-id="30ede-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="30ede-106">Velg **Brukere som** er aktive  >  **brukere.**</span><span class="sxs-lookup"><span data-stu-id="30ede-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="30ede-107">Velg brukeren som har en konto som er kompromittert.</span><span class="sxs-lookup"><span data-stu-id="30ede-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="30ede-108">Utvid E-postinnstillinger i undermenyen som vises, og klikk deretter **Rediger** for videresending av **e-post.**</span><span class="sxs-lookup"><span data-stu-id="30ede-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="30ede-109">Fjern eventuelle videresendingsadresser som du ikke gjenkjenner.</span><span class="sxs-lookup"><span data-stu-id="30ede-109">Remove any forwarding addresses you don't recognize.</span></span>