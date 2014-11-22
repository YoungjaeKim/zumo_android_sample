zumo_android_sample
===================

This project is an working example of Azure Mobile Service Push Notification for Android GCM. The Azure documentation does not provide enough information, so I upload simplified working source code.

Modify following lines in **MainActivity.java**.

1.line 50. Change below number to GCM project number (not project ID nickname).
```java
public static final String SENDER_ID = "0000000000"; // YOUR_GOOGLE_GCM_PROJECT_NUMBER
```
 
2.line 60. Download android file from Azure Mobile Service dashboard and replace below `***placeholder***` values.
```java
			mClient = new MobileServiceClient(
					"https://***YOUR_ZUMO_DOMAIN***.azure-mobile.net/",
					"***REPLACE_FROM_YOUR_ZUMO_TEMPLATE***",
					this).withFilter(new ProgressFilter());
```

##Reference
 - [Azure Mobile Service for GCM](http://azure.microsoft.com/en-us/documentation/articles/mobile-services-dotnet-backend-android-get-started-push/)
