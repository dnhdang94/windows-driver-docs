---
title: Static Driver Verifier Error Codes
description: The following table lists the error codes that Static Driver Verifier could return, and where possible, suggests methods for resolving them.
ms.assetid: AB644106-EB4A-448F-9DA3-D208A38B31F5
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Static Driver Verifier Error Codes


The following table lists the error codes that Static Driver Verifier could return, and where possible, suggests methods for resolving them.

| Code                                         | Description                                                                                                                                                                                                    |
|----------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 0 SDV\_SUCCESS                               | SDV encountered no errors and completed successfully.                                                                                                                                                          |
| 1 SDV\_COMPILER\_ERROR                       | SDV encountered errors when invoking the compiler.                                                                                                                                                             |
| 2 SDV\_ENGINE\_ERROR                         | SDV encountered engine errors during verification.                                                                                                                                                             |
| 3 SDV\_BUILD\_ERROR                          | SDV encountered errors when building the driver.                                                                                                                                                               |
| 4 SDV\_LINK\_ERROR                           | SDV encountered errors when linking the driver.                                                                                                                                                                |
| 5 SDV\_SCAN\_ERROR                           | SDV encountered errors when scanning the driver.                                                                                                                                                               |
| 6 SDV\_UNKNOWN\_ERROR                        | SDV encountered an error of unknown origin.                                                                                                                                                                    |
| 7 SDV\_RULE\_ERROR                           | SDV encountered errors due to rules (for example, the specified \*.slic, \*.h, or \*.fsm file could not be found. )                                                                                            |
| 8 SDV\_MSBUILD\_ERROR                        | SDV encountered an error when invoking MSBUILD.                                                                                                                                                                |
| 9 SDV\_INCOMPLETE\_VERIFICATION              | SDV did not complete the verification and writing to check\_sdv.xml.                                                                                                                                           |
| 10 SDV\_REFINE\_ERROR                        | SDV encountered an error when attempting to do per entry verification using the “/refine” switch.                                                                                                              |
| 11 SDV\_CONFIG\_ERROR                        | SDV encountered an error when processing the config file specified by user.                                                                                                                                    |
| 12 SDV\_MERGE\_ERROR                         | SDV encountered an error when merging results for the driver.                                                                                                                                                  |
| 13 SDV\_CLEAN\_ERROR                         | SDV encountered an error when attempting to clean the SDV folder in the driver sources folder.                                                                                                                 |
| 14 SDV\_CLEANLIBS\_ERROR                     | SDV encountered an error when attempting to clean libraries.                                                                                                                                                   |
| 15 SDV\_UNSUPPORTED\_DRIVER\_TYPE\_ERROR     | SDV does not support the driver due to driver type.                                                                                                                                                            |
| 16 SDV\_REUSE\_ERROR                         | SDV encountered an error when reusing verification data.                                                                                                                                                       |
| 17 SDV\_NO\_ENTRY\_POINTS\_FOUND\_ERROR      | SDV could not discover any entry points in the driver. Make sure that the driver has declared at least one entry point see [Using Function Role Type Declarations](using-function-role-type-declarations.md). |
| 18 SDV\_FINALCOMPILE\_ERROR                  | SDV encountered an error during the final compile stage of SDV.                                                                                                                                                |
| 19 SDV\_UNSUPPORTED\_LOC\_ERROR              | SDV does not support this driver due to driver size.                                                                                                                                                           |
| 20 SDV\_LIBRARY\_VERSION\_ERROR              | SDV could not use the processed library because it was generated using a different version of SDV.                                                                                                             |
| 21 SDV\_RESERVED\_NAME\_ERROR                | SDV could not process the driver/library because a reserved name is used by the driver/library.                                                                                                                |
| 22 SDV\_FILENAME\_ERROR                      | SDV could not process the source files of the driver/library because of the filenames. Spaces and other special characters are not allowed.                                                                    |
| 23 SDV\_UNSUPPORTED\_MODEL\_VERSION\_ERROR   | SDV does not support this version of the driver type, but only the latest versions.                                                                                                                            |
| 24 SDV\_ENVIRONMENT\_ERROR                   | SDV encountered an error trying to detect/set the environment. Please ensure that a complete WDK is installed on the system.                                                                                   |
| 25 SDV\_CORRUPT\_DATA                        | Corrupt SDV data is present in the driver sources folder. Please clean and restart verification.                                                                                                               |
| 26 SDV\_DRIVER\_SOURCES\_ERROR               | SDV encountered an error when loading the driver sources or project file.                                                                                                                                      |
| 27 SDV\_UNSUPPORTED\_ENIRONMENT              | SDV does not support the specified environment.                                                                                                                                                                |
| 28 SDV\_UNSUPPORTED\_LINKER\_SWITCH\_ERROR   | The switches passed to the linker are not supported by the current version of Visual Studio. Static Driver Verifier is supported in Microsoft Visual Studio Ultimate 2012.                                     |
| 29 SDV\_UNSUPPORTED\_CONFIGURATION\_ERROR    | SDV does not support the specified configuration. Please make sure that the selected configuration is a non-debug configuration.                                                                               |
| 30 SDV\_UNSUPPORTED\_PLATFORM\_ERROR         | SDV does not support the specified platform. Please make sure that the selected platform is a Win32, x64, or arm platform.                                                                                     |
| 31SDV\_UNSUPPORTED\_PLATFORM\_TOOLSET\_ERROR | SDV does not support the specified platform toolset.                                                                                                                                                           |
| 32 SDV\_UNSUPPORTED\_SWITCH                  | SDV does not support the given command. Please check and try again. Consult SDV documentation for a list of supported commands.                                                                                |

 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[devtest\devtest]:%20Static%20Driver%20Verifier%20Error%20Codes%20%20RELEASE:%20%2811/17/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




