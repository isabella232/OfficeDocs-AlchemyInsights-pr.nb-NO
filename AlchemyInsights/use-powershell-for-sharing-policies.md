---
title: Bruke PowerShell for deling av policyer og organisasjonsrelasjoner
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709475"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Bruke PowerShell for deling av policyer og organisasjonsrelasjoner


Se gjennom den detaljerte syntaksen og parameterinformasjonen for organisasjonsrelasjoner : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  OG  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

For å opprette policy for deling, bruk [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). For å  [bruke en policy for deling på en postboks eller bruker](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  må du bruke en kombinasjon av  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) og [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) sammen med policyen som ble opprettet. For å  [endre, deaktivere eller fjerne en policy for deling](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  må du bruke  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) og [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**For full forståelse av dette emnet kan du lese:**

[Deling i Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)