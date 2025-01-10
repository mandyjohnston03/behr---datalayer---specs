# Rating
Fire this whenever a user presses the thumbs up/thumbs down rating


## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "Rating Submitted",
  "rating": "Positive/Negative"
}
});
```


##Dynamic Variable Definitions
| Path     | Definition | Possible Values | Data Type |
|----------|----------|----------|----------|
| rating | If user presses thumbs up, return "Positive". If user presses thumbs down, return "Negative" | Positive/Negative | String |
|  |  | ||

