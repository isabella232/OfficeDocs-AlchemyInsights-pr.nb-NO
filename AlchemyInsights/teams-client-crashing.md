---
title: Krasjer Teams-klienten?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030679"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="0c7ff-102">Krasjer Teams-klienten?</span><span class="sxs-lookup"><span data-stu-id="0c7ff-102">Teams client crashing?</span></span>

<span data-ttu-id="0c7ff-103">Hvis Teams-klienten krasjer, kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="0c7ff-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="0c7ff-104">Hvis du bruker Teams skrivebordsprogram, [forsikre deg om at appen er oppdatert til siste versjon](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="0c7ff-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="0c7ff-105">Kontroller at alle [URL-adressene og adresseområdene til Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgjengelige.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="0c7ff-106">Logg på med administratorkontoen og kontroller [Tjenestetilstandsinstrumentbordet](https://docs.microsoft.com/office365/enterprise/view-service-health) for å bekrefte at ingen avbrudd eller tjenestereduksjon finnes.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="0c7ff-107">Som et siste trinn kan du prøve å slette klientens hurtigbuffer for Teams:</span><span class="sxs-lookup"><span data-stu-id="0c7ff-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="0c7ff-108">Gå helt ut av skrivebordsklienten for Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="0c7ff-109">Du kan høyreklikke på **Teams** fra ikonstatusfeltet og klikke **Avslutt**eller Kjør oppgavebehandling og avslutt prosessen helt.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="0c7ff-110">Gå til Filutforsker, og skriv inn %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="0c7ff-111">Når du er i katalogen, ser du noen av følgende mapper:</span><span class="sxs-lookup"><span data-stu-id="0c7ff-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="0c7ff-112">Gå til **Appbuffer** under Hurtigbuffer, og slett filene i hurtigbufferen: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="0c7ff-113">Slett alle filer i **Blob_lagring**: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="0c7ff-114">Slett alle filer i **Cache**: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="0c7ff-115">Slett alle filer i **databaser**: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="0c7ff-116">Slett alle filer i **GUPUCache**: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="0c7ff-117">Slett alle filer i **IndeksertDB**: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="0c7ff-118">Slett alle filer i **Lokal lagring**: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="0c7ff-119">Til slutt, slett alle filer i **tmp**: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="0c7ff-120">Start Teams-klienten på nytt.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-120">Restart your Teams client.</span></span>
