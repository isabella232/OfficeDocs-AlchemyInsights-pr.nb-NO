---
title: Problemer med å logge på Microsoft 365-apper
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
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709115"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="c6175-102">Retting av Microsoft 365-appene « Datamaskinens Klarerte plattform-modul fungerer ikke som den skal»</span><span class="sxs-lookup"><span data-stu-id="c6175-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="c6175-103">For å løse denne filen kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="c6175-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="c6175-104">Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="c6175-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="c6175-105">[Fjern Office-legitimasjon ved](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) hjelp av Windows Legitimasjonsbehandling.</span><span class="sxs-lookup"><span data-stu-id="c6175-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c6175-106">**Obs!** Registerbanene for Office 2016 er endret til 16.0.</span><span class="sxs-lookup"><span data-stu-id="c6175-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c6175-107">(Eksempel: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c6175-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c6175-108">Prøv [brukergjenopprettingsprosessen for](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) å løse TPM-feil (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="c6175-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="c6175-109">Angi EnableADAL = 0 ved hjelp av følgende fremgangsmåte:</span><span class="sxs-lookup"><span data-stu-id="c6175-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="c6175-110">Høyreklikk på Start-knappen i Windows, velg **Kjør,** skriv inn **regedit** og velg deretter **OK.**</span><span class="sxs-lookup"><span data-stu-id="c6175-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="c6175-111">Velg **Ja** for å tillate at registerredigering gjør endringer på enheten.</span><span class="sxs-lookup"><span data-stu-id="c6175-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="c6175-112">Legg til en DWORD-verdi for **EnableADAL** i Registerredigering med en innstilling på **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="c6175-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="c6175-113">Hvis du vil ha mer informasjon, kan du se Tilkoblingsproblemer ved pålogging etter oppdatering til [Office 2016 bygg 16.0.7967 på Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="c6175-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>