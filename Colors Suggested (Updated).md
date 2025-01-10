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
      item_id: "color_only",
      item_name: "color_only",
      index: 1,
      item_category3: "tart orange", // Color Name
      item_category4: “hdc-md-27”, // Color ID
      item_category5: “Visualizer”, //Context of display
      item_variant: “Orange”, // Color Family 
      item_list_name: "Chat"
    }]
  }
});
```


##Dynamic Variable Definitions
| Path     | Definition | Possible Values | Data Type |
|----------|----------|----------|----------|
| ecommerce.item_list_name  | This will always be "Chat" |  | String |
| ecommerce.items.item_id | Placeholder - "color" - they currently define this aligned to the brand name | |String |	
| ecommerce.items.item_name | Placeholder - "color" - they currently define this is the size of the paint being purchased | |String |	
| ecommerce.items.index | Position of the color in the list | | Integer |	
| ecommerce.items.item_category3 | Name of the color | | String |	
| ecommerce.items.item_category4 | Color ID | | String |	
| ecommerce.items.item_category5 | Context of display - "Visualizer", "One Chip View", "Three Chip View" | | String |	
| ecommerce.items.item_variant | Color Family | | String |	
