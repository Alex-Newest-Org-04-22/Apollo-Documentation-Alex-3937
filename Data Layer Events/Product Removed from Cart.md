# Product Removed from Cart

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "remove_from_cart",
  "detailed_event": "Product Removed from Cart",
    "ecommerce": {
        "cart_id": "<cart_id>",
        "currency": "<currency>",
        "items": [
            {
                "affiliation": "<affiliation>",
                "item_id": "<item_id>",
                "item_name": "<item_name>"
            }
        ],
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.cart_id|string|Captures the name or ID of the region within which CTA links are used.|12345, 435678, 34567, XCV456, XCV876|||||||
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.items[n].affiliation|string|A product affiliation to designate a supplying company or brick and mortar store location.|Google Store|||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




