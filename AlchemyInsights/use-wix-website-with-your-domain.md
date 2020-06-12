---
title: Bruke Wix-nettstedet med Office 365 kjøpte eller administrerte domener
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
ms.openlocfilehash: 64dfe6082bea1e468eae78bf1576fde398e4c28a
ms.sourcegitcommit: 3ca312535d950105ee829e037f0ff8f1ddbbae72
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/11/2020
ms.locfileid: "44708495"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Bruke Wix-nettstedet med Office 365 kjøpte eller administrerte domener

- [Oppdater DNS-poster for å beholde nettstedet ditt hos din nåværende vertsleverandør](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix-artikkelen "Koble et domene til Wix ved hjelp av pekemetoden" anbefaler å bruke peker (legge til DNS-poster per koblingen ovenfor) i stedet for å endre navneservere når du bruker Office 365
- Hvis du fortsatt velger å endre navneservere til Wix, må du [opprette DNS-poster på Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Hvis domenet ble kjøpt fra Microsoft, kan ikke navneserverne endres. Hvis du må endre navneservere, må Microsoft-kjøpte domenet [overføres til en annen vertsleverandør etter 60 dager](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)