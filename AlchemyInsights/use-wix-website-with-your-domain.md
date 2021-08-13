---
title: Bruke Wix-nettsted med Office 365 eller administrerte domener
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
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980186"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Bruke Wix-nettsted med Office 365 eller administrerte domener

- [Oppdater DNS-poster for å beholde nettstedet hos gjeldende vertsleverandør](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix-artikkelen «Koble et domene til Wix Ved hjelp av pekemetoden» anbefales det å bruke pekemetode (legge til DNS-poster per koblingen ovenfor) i stedet for å endre navneservere når du bruker Office 365
- Hvis du fortsatt velger å endre navneservere til Wix, må du opprette  [DNS-poster på Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Hvis domenet ble kjøpt fra Microsoft, kan ikke navneserverne endres. Hvis du må endre navneservere, må Microsoft-domenet overføres til en annen  [vertsleverandør etter 60 dager](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)