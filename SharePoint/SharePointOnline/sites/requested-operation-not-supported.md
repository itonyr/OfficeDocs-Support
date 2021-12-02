---
title: Site deletion error The requested operation is not supported for site
description: When you try to delete a site using the SharePoint management shell, you encounter this error.
author: PramodBalusu
manager: dcscontentpm
localization_priority: Normal
search.appverid: 
- MET150
audience: ITPro
ms.prod: sharepoint-server-itpro
ms.topic: article
ms.custom: 
- CSSTroubleshoot
- CI 158139
ms.author: v-matthamer
appliesto:
- SharePoint Online
---

# Site deletion error: “The requested operation is not supported for site”  

When you try to delete a site using the `Remove-SPOSite` command in the SharePoint Management shell, you encounter the following error:

> The requested operation is not supported for site

The error occurs because the site is included in an eDiscovery hold or retention policy that is blocking deletion.

If you must delete the site, you can remove or exclude the site from the retention policy using the steps provided in [Exclude or remove sites from a SharePoint Online retention policy](../administration/exclude-sites-from-retention-policy.md).