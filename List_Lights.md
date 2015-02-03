  Command:
  
  ```js
  {
      "cmd":"light_list"
  }
  ```
  
  Response data:
 ```js
  {
"msync_switch":"<musicSwitch>",
"led":[{"online":"<onlineValue>",
"sn":"<snNUm>",
"title": "<titleValue>", 
"iswitch": "<ledStatus>", 
"r": "<redValue>", 
"g": "<greenValue>",
"b": "blueValue",
"bright": "<lightness>",
"effect": "<model>",
"angle": "<colorAngle>",
"music_sync": "<syncStatus>" 
}
```

msync_switch: switch of music group，default status is on (“msync_switch”:”1”)，stands for allow the leds change the color or lightness with the music \\
Online


## Example
```js
{ 
"msync_switch": "1", 
"led": 
[ { 
"online": "1",
 		"sn": "MD1AC44200001188", 
"title": "iijjjw",
 		"iswitch": "0", 
"r": "0", 
"g": "11", 
"b": "106",
"bright": "89", 
"effect": "9", 
"angle": "233.41176", 
"music_sync": "0"
 	},
{ 
"online": "1", 
"sn": "MD1AC44200001866", 
"title": "lightX", "iswitch": "0", 
"r": "140", 
"g": "30", 
"b": "0", 
"bright": "66",
"effect": "9", 
"angle": "0.0", 
"music_sync": "0"
} 
]}
```
