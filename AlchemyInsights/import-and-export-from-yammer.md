---
title: Importere og eksportere fra Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036120"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="8ef35-102">Importere og eksportere fra Yammer</span><span class="sxs-lookup"><span data-stu-id="8ef35-102">Import and export from Yammer</span></span>

<span data-ttu-id="8ef35-103">**Importer**</span><span class="sxs-lookup"><span data-stu-id="8ef35-103">**Import**</span></span>

<span data-ttu-id="8ef35-104">Alternativene for brukerimport varierer avhengig av om Yammer-nettverket er i [opprinnelig modus for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)eller ikke.</span><span class="sxs-lookup"><span data-stu-id="8ef35-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="8ef35-105">**Ikke-opprinnelig modus:** Brukere kan importeres til grupper ved hjelp av Legg til fra adresseboken (grense til 100 brukere) i gruppeinnstillinger, eller til nettverket ved hjelp av masseoppdatering i Nettverksadministrator. [](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)</span><span class="sxs-lookup"><span data-stu-id="8ef35-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="8ef35-106">**Opprinnelig modus:** Operasjoner for gruppemedlemskap og nettverksmedlemskap bør utføres fra administrasjonsportalen for [Microsoft 365,](https://docs.microsoft.com/microsoft-365/admin/add-users) [Azure AD-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)eller ved hjelp av et annet Azure AD-alternativ.</span><span class="sxs-lookup"><span data-stu-id="8ef35-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="8ef35-107">Nettverk i opprinnelig modus har ikke lenger tilgang til masseoppdatering og andre eldre funksjoner.</span><span class="sxs-lookup"><span data-stu-id="8ef35-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8ef35-108">Yammer støttet aldri import av innhold fra nettverksadministratoren selv når dataeksportfunksjonen ble brukt i et annet nettverk.</span><span class="sxs-lookup"><span data-stu-id="8ef35-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="8ef35-109">Innhold kan publiseres på nytt av partnerløsninger eller YAMMER REST API-er.</span><span class="sxs-lookup"><span data-stu-id="8ef35-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="8ef35-110">**Eksporter**</span><span class="sxs-lookup"><span data-stu-id="8ef35-110">**Export**</span></span>

<span data-ttu-id="8ef35-111">[Eksporter nettverksdata i Nettverksadministrator](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) tillater eksport av innhold fra Yammer-nettverk, inkludert meldinger og filer.</span><span class="sxs-lookup"><span data-stu-id="8ef35-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="8ef35-112">Vedlegg kan være svært store, og det vil føre til at eksporten tar betydelig tid å fullføre.</span><span class="sxs-lookup"><span data-stu-id="8ef35-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="8ef35-113">Vi anbefaler at aktive nettverk eksporteres ved hjelp av [dataeksport-API-en](https://developer.yammer.com/docs/data-export-api) i biter etter dag eller uke.</span><span class="sxs-lookup"><span data-stu-id="8ef35-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="8ef35-114">Microsoft Kundestøtte tilbyr ikke egendefinerte skript til dette formålet.</span><span class="sxs-lookup"><span data-stu-id="8ef35-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="8ef35-115">Det finnes [en egen GDPR-eksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) for å eksportere innhold for en enkeltbruker.</span><span class="sxs-lookup"><span data-stu-id="8ef35-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>