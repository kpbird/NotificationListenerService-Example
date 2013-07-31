NotificationListenerService-Example
===================================

##Introduction
NotificationListenerService is introduced in Android 4.3 (API 18). It allows an application to receive information about notifications as it creates or removes. NotificationListenerService class is derived from the Service class. It has two abstract methods namely 1. onNotificationPosted 2. onNotificationRemoved.  
To use NotificationListenerService, we need to create a java file which extends NotificationListenerService and implement two callback methods. Both methods have a parameter named "sbn", which is an object of StatusBarNotification class. StatusBarNotification provides necessary information about Notifications.
NotificationListenerService provides facility to fetch active notifications using getActiveNotifications and also provides a feature to remove notifications using cancelAllNotifications.

##Useful Methods
1. NotificationListenerService
	* onNotificationPosted
	* onNotificationRemoved
2. StatusBarNotification
	* getId
	* getNotification
	* getPackageName
	* getPostTime
	* isClearable
	* isOngoing

##Note
User require to enable notification permission from "Settings > Security > Notification access".

![Mou icon](http://1.bp.blogspot.com/-7Q9G72-ZLCw/UfirCZP-H_I/AAAAAAAAEOk/aqX_YHs6s6Q/s400/device-2013-07-31-113010.png)
![Mou icon](http://1.bp.blogspot.com/-h_bFIcDWWp8/UfirCzDrC_I/AAAAAAAAEO0/9_aMH5EM6Dg/s400/device-2013-07-31-113539.png)
![Mou icon](http://2.bp.blogspot.com/-thl_wNKzILI/UfirDX6NR2I/AAAAAAAAEO4/_o5FWLmkJ2o/s400/device-2013-07-31-113701.png)
![Mou icon](http://1.bp.blogspot.com/-5KyUJQVOVzE/UfirDhqpFzI/AAAAAAAAEPA/RiZoI9dF--Q/s400/device-2013-07-31-113720.png)