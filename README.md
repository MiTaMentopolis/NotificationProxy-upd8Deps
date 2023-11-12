# NotificationProxy - NP

### Location
The NotificationProxy is part of the HighPerformanceNetworkInterface.

### Description
The NotificationProxy allows subscribing for DeviceNotifications and ControllerNotifications according to the ONF TR-532 definitions.  

It encapsulates all necessary formats and communication required for that. This includes:  
- It opens the necessary permanent HTTP connections for receiving notifications of all controllers.  
- It opens the necessary permanent HTTP connections for receiving notifications of all mounted devices.  
- Wherever required, it is translating notification formats (e.g. ODL=>ONF or IETF=>ONF).  
- It translates the event stream based method for forwarding notifications applied by OpenDaylight to the webhook based method applied in the MW SDN application layer.  
- It removes duplicates potentially caused by the controller architecture.  

### Relevance
The NotificationProxy significantly reduces the implementation efforts of every application that requires receiving notifications.
This includes not just Closed-Loop-Automation applications, but also very fundamental Inventories.

### Resources
- [Specification](./spec/)
- [TestSuite](./testing/)
- [Implementation](./server/)

### Comments
./.