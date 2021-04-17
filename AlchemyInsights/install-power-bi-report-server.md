---
title: Installere Rapportserver for Power BI
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832103"
---
# <a name="install-power-bi-report-server"></a>Installere Rapportserver for Power BI

1. Finn plasseringen av PowerBIReportServer.exe og start installasjonsprogrammet.

2. Velg **Installer Power BI Report Server**.

3. Velg en utgave som skal installeres, og velg deretter **Neste**.

4. Du kan velge enten Evaluering eller Utviklerutgave fra rullegardinlisten.  Ellers kan du angi en produktnøkkel for serveren du anskaffet fra Power BI-tjenesten eller servicesenteret for volumlisens. Hvis du vil ha mer informasjon om hvordan du får produktnøkkelen, kan du se delen Før du begynner. Les og godta lisensvilkårene, og velg deretter **Neste**.

5. Du må ha en databasemotor tilgjengelig for å lagre rapportserverdatabasen. Velg **Neste** for bare å installere rapportserveren.

6. Angi installasjonsplasseringen for rapportserveren. Velg **Installer for** å fortsette.

7. Etter en vellykket konfigurasjon velger du **Konfigurer rapportserver for** å starte Reporting Services Configuration Manager.

Du trenger ikke en SQL Server Database Engine-server som er tilgjengelig på tidspunktet for installasjonen. Du må konfigurere Reporting Services etter installasjon.

Hvis du vil ha mer informasjon: https://docs.microsoft.com/power-bi/report-server/install-report-server
