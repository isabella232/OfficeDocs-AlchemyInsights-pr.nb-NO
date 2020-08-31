---
title: Bruke Wix-nettstedet med Office 365-kjøpte eller administrerte domener
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300723"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Bruke Wix-nettstedet med Office 365-kjøpte eller administrerte domener

- [Oppdatere DNS-poster for å beholde nettstedet hos gjeldende verts leverandør](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix-artikkelen «koble et domene til Wix ved hjelp av peke metoden» anbefaler at du bruker peke (legge til DNS-poster i koblingen ovenfor) i stedet for å endre navneservere når du bruker Office 365
- Hvis du fremdeles velger å endre navneservere til Wix, må du  [opprette DNS-poster på Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Hvis domenet ble kjøpt fra Microsoft, kan ikke Name-serverne endres. Hvis du må endre navneservere, må Microsoft-kjøpt domene  [overføres til en annen verts leverandør etter 60 dager](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)