---
title: Endre fra Microsoft-navneservere tilbake til å administrere dine egne DNS-poster
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506979"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Endre fra Microsoft-navneservere tilbake til å administrere dine egne DNS-poster

Du har tidligere endret NS-postene slik at de peker til Microsoft (ns1.bdm.microsoftonline.com), men nå har du bestemt deg for å administrere dine egne DNS-poster:

På domeneregistratorens nettsted endrer du navneserveren tilbake til registratoren eller forrige innstilling. Hvis du ikke er kjent med DNS, bør du kontakte kundestøtte hos domeneregistratoren. Vær oppmerksom på at endringer i navneserveren kan ta opptil 48 timer å overføre. 

1. Gå Microsoft 365 til Domener i **Innstillinger** administratorportalen, merk av for  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)domenet, og velg **Administrer DNS**. 

2. Velg Legg til dine egne **DNS-poster** i veiviseren, og fullfør veiviseren. Dette endrer hvordan DNS administreres, og lar deg deretter legge til de egendefinerte DNS-postene som kreves for å støtte de valgte tjenestene.

Hvis du har endret navneserverpostene til Microsoft og har et nettsted, kan du også legge til DNS-poster for nettstedet i stedet for å endre navneserverne tilbake. Hvis du vil ha mer informasjon, kan du se Oppdatere [DNS-poster for å beholde nettstedet hos gjeldende vertsleverandør.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


