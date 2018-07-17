---
layout: tutorial
group: rest
title: Step 3. Assign a source to stock
menu_title: Step 3. Assign a source to stock
menu_order: 30
level3_subgroup: msi-tutorial
return_to:
  title: REST Tutorials
  url: rest/tutorials/index.html
version: 2.3
github_link: rest/tutorials/msi-order-processing/assign-source-to-stock.md
functional_areas:
  - Integration
---

To assign a source to a stock, you must specify a `source_code`, `stock_id`, and `priority`. The priority value indicates where the stock ranks in the list of stocks that can be used for fulfilling orders.

**Endpoint**

`POST http://<host>/rest/all/V1/inventory/stock-source-links
`
**Headers**

`Content-Type application/json`
`Authorization: Bearer <admin_token>`

**Payload**

```json
{
   "links" : [
      {
         "source_code" : "txspeqs",
         "stock_id" : "2",
         "priority" : 1
      }
   ]
}
```

**Response**
Magento returns empty array.
[]


## Verify this step
