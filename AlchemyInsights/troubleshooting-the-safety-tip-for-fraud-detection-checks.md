---
title: Feilsøking av sikkerhetstips for gjenkjenning av svindel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955975"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Feilsøking av sikkerhetstips for gjenkjenning av svindel

Hvis du får en sikkerhetstips som sier «Avsenderen mislyktes med å oppdage svindel og er kanskje ikke den de ser ut til å være», kan avsenderen ikke sende enten DKIM- eller SPF-godkjenningskontroller. Den beste metoden for å løse dette er at avsenderen kan godkjenne seg selv. Hvis avsenderen sender på dine vegne, må du godkjenne dem ved å legge til avsenderens IP-adresse i SPF-posten.
  
Se [Feilsøke røde (mistenkelige)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) sikkerhetstips for gjenkjenning av svindel for mer informasjon.
  
Her er noen andre koblinger som kan hjelpe deg:
  
- [Slik bruker Microsoft rammeverket for avsenderpolicy (SPF) til å forhindre forfalsling](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurere SPF for å forhindre forfalsling](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
