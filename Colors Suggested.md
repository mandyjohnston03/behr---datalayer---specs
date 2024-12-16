# Color Presented / view_item_list
Example: https://www.behr.com/consumer/colors/paint/popular-colors/colors-by-hue/oranges

## Javascript Code
```js
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  event: "view_item_list",
  ecommerce: {
    item_list_name: "Chat",
    items: [
     {
      item_id: "hdc-md-27",
      item_name: "tart orange",
      affiliation: "Google Merchandise Store", //Don't think this is relavent
      coupon: "SUMMER_FUN", //Don't think this is relavent
      discount: 2.22, //Don't think this is relavent
      index: 3,
      item_brand: "Behr Dynasty",
      item_category: "Orange", //Color Family
      item_category2: "", //Interior/Exterior
      item_category3: "", //Finish
      item_category4: "",
      item_category5: "",
      item_list_name: "Chat",
      item_variant: "green", //Don't think this is relavent
      price: 10.03, //Don't think this is relavent
      quantity: 3 //Don't think this is relavent
    }]
  }
});
```


##Dynamic Variable Definitions
| Path     | Definition | Possible Values | Data Type |
|----------|----------|----------|----------|
| ecommerce.item_list_name  | This will always be "Chat" |  | String |
| ecommerce.items.item_id | SKU number | |String |	
| ecommerce.items.item_name | Name of the color | |String |	
| ecommerce.items.index | Position of the color in the list | | Integer |	
| ecommerce.items.item_brand | Specific Behr Brand | | String |	
| ecommerce.items.item_category | Color Family | | String |	
| ecommerce.items.item_category2 | Interior/Exterior | | String |	
| ecommerce.items.item_category3 | Finish | | String |	
