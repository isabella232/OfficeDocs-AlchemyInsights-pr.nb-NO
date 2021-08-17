---
title: 401 Uautorisert feil i SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314357"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Uautorisert feil i SharePoint

Hvis du får feilmeldingen «(401) Uautorisert» i SharePoint kan den være relatert til avviklingen av TLS 1.0/1.1. Hvis du vil ha mer informasjon, kan du ta en titt på:

- [Klargjøre for TLS 1.2 i Office 365 og Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Godkjenningsfeil oppstår hvis klienten ikke har støtte for TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Oppdater for å aktivere TLS 1.1 og TLS 1.2 som standard sikre protokoller i WinHTTP i Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Hvis brukerne er på Windows 7, må du kontrollere at de kontrollerer [TLS Cipher Suites i Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).