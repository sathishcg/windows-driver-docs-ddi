---
UID: NS:d3d12umddi.D3D12DDI_VIDEO_DECODE_COMPRESSED_BITSTREAM_0032
title: D3D12DDI_VIDEO_DECODE_COMPRESSED_BITSTREAM_0032
author: windows-driver-content
description: Video decode compressed bitstream.
old-location: display\d3d12ddi-video-decode-compressed-bitstream-0032.htm
ms.assetid: 5ef654ff-9a1e-4e97-9087-34ff21e40e1d
ms.author: windowsdriverdev
ms.date: 4/16/2018
ms.keywords: D3D12DDI_VIDEO_DECODE_COMPRESSED_BITSTREAM_0032, D3D12DDI_VIDEO_DECODE_COMPRESSED_BITSTREAM_0032 structure [Display Devices], d3d12umddi/D3D12DDI_VIDEO_DECODE_COMPRESSED_BITSTREAM_0032, display.d3d12ddi-video-decode-compressed-bitstream-0032
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: d3d12umddi.h
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
-	d3d12umddi.h
api_name:
-	D3D12DDI_VIDEO_DECODE_COMPRESSED_BITSTREAM_0032
product:
- Windows
targetos: Windows
tech.root: display
req.typenames: D3D12DDI_VIDEO_DECODE_COMPRESSED_BITSTREAM_0032
---

# D3D12DDI_VIDEO_DECODE_COMPRESSED_BITSTREAM_0032 structure


## -description


Contains the compressed bitstream to decode from.


## -struct-fields




### -field hDrvBuffer

The source buffer that contains the compressed bitstream to decode.


### -field Offset

The offset to the beginning of the first slice. This offset has alignment requirements based on the tier value.


### -field Size

The buffer size.

