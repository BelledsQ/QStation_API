## Add a group
Command:
```js
{
"cmd":" cmdValue",
"group_title":"<newGroupTitle>"
}
```
cmdValue is add_group, then a new group will be added.
Return: 
ok   
fail

### Example
```js
{
"cmd":"add_group",
"group_title":"testGroup"
}
```

## Delete a group
Command:
```js
{
"cmd":"del_group",
"group_id":"<group_id>"
}
```
Return:
ok
fail

### Example
```js
{
"cmd":"del_group",
"group_title":"testGroup"
}
```

## Add a light to a group
Command:
```js
{
"cmd":"set_group",
"sn":"<sn>",
"group_id":"<groupID>"
}
```
Return:
ok
fail

### Example
```js
{
"cmd":"set_group",
"sn":"MD1AC43300000086",
"group_id":"1"
}
```

## Move a light from a group
Command:
```js
{
"cmd":" leave_group ",
"sn":"<sn>",
"group_id":"<groupID>"
}
```
Return
ok
fail

### Example
```js
{
"group_id":"5",
"sn":"MD1AC44200001372",
"cmd":"leave_group"
}
```

## Edit Group Title
Command:
```js
{
"cmd":" set_group_title ",
"sn":"<sn>",
"group_title":"<groupTitle>"
}
```
Return:
ok
fail

### Example
```js
{
"group_id":"7",
"cmd":"set_group_title",
"group_title":"test_group"
}
```

## Group Control
Command:
```js
{
"cmd":"<cmdValue>",
"r":"<redValue>",
"g":"<greenValue>",
"b":"blueValue",
"bright": "<lightValue>",
"effect": "<effectValue>", 
"angle": "colorAngle", 
"sn_list": [ { "sn": "<xxx>" } ], 
"matchValue": "<value>", 
"iswitch": "<ledStatus>", 
"group1": "<group1Value>", 
"angle": "colorValue" 
}
```

### Example
```js
{
"g": "34", 
"model": "6", 
"cmd": "light_ctrl", 
"b": "46", 
"effect": "8", 
"bright": "22", 
"r": "0", 
"sn_list": [ { "sn": "000" } ], 
"matchValue": "0", 
"iswitch": "1", 
"group1": "1", 
"angle": "0.0" 
}
```
