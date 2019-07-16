# Clarion-H5-Cleaner
Cleans folders left behind when there is no clean exit from the Clarion H5 Appbroker

* Requires Clarion 10 or later


This utility is designed to be run after hours by the Windows Task Sceduler with an Administrator login.
Use with discretion and at your own risk.

The Clarion Appbroker does not remove the temporary folders created for each instance if the users do not exit "cleanly" from
your app. This utility allows you to schedule a regular cleanup. The assets folder is not affected by this.

There are two entries in the H5CLEANER.INI file - change the entries to suit your installation

The PublicPath is the public folder used by the application broker.

The Restart option allows you to force the Clarion Application Broker service to restart. 
Any apps still running will be terminated.

[H5Actions]
PublicPath=c:\AppBroker\public 
Restart=Y
