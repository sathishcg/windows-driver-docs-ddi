---
UID: NS:mpiowmi._GetPathConfiguration_OUT
title: "_GetPathConfiguration_OUT"
author: windows-driver-content
description: The GetPathConfiguration_OUT structure is used to report the output parameters that are associated with the GetPathConfiguration method.
old-location: storage\getpathconfiguration_out.htm
tech.root: storage
ms.assetid: 055db46e-59fc-4eb9-93d7-16d680495220
ms.author: windowsdriverdev
ms.date: 3/29/2018
ms.keywords: "*PGetPathConfiguration_OUT, GetPathConfiguration_OUT, GetPathConfiguration_OUT structure [Storage Devices], PGetPathConfiguration_OUT, PGetPathConfiguration_OUT structure pointer [Storage Devices], _GetPathConfiguration_OUT, mpiowmi/GetPathConfiguration_OUT, mpiowmi/PGetPathConfiguration_OUT, storage.getpathconfiguration_out, structs-scsibus_4d2ebbae-67ff-42bc-8904-c33f914485cd.xml"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: mpiowmi.h
req.include-header: Mpiowmi.h
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
-	mpiowmi.h
api_name:
-	GetPathConfiguration_OUT
product:
- Windows
targetos: Windows
req.typenames: GetPathConfiguration_OUT, *PGetPathConfiguration_OUT
---

# _GetPathConfiguration_OUT structure


## -description


The GetPathConfiguration_OUT structure is used to report the output parameters that are associated with the GetPathConfiguration method.


## -struct-fields




### -field EntryCount

A 32-bitfield that indicates the number of entries contained in the array of SCSI addresses.


### -field Address

An array that returns information about the SCSI addresses. The number of elements in the array is given by EntryCount and each element of the array represents an instance of an SCSI_ADDR structure.

