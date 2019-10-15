---
title: Store SharePoint-lister
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488526"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>Arbeide med store lister og biblioteker i SharePoint

SharePoint-lister og-biblioteker kan inneholde opptil 30 000 000 elementer, men når de har mer enn 5 000 elementer, kan det hende du ser en terskelverdi for listevisning når du prøver å arbeide med dem. Denne terskelen er på plass for å opprettholde ytelsen til tjenesten. Den kan ikke endres. For å unngå å treffe denne terskelen:

**Bruk moderne**

Visninger som viser mange elementer fungerer best i den moderne opplevelsen. [Bruk den moderne opplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) for å unngå feil du kan se i den klassiske opplevelsen.

**Legge til indekser**

Når du filtrerer eller sorterer etter en kolonne som ikke har en indeks, kan det hende du ser en feilmelding. [Legg til en indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **listeinnstillinger** i innstillingsmenyen, og deretter **indekserte kolonner**.

**Redigere listevisningen**

Hvis det oppstår en feil når du arbeider med en stor liste, [redigerer du listevisningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).

Følgende fire endringer vil fjerne terskel feil for listevisning. Gjør alle fire endringer for å fjerne alle feil. Hvis du fremdeles får feilmeldinger, kontrollerer du [behandle store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).

1. Velg **ingen** fra både **første sortering etter kolonnen** , og **Sorter deretter etter kolonnen**.
2. Velg **ingen** fra både **første gruppe etter kolonnen** og **grupper deretter etter kolonnen**.
3. Velg **ingen** for alle kolonnene i **Totaler** -delen.
4. Opphev markeringen av alle unntatt én kolonne for visning fra **kolonner** -delen.

