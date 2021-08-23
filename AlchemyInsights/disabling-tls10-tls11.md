---
title: Deaktivere TLS1.0 og TLS 1.1 for SMTP AUTH-klientinnsending
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/18/2021
ms.locfileid: "58455119"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Deaktivere TLS1.0 og TLS 1.1 for SMTP AUTH-klientinnsending

Vi har nylig begynt å deaktivere TLS1.0 og TLS 1.1 for SMTP AUTH-klientinnsending. 

Hvis du har konfigurert en enhet, et program eller en server som sender e-post til Microsoft 365 ved hjelp av SMTP AUTH-klientinnsendingsmetode, må du kontrollere at enheten, programmet eller serveren støtter TLS 1.2 for SMTP. 