---
title: Feilsøke sikkerhetstipset for kontroller for oppdagelse av svindel
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
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504992"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Feilsøke sikkerhetstipset for kontroller for oppdagelse av svindel

Hvis du får et sikkerhetstips som sier "Avsenderen mislyktes våre svindel deteksjon sjekker og kan ikke være den de ser ut til å være", så avsenderen ikke klarte å passere enten DKIM eller SPF godkjenning sjekker. Den beste metoden for å løse dette er for avsenderen å autorisere seg selv. Hvis avsenderen sender på dine vegne, må du autorisere dem ved å legge til avsenderens IP-adresse i SPF-posten din.
  
Se [Feilsøke det røde (mistenkelige) sikkerhetstipset for svindeldeteksjonskontroller](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for mer informasjon.
  
Her er noen andre koblinger som kan hjelpe:
  
- [Hvordan Microsoft bruker rammeverket for avsenderpolicy (SPF) til å hindre etterligning](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurere SPF for å forhindre etterligning](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
