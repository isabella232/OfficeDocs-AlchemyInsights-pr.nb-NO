---
title: Tilordne en rolle i overvåkingsloggen i sikkerhets- & i Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749517"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Tilordne en rolle i overvåkingsloggen i sikkerhets- & i Office 365

Hvis du vil søke i office 365-overvåkingsloggen, må en administrator tilordnes rollen Bare **overvåkingslogger** eller rollen **Overvåkingslogger** i Exchange Online. Disse rollene er som standard tilordnet rollegruppene Samsvarsbehandling og Organisasjonsbehandling. Globale administratorer i Office 365 og Microsoft 365 legges automatisk til som medlemmer av rollegruppen organisasjonsbehandling.

Hvis du vil at en bruker skal kunne søke med minimum tilgangsnivå, oppretter du en egendefinert rollegruppe i Exchange Online, legger til rollen Bare overvåkingslogger eller **Overvåkingslogger,** og deretter legger du til brukeren som medlem av den nye rollegruppen. 

Hvis du vil ha mer informasjon, kan du se Administrere [rollegrupper i Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) og Søke i overvåkingsloggen [i sikkerhets- & samsvarssenteret](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).