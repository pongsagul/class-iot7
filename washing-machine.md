![Washing Machine](pictures/iot-machine.png)

## Get hardware level operations e.g. wash_count
```
Topic: v1/hw/get/6310301003/model-01/WSH-SN001
Payload: {
    "action"    : "get",
    "project"   : "6310301003",
    "model"     : "model-01",
    "serial"    : "WSH-SN001",
    "name"      : "wash_count",
    "value"     : "114"
}
```

## Get firmware version
```
Topic: v1cdti/hw/get/6310301003/model-01/WSH-SN001
Payload: {
"action" : "get",
"project" : "6310301003",
"model" : "model-01",
"serial" : "SN-001",
"name" : "firmware",
"value" : "v.001"
}
```

## Get manufacture id and geo-location or location placement
```
Topic: v1cdti/hw/get/6310301003/model-01/WSH-SN001
Payload: {
"action" : "get",
"project" : "6310301003",
"model" : "model-01",
"serial" : "SN-001",
"name" : "manufacture",
"value" : "LG"
"lat" : "13.7618"
"long" : "100.5324"
}
```

## Set geo-location or location placement
```
Topic: v1cdti/hw/set/6310301003/model-01/WSH-SN001
Payload: {
    "action" : "set",
    "project" : "6310301003",
    "model" : "model-01",
    "serial" : "SN-001",
    "name" : "location",
    "value" : "Bankok"
}
```

## Monitor machine sensor
```
Topic: v1/hw/Monitor/6310301003/model-01/WSH-SN001
Payload: {
"action" : "Monitor",
"project" : "6310301003",
"model" : "model-01",
"serial" : “SN-001",
"name" : "water_count",
"value" : "200"
}
```

## Set machie status to "maint" to indicate this machine need to be maintenance.
```
Topic: v1/hw/set/6310301003/model-01/WSH-SN001
Payload: {
"action" : "set",
"project" : "6310301003",
"model" : "model-01",
"serial" : "SN-001",
"name" : "status",
"value" : "maint"
}
```