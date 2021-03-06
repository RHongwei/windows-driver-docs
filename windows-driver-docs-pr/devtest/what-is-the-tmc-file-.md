---
title: What is the TMC file
description: What is the TMC file
ms.assetid: 5927d6be-93af-4ab2-bdc1-387fabc9c5ca
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# What is the TMC file?


**Note**  Before Windows Vista, this type of file was generated by default by [Tracepdb](tracepdb.md). Instead, the Tracepdb tool now generates a MOF (.mof) file that describes the provider information in the binary.
Unless you are using [TraceView](traceview.md), ignore references to these TMC files.

 

The [trace message control (.tmc) file](trace-message-control-file.md) is a text file that contains the [control GUID](control-guid.md) along with the trace levels of each [trace provider](trace-provider.md) that is represented in a [PDB symbol file](pdb-symbol-files.md). The name of the TMC file is the control GUID of the trace provider, followed by the .tmc file name extension.

[TraceView](traceview.md) generates a TMC file when it creates a [trace message format (.tmf) file](trace-message-format-file.md) from a PDB symbol file. [Tracepdb](tracepdb.md) can also generate a TMC file when you use the **-c** option.

Most tracing tools do not use the TMC file, but TraceView uses it to associate the control GUID of the trace provider with the [trace flags](trace-flags.md) and [trace level](trace-level.md) that the provider supports.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[devtest\devtest]:%20What%20is%20the%20TMC%20file?%20%20RELEASE:%20%2811/17/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




