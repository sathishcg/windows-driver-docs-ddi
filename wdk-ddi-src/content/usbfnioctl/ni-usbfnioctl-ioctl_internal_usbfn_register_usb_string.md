---
UID: NI:usbfnioctl.IOCTL_INTERNAL_USBFN_REGISTER_USB_STRING
title: IOCTL_INTERNAL_USBFN_REGISTER_USB_STRING
author: windows-driver-content
description: The class driver sends this request to register a USB string descriptor.
old-location: buses\ioctl_internal_usbfn_register_usb_string.htm
tech.root: usbref
ms.assetid: 80CB670A-4E64-4E53-815C-12580BE982B5
ms.author: windowsdriverdev
ms.date: 5/7/2018
ms.keywords: IOCTL_INTERNAL_USBFN_REGISTER_USB_STRING, IOCTL_INTERNAL_USBFN_REGISTER_USB_STRING control, IOCTL_INTERNAL_USBFN_REGISTER_USB_STRING control code [Buses], buses.ioctl_internal_usbfn_register_usb_string, usbfnioctl/IOCTL_INTERNAL_USBFN_REGISTER_USB_STRING
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: ioctl
req.header: usbfnioctl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	usbfnioctl.h
api_name:
-	IOCTL_INTERNAL_USBFN_REGISTER_USB_STRING
product:
- Windows
targetos: Windows
req.typenames: 
---

# IOCTL_INTERNAL_USBFN_REGISTER_USB_STRING IOCTL


## -description


The class driver sends this request to register a USB string descriptor.


## -ioctlparameters




### -input-buffer

A pointer to a buffer that contains a  <a href="https://msdn.microsoft.com/library/windows/hardware/mt188007">USBFN_USB_STRING</a> structure with the USB string descriptor. 


### -input-buffer-length

The length of the input buffer must be at least <code>sizeof(USBFN_USB_STRING)</code>.


### -output-buffer

NULL.


### -output-buffer-length

None.


### -in-out-buffer








### -inout-buffer-length








### -status-block

If the request is successful, the USB function class extension (UFX) returns STATUS_SUCCESS, or another status value for which NT_SUCCESS(status) equals TRUE. Otherwise it returns a status value for which NT_SUCCESS(status) equals FALSE. 


## -remarks



This request must be sent after sending the <a href="https://msdn.microsoft.com/library/windows/hardware/mt187891">IOCTL_INTERNAL_USBFN_ACTIVATE_USB_BUS</a> request.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/mt187891">IOCTL_INTERNAL_USBFN_ACTIVATE_USB_BUS</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/mt188007">USBFN_USB_STRING</a>
 

 

