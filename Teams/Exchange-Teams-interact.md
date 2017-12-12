---
title: How Exchange and Microsoft Teams interact | Microsoft Support
author: LolaJacobsen
ms.author: lolaj
manager: lolaj
ms.date: 09/25/2017
ms.topic: article
ms.service: msteams
description: Learn what functionality exists between Microsoft Teams and the various Exchange setups such as creating and joining teams, creating channels, and more.
Set_Free_Tag: Strat_MT_TeamsAdmin
---

How Exchange and Microsoft Teams interact 
=========================================

For the full Microsoft Teams experience, every user should be enabled for Exchange Online, SharePoint Online, and Office 365 Group creation.

Users' Exchange mailboxes can be hosted online or on-premises. Users hosted on Exchange Online or Exchange Dedicated vNext can use all the features of Microsoft Teams. They can create and join teams and channels, create and view meetings, modify user profile pictures, add and configure connectors, tabs, and bots, and they can chat and call.

Users hosted on Exchange Online Dedicated – Legacy or Exchange on-premises must be synchronized to Azure Active Directory for Office 365. They can create and join teams and channels, add and configure tabs and bots, and chat and call. However, they can’t modify user profile pictures, create and view meetings, or add and configure connectors. They can receive messages from connectors configured by other users.

The following table provides information for users with Exchange Online hosted in various environments.

**Actions supported:** 

| User's mailbox is hosted in:   | Create teams   |Join teams|Create channels|Create and view meetings|Modify user profile picture|Add and configure connectors|Add and configure tabs|Add and configure bots|
|---|---|---|---|---|---|---|---|---|
|**Exchange Online**|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|**Exchange Online Dedicated vNext**|Yes|Yes|Yes|Yes|Yes|Yes|Yes|Yes|
|**Exchange Online Dedicated – Legacy** (Sync to Azure AD required)|Yes|Yes|Yes|No|No|No|Yes| Yes|
|**Exchange on-premises** (Sync to Azure AD required)|Yes|Yes|Yes|Yes*|No|No|Yes|Yes|
                                                            
*\*Exchange 2016 CU3 and above supported*

Additional information:

-   Microsoft Teams doesn't support SharePoint on-premises.

-   SharePoint Online is required to share and store files in team conversations.

-   OneDrive for Business is required to share and store files in private chats.

-   If users aren't assigned and enabled with SharePoint Online licenses, they don't have OneDrive for Business storage in Office 365. File sharing will continue to work in Channels, but users are unable to share files in Chats without OneDrive for Business storage in Office 365.

-   Users must be enabled for Office 365 group creation to create teams in Microsoft Teams.

-   In Microsoft Teams, security and compliance features like eDiscovery, Content Search, archiving, and legal hold work best in Exchange Online and SharePoint Online environments. For channel conversations, messages are journaled to the group mailbox in Exchange Online, where they're available for eDiscovery. If SharePoint Online and OneDrive for Business (using work or school account) are enabled across the organization and for users, these compliance features are available for all files within Teams as well.

**Important:**   Users who participate in conversations that are part of the Chat list in Microsoft Teams must have an Exchange Online (cloud-based) mailbox for an admin to search chat conversations. That's because conversations that are part of the Chat list are stored in the cloud-based mailboxes of the chat participants. If a chat participant doesn't have an Exchange Online mailbox, the admin won't be able to search or place a hold on chat conversations. For example, in an Exchange hybrid deployment, users with on-premises mailboxes might be able to participate in conversations that are part of the Chat list in Microsoft Teams. However, in this case, content from these conversations isn't searchable and can't be placed on hold because the users don't have cloud-based mailboxes. For more details about Content Searches and Microsoft Teams, see [*Microsoft Teams and Office 365 Groups*](https://support.office.com/en-us/article/Run-a-Content-Search-in-the-Office-365-Security-Compliance-Center-61852fd9-fe8a-4880-a339-cb19ed3bff4a).

**Tip:**   For information about how to use Azure AD Connect to synchronize with Azure Active Directory, see [*Integrating your on-premises identities with Azure Active Directory*](https://go.microsoft.com/fwlink/?linkid=854600).
