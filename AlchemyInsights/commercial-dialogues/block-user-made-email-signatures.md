---
title: Blokkere brukerdefinerte e-postsignaturer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482308"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="29fee-102">Blokkere brukerdefinerte e-postsignaturer</span><span class="sxs-lookup"><span data-stu-id="29fee-102">Block user-made email signatures</span></span>

<span data-ttu-id="29fee-103">Følgende løsning gjelder bare for e-postsignaturer opprettet i Outlook på nettet.</span><span class="sxs-lookup"><span data-stu-id="29fee-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="29fee-104">Du kan bare blokkere signaturer i Outlook-appen hvis du har en lokal Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="29fee-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="29fee-105">Velg **Administrasjonssentre** for Exchange i  >  **administrasjonssenteret.**</span><span class="sxs-lookup"><span data-stu-id="29fee-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="29fee-106">Klikk **tillatelser for** Outlook Web  >  **App-policyer.**</span><span class="sxs-lookup"><span data-stu-id="29fee-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="29fee-107">Velg policyen, og klikk deretter blyantikonet for å redigere det.</span><span class="sxs-lookup"><span data-stu-id="29fee-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="29fee-108">Klikk **funksjoner Flere**  >  **alternativer.**</span><span class="sxs-lookup"><span data-stu-id="29fee-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="29fee-109">Fjern merket for E-postsignatur **under** Brukeropplevelse, og klikk deretter **Lagre.** </span><span class="sxs-lookup"><span data-stu-id="29fee-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="29fee-110">**Viktig:** Hvis en signatur ble lagt til før merket ble fjernet i avmerkingsboksen, vil brukeren fremdeles kunne bruke den.</span><span class="sxs-lookup"><span data-stu-id="29fee-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="29fee-111">Be dem om å fjerne den.</span><span class="sxs-lookup"><span data-stu-id="29fee-111">Ask them to remove it.</span></span>
