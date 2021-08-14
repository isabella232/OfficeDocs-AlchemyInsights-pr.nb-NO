---
title: Løse regler for avsenderadresse/domeneliste
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bf2a36853f53c723ca620487dd1c656ecb188cba9c80def68c793e3d5fbf5f87
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930034"
---
# <a name="fix-sender-addressdomain-list-rules"></a>Løse regler for avsenderadresse/domeneliste

En policy for søppelpost i tenanten påvirket denne meldingen. Avsenderen av meldingen ble funnet i en tillatelses- eller blokkeringsliste. Gjør følgende for å se gjennom policyen:

1. Gå til Office 365 [Sikkerhets- & samsvarssenter](https://go.microsoft.com/fwlink/p/?linkid=2077143), og gå deretter til **Policy** for trusselbehandling  >    >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Hvis **Standardinnstillinger** er aktivert på **Standard-fanen,** merker du av for Tillat **lister** og **Blokker lister**.
3. Hvis **Egendefinerte** innstillinger  er aktivert på Egendefinert-fanen, kan du se gjennom policyene ved å velge Rediger **policy** og merke **av for** Tillat lister **og Blokker lister**.

Hvis du vil ha mer informasjon om hvordan du konfigurerer policyer for søppelpostfilter, kan [du se Konfigurere policyer for søppelpostfilter .](https://go.microsoft.com/fwlink/?linkid=2101431)
