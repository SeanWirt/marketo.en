---
unique-page-id: 2360368
description: Configure Marketo Sales Insight in Salesforce Enterprise/Unlimited - Marketo Docs - Product Documentation
title: Configure Marketo Sales Insight in Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
---
# Configure Marketo Sales Insight in Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Here are the steps you need to take to configure Marketo Sales Insight in Salesforce Enterprise/Unlimited Editions. Let's get started.

>[!PREREQUISITES]
>
>[Install Marketo Sales Insight Package in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Admin Permissions Required**

## Configure Sales Insight in Marketo {#configure-sales-insight-in-marketo}

1. Obtain your MSI credentials in Marketo. Go to the Admin area and select **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Click **Edit API Configuration**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Enter an API Secret Key of your choosing and click **Save**. Do NOT use an ampersand (&) in your API Secret Key.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Your API Secret Key is like a password for your organization and should be secure.

1. Click **View** in the Rest API Configuration panel to populate the credentials.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. You will see a confirmation pop-up. Click **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Keep this window open. You'll need this information later in Salesforce.

## Configure Sales Insight in Salesforce {#configure-sales-insight-in-salesforce}

1. In Salesforce, click **Setup**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Search for “remote site" and select **Remote Site Settings**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Click **New Remote Site**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Enter the Remote Site Name (it can be something like “MarketoSoapAPI”). Enter Remote Site URL, which is your Marketo Host URL from the Soap API Configuration panel in Marketo. Click **Save**. You have now created remote site settings for Soap API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Click **New Remote Site** again.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Enter the Remote Site Name (it can be something like “MarketoAPI”). Enter Remote Site URL, which is your API URL from Rest API Configuration panel in Marketo. Click **Save**. You have now created remote site settings for Rest API.

   >[!NOTE]
   >
   >_You_ choose your **Remote Site Name** (MarketoAPI is used here). The **Remote Site URL** can be found in the Marketo Host field of your Edit API Configuration dialog box from Step 3 in the "Configure Sales Insight in Marketo" section.

## Customize Page Layouts {#customize-page-layouts}

1. Click **Setup**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Search for "page layout" and select the **Page Layout** under **Leads**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Click **Visualforce Pages** on the left. Drag **Section** to the layout underneath Custom Links section.
  
   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Enter "Marketo Sales Insight" as the **Section Name**. Select **1-Column** and click **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Drag and drop **Lead** into the new section.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >The name of this box will change based on the object type. For example, if you are modifying the page layout for Contacts, it will say Contact.

1. Double-click on the **Lead** block that you just added.
  
   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Edit height to **450** pixels and click **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Check **Show scrollbars** if you need access to scroll-through activities.

   >[!TIP]
   >
   >We recommend a height of 410 pixels for the Accounts and Opportunities objects.

1. Click on **Fields** on the left. Then search and drag the **Urgency** label into the **Marketo Sales Insight** layout.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Repeat the above step for these fields as well.

   <table> 
    <tbody> 
     <tr> 
      <td>Last Interesting Moment</td> 
     </tr> 
     <tr> 
      <td>Last Interesting Moment Date</td> 
     </tr> 
     <tr> 
      <td>Last Interesting Moment Desc</td> 
     </tr> 
     <tr> 
      <td>Last Interesting Moment Source</td> 
     </tr> 
     <tr> 
      <td>Last Interesting Moment Type</td> 
     </tr> 
     <tr> 
      <td>Last Marketo Activity by Sales</td> 
     </tr> 
     <tr> 
      <td>Last Marketo Engagement by Sales</td> 
     </tr> 
     <tr> 
      <td>MSI Contact Id</td> 
     </tr> 
     <tr> 
      <td>Relative Score</td> 
     </tr> 
     <tr> 
      <td>Relative Score Value</td> 
     </tr> 
     <tr> 
      <td>Urgency</td> 
     </tr> 
     <tr> 
      <td>Urgency Value</td> 
     </tr> 
     <tr> 
      <td>View in Marketo</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save** when finished.
  
   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repeat steps 5-7 to add Visualforce page sections and Sales Insight fields for **Contact**, **Account** and **Opportunity**.

1. Repeat steps 8-10 to add Sales Insight fields from the list below for **Contact**. Be sure to save any changes.

<table> 
    <tbody> 
     <tr> 
      <td>Last Interesting Moment</td> 
     </tr> 
     <tr> 
      <td>Last Interesting Moment Date</td> 
     </tr> 
     <tr> 
      <td>Last Interesting Moment Desc</td> 
     </tr> 
     <tr> 
      <td>Last Interesting Moment Source</td> 
     </tr> 
     <tr> 
      <td>Last Interesting Moment Type</td> 
     </tr> 
     <tr> 
      <td>Last Marketo Activity by Sales</td> 
     </tr> 
     <tr> 
      <td>Last Marketo Engagement by Sales</td> 
     </tr> 
     <tr> 
      <td>MKTO Lead Score</td> 
     </tr> 
     <tr> 
      <td>Relative Score</td> 
     </tr> 
     <tr> 
      <td>Relative Score Value</td> 
     </tr> 
     <tr> 
      <td>Sales Insight - Opens contact full list page</td> 
     </tr> 
     <tr> 
      <td>Urgency</td> 
     </tr> 
     <tr> 
      <td>Urgency Value</td> 
     </tr> 
    </tbody> 
   </table>

## Map Custom Person Fields {#map-custom-person-fields}

Marketo person fields need to be mapped to Salesforce contact fields to ensure that the conversion works properly. Here's how.

1. Click **Setup**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Search for "fields" in the search bar and click **Fields** under **Leads**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Click **Map Lead Fields**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Click on the dropdown on the right for **Engagement**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Select **Contact.Engagement** in the list.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Repeat and map these fields as well.

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Marketo Person Custom Field</th> 
      <th colspan="1" rowspan="1">Salesforce Contact Custom Field</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Engagement</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Relative Score Value</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Relative Score Value</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Urgency Value</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Urgency Value</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Last Interesting Moment Date</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interesting Moment Date</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Last Interesting Moment Desc</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interesting Moment Desc</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Last Interesting Moment Source</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interesting Moment Source</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Last Interesting Moment Type</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interesting Moment Type</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save** when you’re done.

## Marketo Sales Insight Configuration Tab {#marketo-sales-insight-configuration-tab}

1. In Salesforce, click the **+** at the end of the tab bar and click **Marketo Sales Insight Config**.

1. Select the **Enable Marketo API** checkbox.

1. Copy the credentials from the Soap API panel in [Marketo’s Sales Insight Admin page](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} and paste them into the Soap API section of the Salesforce Sales Insight Configuration page.

1. Copy the credentials from the Rest API panel in [Marketo’s Sales Insight Admin page](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} and paste them into the Rest API section of the Salesforce Sales Insight Configuration page.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

And that’s it! You should be able to see the Marketo Sales Insight fields for Leads, Contacts, Accounts and Opportunities.

>[!NOTE]
>
>If the diagnostics test failed, you might need to [add more fields to your page layout](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>For accounts, Sales Insight will include all emails, but only the most recent interesting moments, web activity, and score changes.

>[!MORELIKETHIS]
>
>* [Priority, Urgency, Relative Score, and Best Bets](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Add Marketo Tab to Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Add Sales Insight Access to Profiles](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
