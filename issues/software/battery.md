Build Number:google/lineage_karnak/karnak:9/PQ3A.190801.002/kai08160902:userdebug/test-keys

screen shot:
![alt text](https://github.com/488315/issuetracker/raw/master/issues/software/screenshot/Screenshot_20190723-231113_Settings.png)
![alt text](https://github.com/488315/issuetracker/raw/master/issues/software/screenshot/Screenshot_20190816-144930_Settings.png)
issue title : USB MTP doesnt work and usb hal

What type of issue is this?
USB HAL


What happens?
when i disconnect from the charger it reports plugged in, not charging after a while the battery screen says discharging

also the USB settings greys out when plugged in and unplugged
Logcat snippet:
```
SystemServiceManager: Starting com.android.server.usb.UsbService$Lifecycle
08-16 13:22:29.470   451   451 I UsbDeviceManager: USB GADGET HAL not present in the device
08-16 13:22:29.470   451   451 I UsbDeviceManager: java.util.NoSuchElementException
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at android.os.HwBinder.getService(Native Method)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at android.hardware.usb.gadget.V1_0.IUsbGadget.getService(IUsbGadget.java:40)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at android.hardware.usb.gadget.V1_0.IUsbGadget.getService(IUsbGadget.java:44)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.usb.UsbDeviceManager.<init>(UsbDeviceManager.java:270)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.usb.UsbService.<init>(UsbService.java:139)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.usb.UsbService$Lifecycle.onStart(UsbService.java:73)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:126)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:113)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.SystemServiceManager.startService(SystemServiceManager.java:72)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.SystemServer.startOtherServices(SystemServer.java:1338)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.SystemServer.run(SystemServer.java:457)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.server.SystemServer.main(SystemServer.java:302)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at java.lang.reflect.Method.invoke(Native Method)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:493)
08-16 13:22:29.470   451   451 I UsbDeviceManager: 	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:838)
08-16 13:22:29.470   451   451 E UsbDeviceManager: Failed to open control for mtp
08-16 13:22:29.471   451   451 E UsbDeviceManager: Failed to open control for ptp
08-16 13:22:29.500   451   512 I UsbPortManager: Usb hal service started android.hardware.usb@1.0::IUsb default

```


software/hardware:
Both


Developers's task:
 * Fix The USB HAL by updating the kernel or providing an 
Testing:
* go to settings>battery
* unplug the charger and you will see the message






