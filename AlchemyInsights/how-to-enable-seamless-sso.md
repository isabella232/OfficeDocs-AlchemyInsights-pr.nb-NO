---
title: Slik aktiverer du sømløst SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780536"
---
# <a name="how-to-enable-seamless-sso"></a>Slik aktiverer du sømløst SSO

Aktiver sømløs SSO gjennom [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Hvis du vil utføre en ny installasjon av Azure AD Connect, velger du den [egen definerte installasjons banen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). Velg alternativet **Aktiver enkel pålogging** på **bruker påloggings** siden.
  
Slik kontrollerer du at du har aktivert sømløs SSO på riktig måte:
  
1. Logg deg på det [administrative senteret for Azure Active Directory](https://aad.portal.azure.com) som global administrator.

2. Velg **Azure Active Directory** i den venstre ruten.

3. Kontroller at en sømløs enkel pålogging er **aktivert**.

Hvis du vil ha mer informasjon, kan du se [Azure Active Directory sømløs enkel pålogging: hurtigst Art](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  