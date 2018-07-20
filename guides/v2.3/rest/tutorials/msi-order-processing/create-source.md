---
layout: tutorial
group: rest
title: Step 1. Create a source
menu_title: Step 1. Create a source
menu_order: 10
level3_subgroup: msi-tutorial
return_to:
  title: REST Tutorials
  url: rest/tutorials/index.html
version: 2.3
github_link: rest/tutorials/msi-order-processing/create-source.md
functional_areas:
  - Integration
---

The `name`, `source_code`, `country_id`, and `postcode` attributes are required.

**Endpoint**

`POST http://<host>/rest/all/V1/inventory/sources`

**Headers**

Content-Type application/json
Authorization: Bearer <admin_token>

**Payload**

``` json
{
   "source" : {
      "description" : " Source #17",
      "source_code" : "txspeqs",
      "phone" : "(555) 555-5555",
      "email" : "sales@company.com",
      "postcode" : "77010",
      "longitude" : -95.383056,
      "enabled" : true,
      "contact_name" : "Ethan Carter",
      "latitude" : 29.762778,
      "region_id" : 57,
      "region" : "Texas",
      "name" : "Texas Sport Equipment Source #017",
      "country_id" : "US",
      "city" : "Houston"
   }
}
```

**Response**
Magento returns an empty array.

`[]`

## Verify this step

In Admin, click **Stores** > **Manage Sources**.  The new source is displayed in the Sources grid. 
