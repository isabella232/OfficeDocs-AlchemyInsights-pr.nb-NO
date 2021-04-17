---
title: Overføring fra AIP til MIP/Unified Labeling i samsvarssenteret
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825380"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Overføring fra AIP til MIP/Unified Labeling i samsvarssenteret

Hvis du vil overføre fra AIP-etiketter til Enhetlig merking i sikkerhets- og samsvarssenteret, gjør du følgende:

**Aktivere beskyttelse fra Azure-portalen**

1. Hvis du ikke allerede har gjort det, åpner du et nytt nettleservindu og [logger på Azure-portalen.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Gå til **Azure Information Protection-bladet.** Klikk for eksempel Alle tjenester på hubmenyen, **og** begynn å skrive **inn informasjon** i Filter-boksen. Velg **Azure Information Protection**. Hvis du ikke har tilgang til Azure Information Protection-bladet før, kan du se engangstrinnene for å legge til dette bladet i portalen. [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Hvis du vil åpne Azure Information Protection-bladet, må du enten ha et [Azure Information Protection Premium-abonnement](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller et Office 365-abonnement som inkluderer Rights Management. Hvis du har et av disse abonnementene, men ser en melding om at et gyldig abonnement ikke finnes, kan du kontakte [Microsoft Kundestøtte](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller bruke standard støttekanaler.

2. Finn **alternativene for** Administrer meny, og velg **Beskyttelsesaktivering**. Klikk **Aktiver**, og bekreft deretter handlingen. Når aktiveringen er fullført, viser informasjonslinjen **aktiveringen fullført.**

**Overføre Azure Information Protection-etiketter til Sikkerhets- & i Office 365**

1. Kontroller at du er logget på som en bruker med global administratortillatelse.

2. Gå til **Azure Information Protection-bladet.**

3. Velg **Enhetlig** merking fra **behandle-menyalternativet.**

4. Klikk **Aktiver på Azure Information Protection – Unified labeling** **bladet,** og følg instruksjonene på nettet.

**Obs!** Kontroller at du har de riktige tillatelsene før du aktiverer overføringen av sikkerhets- & samsvarssenteret. Se disse artiklene for mer informasjon:

1. [Må du være global administrator for å konfigurere Azure Information Protection, eller kan jeg delegere til andre administratorer?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Viktig informasjon om administrative roller etter overføring til sikkerhets- & samsvarssenteret.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Hvis du vil ha mer informasjon om AIP til Unified Labeling-overføring til sikkerhets- og samsvarssenteret, kan du se [Overføre etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
