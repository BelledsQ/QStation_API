Command:
```js
{
“cmd”:” group_leds_list”,
”group_id”:”<groupID>”
}
```
Response:
```js
{ 
"data": 
[ {
 "sn": "<sn1>", 
"status": "groupStatus"
}, 
{ 
"sn": "<sn2>", 
"status": "groupStatus" 
} ] 
}
```

- Status: 0 represents that the light is not assigned to any group, 1 represents the light is assigned to this group, 2 represents the light is assigned to the other group

## Example
```js
{ 
"data": 
[ { 
"sn": "MD1AC43300000086", 
"status": "1" 
}, 
{ 
"sn": "MD1AC43300000085", 
"status": "2" 
} ] 
}
```
