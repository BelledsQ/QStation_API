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

- msync_switch: switch of music group，default status is on (“msync_switch”:”1”)，stands for allow the leds change the color or lightness with the music
- Online: led is online or offline，1stands for online，0 stands for offline，2 stands for the led was matched but has deleted 
- Sn:	the number of a led
- Title：led label，can be renamed by user,length:0-128
- Iswitch：the status of led，1 stands for on，0 stands for off
- R: color led red value, [0-255]
- G: color led green value, [0-255]
- B: color led blue value, [0-255]
- Bright: brightness, [0-255]
- Effect: mode of lights: 8 represents white light, 9 is color lights
- Angle: hue value
- music_sync: 1 represents that lights do not sync with music, 0 represents that lights sync with music

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
