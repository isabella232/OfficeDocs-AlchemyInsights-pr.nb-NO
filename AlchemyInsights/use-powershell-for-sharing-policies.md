---
title: Bruke PowerShell for delingspolicyer og organisasjonsrelasjoner
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862150"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Bruke PowerShell for delingspolicyer og organisasjonsrelasjoner


For organisasjonsforhold kan du se gjennom detaljert syntaks og parameterinformasjon for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Hvis du vil opprette delingspolicy, bruker [du New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Hvis du vil [bruke en delingspolicy på en postboks eller bruker,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) må du bruke en kombinasjon av [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) og [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) med den nylig opprettede policyen. Hvis du vil [endre, deaktivere eller fjerne en delingspolicy,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) må du bruke [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) og [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**For full forståelse av dette emnet kan du lese:**

[Deling i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)