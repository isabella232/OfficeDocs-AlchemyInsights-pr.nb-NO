---
title: Send som Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872000"
---
# <a name="send-as-microsoft-365-group"></a>Send som Microsoft 365-gruppe

Du kan tilordne Send som-tillatelser slik at bestemte brukere kan sende meldinger som en Microsoft 365-gruppe:  

1. Koble til Exchange Online PowerShell.  

2. Kjør følgende kommando:  

    Legg til RecipientPermission- `<GroupName>` trustee `<MailboxName>` -AccessRights SendAs

Hvis du vil ha mer informasjon, kan du se [tillate at medlemmer sender som eller sender på vegne av en gruppe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).