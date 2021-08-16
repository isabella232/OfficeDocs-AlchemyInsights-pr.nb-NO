---
title: Finn ut hvem som konfigurerte videresending på en postboks, og hvordan
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988215"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Finn ut hvem som konfigurerte videresending på en postboks, og hvordan

Hvis ekstern videresending ble angitt på en postboks, overvåkes aktiviteten som en del av Set-Mailbox cmdleten. Slik finner du aktiviteten i overvåkingsloggen:

1. Gå til [Office 365 Sikkerhets- & Samsvarssenter](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Velg **Søk i** >  **overvåkingslogg for søk**.
    > [!NOTE]
    > Hvis du ser et varsel om at du må aktivere overvåking, kan du aktivere den nå. Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.
1. Kontroller at **Aktiviteter-feltet** er satt til **Vis resultater for alle aktiviteter** (standard). Angi datointervallet. Du trenger ikke å angi et brukernavn.
1. Velg **Søk**. Aktivitetene vises under **Resultater**.
1. Velg **Filterresultater**, og angi **deretter Set-mailbox** i Aktivitetsfilter-feltet.  Dette returnerer alle **Set-Mailbox-aktiviteter.**
1. Hvis du vil vise detaljene, velger du en aktivitet og velger **deretter Mer informasjon**. Under **Parametere** kan du se e-postadressen for videresending som ble angitt i postboksen. **Bruker-ID-en** representerer brukeren som konfigurerte ekstern videresending på postboksen.
Hvis du vil ha mer informasjon, [kan du se Søke i Office 365 for å feilsøke vanlige scenarier](https://go.microsoft.com/fwlink/?linkid=2103944).