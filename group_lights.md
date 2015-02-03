Command: 
```js
{"cmd":"group_list"}
```

Response: 
```js
{ 
"data": 
[ { 
"effect": "<model>", 
"r": "<redValue>", 
"g": "<greenValue>", 
"b": "blueValue", 
"bright": "<lightness>",
"angle": "<colorAngle>",
"group_title": "<groupLabel>",
"iswitch": "<groupStatus>", 
"group_id": "<groupID>"
}
]}
```

Effect:8 represents white light mode, 9 represents color light mode
R: red light value, [0-255]
G: green light value, [0-255]
B: blue light value, [0-255]
Bright: brightness value
Angle: hue value
Group_title: name of the lights group, editable
lswitch: 1 represents on, 0 represents off
group_id: group number

## Example
{
 "data":
 [ { 
"effect": "9", 
"r": "0", 
"g": "74",
 "b": "225", 
"bright": "106", 
"angle": "220.23529",
 "group_title": "music", 
"iswitch": "1", 
"group_id": "218" 
}, 
{ 
"effect": "8", 
"r": "0", "g": "34", 
"b": "46", "bright": "22", 
"angle": "0.0", 
"group_title": "GSJS", 
"iswitch": "1", 
"group_id": "1" 
} ] 
}

