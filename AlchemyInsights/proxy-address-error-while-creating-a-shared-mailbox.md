---
title: Proxy-adressefeil ved oppretting av en delt postboks
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568299"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="9a122-102">Proxy-adressefeil under oppretting av en postboks eller et annet e-postaktivert objekt</span><span class="sxs-lookup"><span data-stu-id="9a122-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="9a122-103">Hvis du prøvde å opprette et e-postaktivert objekt (postboks, delt postboks og så videre) og fikk feilmeldingen «Proxy-adressen «SMTP:alias@domain.com» er allerede i bruk...», er e-postadressen du valgte allerede tatt av et annet e-postaktivert objekt i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="9a122-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="9a122-104">Du må finne brukeren, gruppen, den delte postboksen eller fellesmappen som har denne e-postadressen, og slette den eller endre e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="9a122-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="9a122-105">Deretter kan du opprette et nytt e-postaktivert objekt med den frigjorte e-postadressen.</span><span class="sxs-lookup"><span data-stu-id="9a122-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="9a122-106">Bruk Søk på hjemmesiden for å finne den.</span><span class="sxs-lookup"><span data-stu-id="9a122-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="9a122-107">Du kan også bruke følgende Exchange Online PowerShell-kommando for å søke etter den:</span><span class="sxs-lookup"><span data-stu-id="9a122-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="9a122-108">Hvis du ikke vil slette den eksisterende e-postadressen, velger du en ny e-postadresse for det nye objektet du oppretter.</span><span class="sxs-lookup"><span data-stu-id="9a122-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  