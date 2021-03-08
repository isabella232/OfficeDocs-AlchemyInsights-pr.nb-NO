---
title: Tilordne en rolle i overvåkingsloggen i sikkerhets- & for Office 365
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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526524"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Tilordne en rolle i overvåkingsloggen i sikkerhets- & for Office 365

Hvis du vil søke i Office 365-overvåkingsloggen, må en administrator være tilordnet rollen Bare vise overvåkingslogger eller **overvåkingsloggrollen** i Exchange Online.  Disse rollene tilordnes som standard til rollegruppene for samsvarsadministrasjon og organisasjonsadministrasjon. Globale administratorer i Office 365 og Microsoft 365 legges automatisk til som medlemmer av rollegruppen for organisasjonsadministrasjon.

Hvis du vil at en bruker skal kunne søke med minimum tilgangsnivå, oppretter du en egendefinert rollegruppe i Exchange Online, legger til rollen Bare **overvåkingslogg** eller **overvåkingslogg,** og legger deretter til brukeren som medlem av den nye rollegruppen.

Hvis du vil ha mer informasjon, kan du se Behandle [rollegrupper i Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) og søke i overvåkingsloggen i sikkerhetssenteret [& samsvarssenteret.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)