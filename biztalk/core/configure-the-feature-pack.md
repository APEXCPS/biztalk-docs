---
title: "Configure the feature pack | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""

ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 1027bfa6-49b9-4f58-a2e2-3e0ae2fc3bf3
caps.latest.revision: 15
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Configure the feature pack
## Overview

[!INCLUDE[btsBizTalkServerNoVersion_md](../includes/btsbiztalkservernoversion-md.md)] uses feature packs to provide improvements, features, and closer integration with Azure. These feature packs extend functionality in key areas, such as deployment, analytics, and runtime. 

> [!NOTE]
> The feature packs are available with the Enterprise and Developer editions of [!INCLUDE[bts2016_md](../includes/bts2016-md.md)] when: 
> 
> - Used with Software Assurance (SA)  
> - Running [!INCLUDE[btsBizTalkServerNoVersion_md](../includes/btsbiztalkservernoversion-md.md)] in Azure using an Enterprise Agreement
> 
> The feature packs are not available for any other [!INCLUDE[btsBizTalkServerNoVersion_md](../includes/btsbiztalkservernoversion-md.md)] edition, or any other [!INCLUDE[btsBizTalkServerNoVersion_md](../includes/btsbiztalkservernoversion-md.md)] version. 

## Download and install

Download the [!INCLUDE[bts2016_md](../includes/bts2016-md.md)] [Feature Pack 1](https://www.microsoft.com/download/details.aspx?id=55100).

#### Install

1. Run setup as administrator.
2. In **Welcome**, select **Next**. 
3. Accept the license agreement, and select **Next**. 
4. Continue with the installation. During the install, several command windows may open and close. When complete, you are prompted to **Finish**.

A setup log is created in `C:\ProgramData\Microsoft\E-Business Servers Updates\Updates\Uninstall4014788-FP2\setup.log`.

## Feature Pack 2 updates

#### API-M Integration
#### Event Hub adapter for both send and receive
#### BizTalk backup to Azure Blobs
#### Multi machine deployment in ALM

#### [Use Service Bus partition key](../core/sb-messaging-adapter.md)

The Service Bus adapter supports Service Bus Premium, including sending messages to partitioned queues and topics. [Service Bus Premium and Standard messaging tiers](https://docs.microsoft.com/azure/service-bus-messaging/service-bus-premium-messaging) details more about Service Bus Premium. 

#### TLS 1.2 
#### HL7 runtime ready to support 2.7.1
#### JSON encode/decode supporting latest Newton Soft 



## Feature Pack 1 updates

#### [Send tracking data to Application Insights](../core/send-tracking-data-to-azure-application-insights-using-biztalk-server.md)

Send tracking data to Azure Application Insights to use its features, such as analytics, machine learning, diagnostics, and more. 

#### [Configure the operational data feed using Power BI](../core/configure-the-operational-data-feed-for-power-bi-with-biztalk-server.md)

Send tracking data to Power BI using oData. For example, get a visual representation of your tracking data from your ports and orchestrations. 

#### [Connect to the management REST APIs in BizTalk](../core/install-and-configure-the-management-rest-apis-in-biztalk-server.md)

Use REST APIs to remotely manage your BizTalk artifiacts, including agreements, suspended instances, unenlisted orchestrations, and more.

#### [Configure advanced scheduling](../core/configure-the-time-zone-and-recurrence-scheduling-in-biztalk-server.md)

Enable advanced scheduling in your receive locations. For example, set the timezone, or set a recurrence service window for a specific day on a specific month.

#### [Configure automatic deployments with VSTS](../core/configure-automatic-deployment-with-visual-studio-team-services-in-biztalk.md)  

Use Visual Studio Team Services (VSTS) to automatically deploy your solutions, or update existing applications. VSTS communicates with an agent installed on the [!INCLUDE[btsBizTalkServerNoVersion_md](../includes/btsbiztalkservernoversion-md.md)].

#### [Connect to SQL Server Always Encrypted columns with BizTalk Server](../core/connect-to-sql-server-always-encrypted-columns-with-biztalk-server.md)  

Use the WCF-SQL adapter to query encrypted columns from an Always Encrypted database in SQL Server.

