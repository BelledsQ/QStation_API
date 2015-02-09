Command:
```js
{
"cmd":"light_ctrl",
"r":"<redValue>", 
"g":"<greenValue>", 
"b":"<blueValue>", 
"bright":"<brightValue>", 
"effect":"<effectValue>", 
"iswitch":"<ledStatus>", 
"matchValue":"<Value>",
"sn_list":
[
{"sn":"<sn1>"},
{"sn":"<sn2>"}…
]
}
```

- light_ctrl: light control commands
- R: red light value, [0-255]
- G: green light value, [0-255]
- B: blue light value, [0-255]
- Bright: brightness of the light
- Effect: mode of the light: 8 represents white light mode, 9 represents color light mode
- iswitch: state of light (on/off), 1 represents on, 0 represents off
- matchValue: actions of light control, 0 represents light control action, 2 represents match action

No responses. If the light is powered on and under the distance of control, it will work.

## Example
```js
{ 
"g": "255", 
"cmd": "light_ctrl", 
"b": "0", 
"effect": "9", 
"bright": "50", 
"r": "218", 
"sn_list": 
[ { "sn": "MD1AC43300000086"} ], 
"matchValue": "0", 
"iswitch": "1" 
}
```
