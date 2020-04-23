---
title: Feilsøke sikkerhetstipset for kontroller for svindelregistrering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759521"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Feilsøke sikkerhetstipset for kontroller for svindelregistrering

Hvis du får et sikkerhetstips som sier "Avsenderen mislyktes våre svindel deteksjon sjekker og kan ikke være den de ser ut til å være", så avsenderen klarte ikke å passere enten DKIM eller SPF autentisering sjekker. Den beste metoden for å løse dette er for avsenderen å autorisere seg selv. Hvis avsenderen sender på dine vegne, må du godkjenne dem ved å legge til avsenderens IP-adresse i SPF-posten.
  
Se [Feilsøke det røde (mistenkelige) sikkerhetstipset for svindeldeteksjonskontroller](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for mer informasjon.
  
Her er noen andre koblinger som kan hjelpe:
  
- [Hvordan Microsoft bruker rammeverket for avsenderpolicy (SPF) til å forhindre forfalskning](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurer SPF for å forhindre forfalskning](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
