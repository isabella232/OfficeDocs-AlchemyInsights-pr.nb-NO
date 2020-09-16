---
title: Overføring fra det administrative alternativet til MIP/Unified-merking i Samsvars senteret
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674335"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Overføring fra det administrative alternativet til MIP/Unified-merking i Samsvars senteret

Hvis du vil overføre fra brukerførte etiketter til enhetlig merking i sikkerhets-og Samsvars senteret, gjør du følgende:

**Aktivere beskyttelse fra Azure-portalen**

1. Hvis du ikke allerede har gjort det, åpner du et nytt nett leser vindu og [logger deg på Azure-portalen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Gå til blad for **Azure Information Protection** . Klikk for eksempel **alle tjenester** på hub-menyen, og begynn å skrive inn **informasjon** i Filter-boksen. Velg **Azure Information Protection**. Hvis du ikke har brukt Azure Information Protection blad før, kan du se [ytterligere trinn](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) for å legge til dette Bladt i portalen. Hvis du vil åpne blad for Azure Information Protection, må du ha enten en [Azure Information Protection Premium-plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) eller en Office 365-plan som inkluderer rettighets administrasjon. Hvis du har et av disse abonnementene, men ser en melding om at et gyldig abonnement ikke blir funnet, kan du [kontakte Microsoft kunde støtte](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) eller bruke standard støtte kanaler.

2. Finn alternativer for **Administrer** -menyen, og velg deretter **beskyttelses aktivering**. Klikk **Aktiver**, og bekreft deretter handlingen. Når aktiveringen er fullført, viser informasjons linjen **aktivering**er fullført.

**Overføre etiketter for Azure Information Protection til Office 365 sikkerhets & Samsvars senter**

1. Kontroller at du er logget på som bruker med global administrator tillatelse.

2. Gå til blad for **Azure Information Protection** .

3. Velg **Unified labelion**på **Manage** Menu-alternativet.

4. Klikk **Aktiver** i det elektroniske utvelgings blad for **Azure Information Protection** , og følg instruksjonene.

**Obs**! Kontroller at du har de nødvendige tillatelsene før du aktiverer sikkerhets & av samsvars senteret. Se disse artiklene for mer informasjon:

1. [Trenger du å være en global administrator for å konfigurere Azure Information Protection, eller kan jeg delegere til andre administratorer?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Viktig informasjon om administrative roller etter overgangen til sikkerhets & Samsvars senter.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Hvis du vil ha mer informasjon om overføring av sikkerhets-og Samsvars senteret for det administrative alternativet, kan du se [overføre etiketter](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
