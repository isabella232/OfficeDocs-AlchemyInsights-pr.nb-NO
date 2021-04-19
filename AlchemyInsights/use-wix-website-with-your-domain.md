---
title: Bruke Wix-nettsted med Office 365 kjøpt eller administrert domener
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
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825956"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Bruke Wix-nettsted med Office 365 kjøpt eller administrert domener

- [Oppdater DNS-poster for å beholde nettstedet hos gjeldende vertsleverandør](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix-artikkelen «Koble et domene til Wix Ved hjelp av pekemetoden» anbefales det å bruke pekemetode (legge til DNS-poster per koblingen ovenfor) i stedet for å endre navneservere når du bruker Office 365
- Hvis du fortsatt velger å endre navneservere til Wix, må du opprette  [DNS-poster på Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Hvis domenet ble kjøpt fra Microsoft, kan ikke navneserverne endres. Hvis du må endre navneservere, må Microsoft-domenet overføres til en annen  [vertsleverandør etter 60 dager](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)