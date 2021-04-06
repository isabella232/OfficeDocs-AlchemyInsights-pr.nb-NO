---
title: Installere Office og OneDrive på Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595845"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installere Office og OneDrive på Windows Virtual Desktop

1. [Klargjøre og tilpasse et hovedbilde av VHD](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Opprett en virtuell maskin (VM) hvis den ikke allerede er opprettet.

1. [Installer Office i modus for aktivering av delt datamaskin](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). Aktivering av delt datamaskin gir flere brukere tilgang til Office.

1. [Installer OneDrive i maskinmodus](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode). Vanligvis er OneDrive installert per bruker, men her bør det installeres per maskin.