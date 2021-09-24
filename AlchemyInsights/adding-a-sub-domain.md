---
title: Legge til et underdomene
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506764"
---
# <a name="adding-a-sub-domain"></a>Legge til et underdomene

Underdomener kan legges til i samme eller en annen leier enn det overordnede domenet. I begge tilfeller må du administrere dine egne DNS-innstillinger på registratorens nettsted. Hvis du har latt Microsoft administrere DNS-innstillingene med NS-poster, eller hvis du kjøpte domenet fra Microsoft, kan du ikke legge til underdomener uten å endre dette først.

Legg til det overordnede domenet først, og legg deretter til underdomenet. Hvis underdomenet er i samme leier, er det ikke nødvendig med ytterligere bekreftelse. Hvis du legger til underdomenet i en separat leier, kreves DNS txt-posten for eierskapskontroll før du legger til domenet og de ekstra DNS-postene for de valgte tjenestene.

- Hvis du vil legge til et domene eller underdomene, følger du veiviseren legg til domene [eller](https://admin.microsoft.com/Adminportal#/Domains/Wizard)legger til domenet eller underdomenet manuelt ved å gå til **Angi**  >  **domener**  >  **Legg til domene**.

Om nødvendig:

- Hvis du vil endre hvem som administrerer DNS-innstillingene for et eksisterende domene, går du til **Innstillinger**  >  [**Domener**](https://admin.microsoft.com/Adminportal/Home#/Domains), merker av for domenet og velger **deretter Administrer DNS**. Velg Legg til dine egne **DNS-poster** i veiviseren, og fullfør veiviseren.
- Hvis du vil legge til underdomener i et Domene kjøpt av Microsoft, må du først overføre domenet til en annen registrator og deretter gjøre endringen ovenfor for å administrere dine egne DNS-poster. Hvis du vil ha instruksjoner, kan du se Overføre [et domene fra Microsoft til en annen vert](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- Hvis du får en feilmelding om at domenet allerede er i bruk av andre medlemmer eller personer i organisasjonen, må du først ta over denne uadministrerte kontoen før du bruker domenet. Hvis du vil ha instruksjoner, kan du se Overta en [uadministrert katalog som administrator i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
