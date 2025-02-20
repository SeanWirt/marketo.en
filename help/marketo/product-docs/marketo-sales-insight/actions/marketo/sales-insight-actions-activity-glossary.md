---
description: Sales Insight Actions Activity Glossary - Marketo Docs - Product Documentation
title: Sales Insight Actions Activity Glossary
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
---
# Sales Insight Actions Activity Glossary {#sales-insight-actions-activity-glossary}

In Sales Insight Actions, when a seller: adds a lead to a sales campaign, sends them a sales email, or makes an outbound sales call, it will be logged under the Marketo activity history for that lead. Additionally, when the lead engages with emails, opens, clicks, and replies, it also gets logged.

The activities below will be logged to Marketo from Sales Insight Actions.

>[!NOTE]
>
>These activities and attributes are available to be consumed from our REST and Bulk API.

## Activities {#activities}

<table>
 <tr>
  <th>Sales Activity</th>
  <th>Attribute</th>
 </tr>
 <tr>
  <th rowspan="9">Send Sales Email</th>
  <td>Sent By</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Template ID</td>
 </tr>
 <tr>
  <td>Sales Template URL</td>
 </tr>
 <tr>
  <td>Sales Campaign URL</td>
 </tr>
 <tr>
  <td>Sales Template Name</td>
 </tr>
 <tr>
  <td>Email Subject</td>
 </tr>
 <tr>
  <td>Sales Campaign Name</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
 <tr>
  <th rowspan="9">Open Sales Email</th>
  <td>Sent By</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Template ID</td>
 </tr>
 <tr>
  <td>Sales Template URL</td>
 </tr>
 <tr>
  <td>Sales Campaign URL</td>
 </tr>
 <tr>
  <td>Sales Template Name</td>
 </tr>
 <tr>
  <td>Email Subject</td>
 </tr>
 <tr>
  <td>Sales Campaign Name</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
 <tr>
  <th rowspan="10">Clicked Sales Email</th>
  <td>Link</td>
 </tr>
 <tr>
  <td>Sent By</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Template ID</td>
 </tr>
 <tr>
  <td>Sales Template URL</td>
 </tr>
 <tr>
  <td>Sales Campaign URL</td>
 </tr>
 <tr>
  <td>Sales Template Name</td>
 </tr>
 <tr>
  <td>Email Subject</td>
 </tr>
 <tr>
  <td>Sales Campaign Name</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
<tr>
  <th rowspan="3">Replied to Sales Email</th>
  <td>Received By</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
 <tr>
  <th rowspan="11">Received Sales Call</th>
  <td>Sales Call Made By</td>
 </tr>
 <tr>
  <td>Sales Call Status</td>
 </tr>
 <tr>
  <td>Sales Call Subject</td>
 </tr>
 <tr>
  <td>Sales Campaign Name</td>
 </tr>
 <tr>
  <td>Sales Campaign URL</td>
 </tr>
 <tr>
  <td>Sales Phone Number Called</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Sales Call Duration</td>
 </tr>
 <tr>
  <td>Sales Call Recording URL</td>
 </tr>
  <tr>
  <td>Sales Call Answered By</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
 <tr>
  <th rowspan="6">Add to Sales Campaign</th>
  <td>Sales Campaign Name</td>
 </tr>
 <tr>
  <td>Sales Call Status</td>
 </tr>
 <tr>
  <td>Sales Campaign URL</td>
 </tr>
 <tr>
  <td>Sent By</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Sales Campaign ID</td>
 </tr>
 <tr>
  <th rowspan="6">Remove from Sales Campaign</th>
  <td>Sales Campaign Name</td>
 </tr>
 <tr>
  <td>Sales Call Status</td>
 </tr>
 <tr>
  <td>Sales Campaign URL</td>
 </tr>
 <tr>
  <td>Sent By</td>
 </tr>
 <tr>
  <td>Source</td>
 </tr>
 <tr>
  <td>Sales Campaign ID</td>
 </tr>
</table>

## Descriptions {#descriptions}

<table> 
 <tr>
  <th>Attribute</th>
  <th>Description</th>
 </tr>
 <tbody> 
 <tr> 
   <td><strong>Details</strong></td> 
   <td>Bounce error message detail.</td> 
  </tr> 
  <tr> 
   <td><strong>Email</strong></td> 
   <td>Email address that bounced.</td> 
  </tr> 
  <tr> 
   <td><strong>Link</strong></td> 
   <td>URL that was clicked.</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo Sales Person ID</strong></td> 
   <td>Unique ID for person record in Sales Insight Actions.</td> 
  </tr> 
  <tr> 
   <td><strong>Received By</strong></td> 
   <td>Email address of the person who sent the email.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Call Answered By</strong></td> 
   <td>Name of person who answered the call.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Call Duration</strong></td> 
   <td>Length of call in seconds.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Call Made By</strong></td> 
   <td>Email address of sales person who made the call.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Call Recording URL</strong></td> 
   <td>URL of call recording.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Call Status</strong></td> 
   <td>Will save the final call status of the call which includes: completed, no answer, cancelled, failed.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Call Subject</strong></td> 
   <td>Call outcome that's selected by a sales user in the dialer.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Campaign ID</strong></td> 
   <td>Unique ID for Sales Campaign asset in Sales Insight Actions.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Campaign Name</strong></td> 
   <td>Name of Sales Campaign.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Campaign URL</strong></td> 
   <td>Sales Insight Actions URL for Sales Campaign.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Email Subject</strong></td> 
   <td>Subject line of email followed by a unique ID (ex: My Subject Line (SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>Sales Phone Number Called</strong></td> 
   <td>Phone number called by Sales.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Template Name</strong></td> 
   <td>Name of email template in Sales Insight Actions.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Template URL</strong></td> 
   <td>Sales Insight Actions URL for email template.</td> 
  </tr>
  <tr> 
   <td><strong>Sent By</strong></td>
   <td>Email address of the person who sent the email.</td> 
  </tr> 
  <tr> 
   <td><strong>Source</strong></td> 
   <td>Source of the activity. Will be set as "Tout" for Sales Insight Actions activities prior to the Oct '21 Release. Will be "Sales App" for Sales Insight Actions activities after the Oct '21 Release.</td>
  </tr> 
  <tr> 
   <td><strong>Template ID</strong></td> 
   <td>When the source is Tout, the Template ID will be the Marketo Sales Insight Actions Template ID. Use this to target a specific template instead of subject line, which could exist in multiple templates.
</td> 
  </tr> 
 </tbody> 
</table>
