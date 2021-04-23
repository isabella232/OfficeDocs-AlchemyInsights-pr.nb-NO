---
title: Oppbevaringspolicyer i administrasjonssenteret for Exchange fungerer ikke
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952237"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="39094-102">Oppbevaringspolicyer i administrasjonssenteret for Exchange</span><span class="sxs-lookup"><span data-stu-id="39094-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="39094-103">Hvis du vil at vi skal kjøre automatiserte kontroller for innstillingene som er nevnt nedenfor, velger du Tilbake-knappen <- øverst på denne siden, og deretter skriver du inn e-postadressen til brukeren som har problemer med oppbevaringspolicyer.</span><span class="sxs-lookup"><span data-stu-id="39094-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="39094-104">Hvis du har problemer med oppbevaringspolicyer i administrasjonssenteret for Exchange som ikke gjelder for postbokser eller elementer som ikke flyttes til arkivpostboksen, kontrollerer du følgende:</span><span class="sxs-lookup"><span data-stu-id="39094-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="39094-105">**Grunnårsaker:**</span><span class="sxs-lookup"><span data-stu-id="39094-105">**Root Causes:**</span></span>

- <span data-ttu-id="39094-106">**Assistent for administrert** mappe har ikke behandlet brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="39094-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="39094-107">Assistenten for administrert mappe prøver å behandle hver postboks i den skybaserte organisasjonen én gang hver sjuende dag.</span><span class="sxs-lookup"><span data-stu-id="39094-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="39094-108">**Løsning:** Kjør assistenten for administrert mappe.</span><span class="sxs-lookup"><span data-stu-id="39094-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="39094-109">**Oppbevaringshold** er **aktivert** på postboksen.</span><span class="sxs-lookup"><span data-stu-id="39094-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="39094-110">Hvis postboksen er plassert på en Oppbevaringshold, behandles ikke oppbevaringspolicyen for postboksen i løpet av denne tiden.</span><span class="sxs-lookup"><span data-stu-id="39094-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="39094-111">**Løsning:** Kontroller statusen for oppbevaringssperreinnstillingen, og oppdater etter behov.</span><span class="sxs-lookup"><span data-stu-id="39094-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="39094-112">Hvis du vil ha mer informasjon, [kan du se Oppbevaringssperre for postboks](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="39094-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="39094-113">**Obs!** Hvis en postboks er mindre enn 10 MB, behandler ikke assistenten for administrert mappe postboksen automatisk.</span><span class="sxs-lookup"><span data-stu-id="39094-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="39094-114">Hvis du vil ha mer informasjon om oppbevaringspolicyer i administrasjonssenteret for Exchange, kan du se:</span><span class="sxs-lookup"><span data-stu-id="39094-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="39094-115">Oppbevaringskoder og oppbevaringspolicyer</span><span class="sxs-lookup"><span data-stu-id="39094-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="39094-116">[Bruke en oppbevaringspolicy på postbokser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) eller [Legge til eller fjerne oppbevaringskoder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="39094-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="39094-117">Slik identifiserer du typen sperring som er plassert i en postboks</span><span class="sxs-lookup"><span data-stu-id="39094-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
