# Colors Suggested / view_item_list
Fire this whenever the chatbot presents a color suggestion. Items are in an array, so it should just be one event per presentation, with all colors represented.

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
      index: 3,
      item_category: "Orange", //Color Family
      item_list_name: "Chat"
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
