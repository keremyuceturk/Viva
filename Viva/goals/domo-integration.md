---
title: "Domo Integration"
ms.reviewer: 
ms.author: vsreenivasan
author: ms-vikashkoushik
manager: <TBD>
audience: Admin
f1.keywords:
- NOCSH
ms.topic: article
ms.service: viva
ms.subservice: viva-goals
ms.localizationpriority: medium
ms.collection:  
- m365initiative-viva-goals
search.appverid:
- MET150

description: "Learn how to integrate your Domo datasets directly with Viva Goals to automate OKR success measurement."
---

# Domo integration

The Viva Goals Domo integration allows automated real-time tracking of OKR progress. 
  
Let's take this example: you use Domo cards to visualize your Sales team's close rate: Quarter-to-date (QTD) vs. Goal. By configuring a Domo integration and setting up a data link within Viva Goals, you can save the hassle of reinventing the wheel by connecting to other source sales systems, if all data integrations, aggregations and key performance indicator (KPI) visualizations have already been implemented within Domo. Viva Goals will automatically update OKR progress, saving you time and bringing all your data and progress in one place. 
  
## How to enable the Domo Integration

A Viva Goals admin can enable the Domo Integration on Viva Goals. Take the following steps: 

1. Navigate to Viva Goals’ Integrations page through **Admin > Integrations**.
  
    :::image type="content" source="../media/goals/7/viva-goals-integrations-page.png" alt-text="Integrations page in Viva Goals." lightbox="../media/goals/7/viva-goals-integrations-page.png":::

2. Enable the Domo Integration under the **Data Integrations** category.
  
    :::image type="content" source="../media/goals/7/domo-enable-button.png" alt-text="Enabling Domo in Viva Goals." lightbox="../media/goals/7/domo-enable-button.png":::

3. The integration can also be disabled at any time from the same section.
  
    :::image type="content" source="../media/goals/7/domo-disable-button.png" alt-text="Disabling Domo in Viva Goals." lightbox="../media/goals/7/domo-disable-button.png":::

## How to configure the Domo connection

In the **Connections** section, select **New Connection.** In the popup that appears, follow the prompt to configure the Domo connection using a Domo Client ID and Secret. A connection can be shared with all users or made private based on the user's preference. Editing a saved Domo connection is also allowed from the same section at any time.
  
  :::image type="content" source="../media/goals/7/domo-creating-new-connection.png" alt-text="Filling in new Domo connection details in Viva Goals." lightbox="../media/goals/7/domo-creating-new-connection.png":::

To create a Domo Client ID & Secret, visit [https://developer.domo.com/new-client](https://developer.domo.com/new-client), sign in with your Domo domain & credentials. Enter **Name** and **Description** details and select **Data** as **Application scope**.

## How to set up the Domo data link

Once the connection configuration is done, users can **Edit** their Viva Goals OKRs to set up a Data Link to directly track progress from their Domo datasets.  

> [!NOTE]
> The Domo integration is available only for **KPI (success metric)** method of measuring OKR success and not for **% completion** method.

1. While creating/editing an Objective or Key Result, select **Add an integration**. Select **Domo** from the list of integrations.
  
   :::image type="content" source="../media/goals/7/domo-from-the-list-of-datasources.png" alt-text="Selecting Domo from the list of data sources in Viva goals." lightbox="../media/goals/7/domo-from-the-list-of-datasources.png":::

2. If a Domo Connection isn't configured, Viva Goals also allows the user to configure a connection right there. If already configured, Viva Goals allows the users to proceed with setting up the data link by selecting an available connection.

3. In the popup that appears, follow the prompts to set up the Domo data link.  
  
4. Select **Connection**, key in **DataSet-ID**, your actual **KPI** from the list of measures/dimensions available on the selected dataset.
  
   :::image type="content" source="../media/goals/7/domo-new-connection-details.png" alt-text="Adding new Domo connection to OKRs in Viva goals." lightbox="../media/goals/7/domo-new-connection-details.png":::

> [!NOTE]
> To obtain the DataSet-ID: Login to your Domo instance and select the Dataset name mentioned under the card.

5. Grab the 36 character DataSet-ID from the URL of the DataSet page.

6. If there are multiple values for the KPI, and you have the Close Rate for all your sales team members as part of the Domo dataset, you can apply a function (sum/average/count) on the set of values. For example, average of Close Rate for the entire sales team.

    or

    Apply any available dataset fields as **Filters**. For example, filter a particular AE Name - Adam's Close Rate.

7. Viva Goals displays the final KPI value for your reference before saving the data link set-up.
