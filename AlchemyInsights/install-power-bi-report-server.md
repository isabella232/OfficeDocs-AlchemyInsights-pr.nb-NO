---
title: Installere rapportserver for Power BI
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
ms.openlocfilehash: 01cc2efc2dacc2fdf0b7b7f036bc18e1c75fd515348b72d5c4dde96949a51a2d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028589"
---
# <a name="install-power-bi-report-server"></a>Installere rapportserver for Power BI

1. Finn plasseringen av PowerBIReportServer.exe og start installasjonsprogrammet.

2. Velg **Installer rapportserver for Power BI**.

3. Velg en utgave som skal installeres, og velg deretter **Neste**.

4. Du kan velge enten Evaluering eller Utviklerutgave fra rullegardinlisten.  Ellers kan du angi en produktnøkkel for serveren du anskaffet fra enten Power BI-tjenesten eller servicesenteret for volumlisens. Hvis du vil ha mer informasjon om hvordan du får produktnøkkelen, kan du se delen Før du begynner. Les og godta lisensvilkårene, og velg deretter **Neste**.

5. Du må ha en databasemotor tilgjengelig for å lagre rapportserverdatabasen. Velg **Neste** for bare å installere rapportserveren.

6. Angi installasjonsplasseringen for rapportserveren. Velg **Installer for** å fortsette.

7. Etter en vellykket konfigurasjon velger du **Konfigurer rapportserver for** å starte Reporting Services Configuration Manager.

Du trenger ikke en SQL Server Database Engine-server som er tilgjengelig på tidspunktet for installasjonen. Du må konfigurere Reporting Services etter installasjon.

Hvis du vil ha mer informasjon: https://docs.microsoft.com/power-bi/report-server/install-report-server
