---
title: 'AIP: Topptekster og bunntekster vises ikke som forventet'
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
- "9002266"
- "4541"
ms.openlocfilehash: 5f50fc1d38618017bca61b4e9290d9893983534e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821708"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a>AIP: Topptekster og bunntekster vises ikke som forventet

Hvis du har problemer med visuelle markeringer som ikke vises som forventet, kan du se følgende retningslinjer:

1. Kontroller at du har gjennomgått [Når visuelle markeringer brukes](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Se gjennom Når [Office 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)bruker innholdsmerking og kryptering for Office-merking.
3. Hvis du vil fjerne eksisterende topp-/bunntekster, kan du se Fjerne topptekster og [bunntekster fra andre etikettløsninger.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)

Hvis du fremdeles har problemet, kan du samle inn Azure Information Protection-klientlogger og legge ved de eksporterte loggene i denne billetten.

**Eksportere Azure Information Protection-logger**

1. Åpne et Office-dokument eller opprett en ny e-post i Outlook.
2. Klikk på **Beskytt/følsomhet** > **Hjelp og tilbakemelding**.
3. Klikk på **Eksporter logger**.
4. Lagre loggene på ønsket plassering, og legg dem ved denne serviceforespørselen.

Hvis du vil ha mer informasjon, kan du se:

- [Slik konfigurerer du en etikett for visuelle markeringer for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Gå gjennom Azure Information Protection-dokumentasjon](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Krav for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Hurtigstartveiledning for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Last ned Azure Information Protection-klient](https://www.microsoft.com/download/details.aspx?id=53018)
