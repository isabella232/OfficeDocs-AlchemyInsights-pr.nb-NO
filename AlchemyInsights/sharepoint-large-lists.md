---
title: Store lister i SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720142"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbeide med store lister og biblioteker i SharePoint

SharePoint-lister og-biblioteker kan inneholde opptil 30 000 000 elementer, men når de har mer enn 5 000 elementer, kan det hende at det vises en terskel feil for liste visning når du prøver å arbeide med dem. Denne terskelen er der for å opprettholde ytelsen til tjenesten. Den kan ikke endres. Slik unngår du å treffe denne terskelen:

**Bruke moderne**

Visninger som viser mange elementer fungerer best i den moderne opplevelsen. [Bruk den moderne opplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) til å unngå feil du kan se i den klassiske opplevelsen.

**Legge til indekser**

Når du filtrerer eller sorterer etter en kolonne som ikke har en indeks, kan du se en feil melding. [Legg til en indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **liste innstillinger** på Innstillinger-menyen, og deretter **indekserte kolonner**.

**Redigere liste visningen**

Hvis det oppstår en feil når du arbeider med en stor liste, kan [du redigere liste visningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Følgende fire endringer vil fjerne terskel feil for liste visning. Gjør alle de fire endringene for å fjerne alle feil. Hvis du fortsatt får feil, må du kontrollere [behandle store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Velg **ingen** fra **den første Sorter etter kolonnen** , og **Sorter deretter etter kolonnen**.
2. Velg **ingen** fra **den første gruppen av kolonnen** , og **grupper deretter etter kolonnen**.
3. Velg **ingen** for alle Kol Onnene i **Totaler** -delen.
4. Fjern merket for alle unntatt én kolonne for visning fra **kolonner** -delen.

