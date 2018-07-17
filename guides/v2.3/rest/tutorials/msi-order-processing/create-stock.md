---
layout: tutorial
group: rest
title: Step 2. Create a stock
menu_title: Step 2. Create a stock
menu_order: 20
level3_subgroup: msi-tutorial
return_to:
  title: REST Tutorials
  url: rest/tutorials/index.html
version: 2.3
github_link: rest/tutorials/msi-order-processing/create-stock.md
functional_areas:
  - Integration
---

The stock.name attribute is required.

**Endpoint**

`POST http://<host>/rest/all/V1/inventory/stocks`

**Headers**

Content-Type: application/json
Authorization: Bearer <admin_token>

**Payload**

``` json
{
   "stock" : {
      "name" : "Stock 2"
   }
}
```

**Response**

Magento returns the stock_id, which is an integer: 2

## Verify this step
