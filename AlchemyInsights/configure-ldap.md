---
title: Konfigurere LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885572"
---
# <a name="configure-ldap"></a><span data-ttu-id="b0e8a-102">Konfigurere LDAP</span><span class="sxs-lookup"><span data-stu-id="b0e8a-102">Configure LDAP</span></span>

<span data-ttu-id="b0e8a-103">Gjør følgende for å konfigurere LDAP:</span><span class="sxs-lookup"><span data-stu-id="b0e8a-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="b0e8a-104">Kontroller domenets tilstand på Azure- [portalen](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="b0e8a-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="b0e8a-105">Sikre at et gyldig Azure AD-abonnement er tilgjengelig, og at Azure AD Domain Services er aktivert.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="b0e8a-106">Sertifikatet som kreves for å tillate sikker LDAP, må hentes fra en klarert offentlig sertifiserings instans eller være et selv signert sertifikat.</span><span class="sxs-lookup"><span data-stu-id="b0e8a-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="b0e8a-107">Pass på at sertifikatet følger de nødvendige [retnings linjene](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="b0e8a-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="b0e8a-108">**Ugyldig sertifikat**</span><span class="sxs-lookup"><span data-stu-id="b0e8a-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="b0e8a-109">Hvis du vil fornye et sertifikat, følger du Fremgangs måten for å opprette et nytt sertifikat og laste det opp på [nytt: Konfigurere LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b0e8a-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="b0e8a-110">Hvis du vil løse kjente problemer med sikre LDAP-varsler i Azure Active Directory Domain Services, kan du se [løse LDAP-varsler](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b0e8a-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
