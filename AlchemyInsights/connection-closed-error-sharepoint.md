---
title: Den underliggende tilkoblingen ble lukket i SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233435"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="c3cc0-102">Feilmeldingen «Den underliggende tilkoblingen ble lukket» i SharePoint</span><span class="sxs-lookup"><span data-stu-id="c3cc0-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="c3cc0-103">Hvis du får feilmeldingen «Den underliggende tilkoblingen ble lukket» i SharePoint kan den være relatert til avviklingen av TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="c3cc0-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="c3cc0-104">Hvis du vil ha mer informasjon, kan du se disse artiklene:</span><span class="sxs-lookup"><span data-stu-id="c3cc0-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="c3cc0-105">Klargjøre for TLS 1.2 i Office 365 og Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="c3cc0-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [<span data-ttu-id="c3cc0-106">Godkjenningsfeil oppstår hvis klienten ikke har støtte for TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="c3cc0-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="c3cc0-107">Hvis brukerne er på Windows 7, må du kontrollere at de kontrollerer [TLS Cipher Suites i Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span><span class="sxs-lookup"><span data-stu-id="c3cc0-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>