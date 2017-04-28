# SmartLab API

Our partner in Lisbon provided us with an API description for the first part of the project.
In the file [DevicesAPI.html](DevicesAPI.html) you will find a description of the
REST API to read the status of power hubs and light bulbs.

You should also have a look at the general [WSO2 Device Management API](https://docs.wso2.com/display/IoTS300/swagger/?url=https://docs.wso2.com/display/IoTS300/swagger/apis/device-mgt.json#!/Device_Management/getDevices).  
You should look at the sections `DeviceManagement` and `DeviceGroupManagement`.

Be aware of the following things:
* Each power socket has its own unique identifier
* There will be a *device group* for each power hub
* There will be other *devices groups*, so you need to filter
* Each device has several *sensortypes* that you need to specify
* the data only contains changes of a certain delta (electricity: +/- 15%, temperature: +/- 0.125 C)
* asking for the state will give you all changes in a given period - to get the latest state, you need to find the last change.

The API is not live yet.  
When it goes live, you will be assigned authentication tokens that you will have to use.

If you are uncertain about something -> Ask!
