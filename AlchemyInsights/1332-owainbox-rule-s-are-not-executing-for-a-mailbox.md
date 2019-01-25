---
title: 1332 OWA - innboks-regler ikke utføres for en bestemt postboks
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482169"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En regel som ikke virker som forventet

Kontroller følgende innstillinger:
  
- En melding kan omadresseres videresendte og besvarte automatisk basert på innboksregler bare én gang. En omadresserer regel (en Innboksregel eller flyt-post, også kjent som regel en transport) kan legge til opptil ti videresending mottakere på en melding. Hvis du vil ha mer informasjon, kan du se [Journal, Transport, og innboksen grenser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Innboksregler fungerer ikke på alternative loggføring postboksen. Hvis du vil ha mer informasjon om alternative loggføring postboksen, kan du se [alternative loggføring postboks](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Hvis du vil løse disse problemene, kan du se [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Hvis de ovenstående problemene ikke bruker, kjører du innboksen regelen diagnoserapporten før du eskalere problemet til Microsoft Support:
  
1. Åpne postboksen i Outlook på weben, og klikk **Innstillinger** \> **Alternativer** \> **Ordne e-post** \> **innboksregler**.
    
2. Nederst på siden, klikker du **Hvis reglene ikke virker på Klikk her for å generere en rapport**.
    

