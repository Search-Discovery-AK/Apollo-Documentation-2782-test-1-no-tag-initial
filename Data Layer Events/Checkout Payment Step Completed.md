# Checkout Payment Step Completed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "add_payment_info",
  "apollo_event": "Checkout Payment Step Completed",
    "count_checkout_payment_step_completions": "<count_checkout_payment_step_completions>",
    "ecommerce": {
        "currency": "<currency>",
        "items": [
            {
                "item_id": "<item_id>",
                "item_name": "<item_name>"
            }
        ],
        "payment_type": "<payment_type>",
        "value": "<value>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|count_checkout_payment_step_completions|number|Captures the specific chat service line used. \(i.e., the agent\)||||||||
|currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\) |SKU\_12345|||||||
|item_name|string|Item Name \(context-specific\).|jeggings|||||||
|payment_type|string|The chosen method of payment.|credit card, gift card, paypal, apple pay|||||||
|value|number|The monetary value of the event.	|7.77, 239.55, 659|||||||




