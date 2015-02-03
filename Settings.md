## Set Light Name
Command: 
```js
{
"cmd":"set_title",
"sn":"<sn>",
"title":"<title>"
}
```
No return value.

### Example
```js
{
"title":"test",
"sn":"MD1AC43300000080",
"cmd":"set_title"
}
```

## Save Lights 
Command:
```js
{
"cmd":"light_ctrl_save",
"r":"<redValue>",
 "g":"<greenValue>", 
"b":"<blueValue>", 
"bright":"<brightValue>", 
"effect":"<effectValue>", 
"iswitch":"<ledStatus>", 
"matchValue":"<Value>",
"angle":"<colorAngle>",
"sn_list":[{"sn":"<sn1>"
},
{"sn":"<sn2>"}…]
}
```
No Return.

### Example
```js
{
"g":30,
"cmd":"light_ctrl_save",
"b":0,
"effect":9,
"bright":"66",
"r":140,
"sn_list":
[{
"sn":"MD1AC44200001866"
}],
"matchValue":"0",
"iswitch":"1",
"angle":"0.0"
}
```
## Music Setting
Command:
```js
{
“cmd”:” set_musicled”,
”sn”:”<music_led_sn>”
}
```
Then the light with this sn number will sync with music.
No return value. 

### Example
```js
{"cmd":"set_musicled","sn":"MD1AC43300000080"}
```

## Music Group Setting
Command:
```js
{
“cmd”:”set_music_group”,
”music_group”:”<music_led_group>”
}
```
Then all the lights in this group will sync with music. 
No return value.

### Example
```js
{
"cmd":"set_music_group",
"music_group":"218"
}
```

## Delete a light
Command:
```js
{
"cmd":" del_device",
"sn":"<sn>"
}
```

