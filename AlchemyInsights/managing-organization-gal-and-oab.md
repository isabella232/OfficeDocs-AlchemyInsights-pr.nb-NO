---
title: Administrere global adresseliste og frakoblet adressebok for organisasjoner
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794841"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="18941-102">Administrere global adresseliste (GAL) og frakoblet adressebok (OAB) for organisasjoner</span><span class="sxs-lookup"><span data-stu-id="18941-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="18941-103">En global adresseliste (GAL) er en liste over e-postaktiverte objekter (en hvilken som helst type mottaker som kan motta en e-postmelding) i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="18941-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="18941-104">Én GAL blir automatisk opprettet i hver organisasjon.</span><span class="sxs-lookup"><span data-stu-id="18941-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="18941-105">Du kan opprette flere GAL-er til å skille brukere etter organisasjon eller sted, men én enkelt bruker kan bare se og bruke én GAL om gangen.</span><span class="sxs-lookup"><span data-stu-id="18941-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="18941-106">Enkelte e-postklienter, for eksempel Outlook for Windows, laster ned GAL-en til frakoblet bruk.</span><span class="sxs-lookup"><span data-stu-id="18941-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="18941-107">Dette kalles en frakoblet adressebok (OAB).</span><span class="sxs-lookup"><span data-stu-id="18941-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="18941-108">I Exchange Online oppdateres en OAB bare én gang hver 8. time, og deretter må kundene laste den ned for å oppdatere sin lokale OAB-kopi.</span><span class="sxs-lookup"><span data-stu-id="18941-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="18941-109">Eventuelle endringer av mottakere må først være synlig i GAL for senere å komme med i OAB.</span><span class="sxs-lookup"><span data-stu-id="18941-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="18941-110">Her er noen vanlige GAL- og OAB-prosedyrer:</span><span class="sxs-lookup"><span data-stu-id="18941-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="18941-111">Det kan være en rekke årsaker til at du vil at noen av objektene skal være skjult fra GAL.</span><span class="sxs-lookup"><span data-stu-id="18941-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="18941-112">Se [Skjul mottakere fra adresselister](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="18941-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="18941-113">Hvis du trenger å gi bestemte brukergrupper tilpassede visninger av organisasjonens GAL, kan du se [Adressebok-policyer i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="18941-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="18941-114">[Opprett en global adresseliste i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list), og for å lære hvordan du arbeider med globale tillatelser, kan du se [Adresselister i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="18941-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="18941-115">Vær oppmerksom på at hvis du oppretter nye GAL-er, vil du kanskje også opprette en ny OAB.</span><span class="sxs-lookup"><span data-stu-id="18941-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="18941-116">Se [prosedyrer for Frakoblet adressebok](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="18941-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
