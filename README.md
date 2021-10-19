# TcLibraryVersions

The TwinCAT remote manager facilitates developing in a production environment where multiple version of TwinCAT are used simultaniously. This is achieved by switching the TwinCAT version directly in the the integrated-development-environment (IDE, e.g. TwinCAT XAE).
However, when installing TwinCAT with a specific version it comes with a large number of libraries in a specific version. With multiple version of TwinCAT installed, there is no real way to tell, which TwinCAT Version comes with what library version.

In a supportable production-environment this information is crucial for maintaining stability. When a harddrive crashes it is desirable to go back to the exact version of all libraries that were used in the PLC with a CI system. Some times it may make no real difference, but in a production-environment the PLCs of some machines may be pretty old and upgrading them to a new library version may introduce undesirable sideeffects, e.g. some bugs in a new library version could have been fixed. As allows in development ["somebody's bug, may be somebody's feature"](https://xkcd.com/1172/) and thus, it is not always beneficial to update to a new version.

Since Beckhoff officially provide any information about the "TwinCAT version" - "library version" relationship, this repository is used to provide this information to developers.

# TwinCAT versions and the library versions it ships with







|TcVersion|Tc2_BA|Tc2_BABasic|Tc2_BACnetRev12|Tc2_CncBase|Tc2_CncHli|Tc2_CncPlcopenP1|Tc2_CncPlcopenP4|Tc2_ControllerToolbox|Tc2_Coupler|Tc2_DALI|Tc2_Database|Tc2_DataExchange|Tc2_DMX|Tc2_Drive|Tc2_EIB|Tc2_EnOcean|Tc2_EtherCAT|Tc2_EthernetIP|Tc2_FTP|Tc2_GENIbus|Tc2_HVAC|Tc2_IoFunctions|Tc2_KL85xx|Tc2_LON|Tc2_Math|Tc2_MBus|Tc2_MC2|Tc2_MC2_Camming|Tc2_MC2_Drive|Tc2_MC2_FlyingSaw|Tc2_MC2_XFC|Tc2_MDP|Tc2_ModbusRTU|Tc2_ModbusSrv|Tc2_MPBus|Tc2_NC|Tc2_NcDrive|Tc2_NcFifoAxes|Tc2_NCI|Tc2_NciXFC|Tc2_PlcInterpolation|Tc2_ProfinetDiag|Tc2_RFID|Tc2_S5S7Com|Tc2_SerialCom|Tc2_SMI|Tc2_SMS|Tc2_Smtp|Tc2_SPA|Tc2_Standard|Tc2_SUPS|Tc2_System|Tc2_SystemC69xx|Tc2_SystemCX|Tc2_TcpIp|Tc2_TempController|Tc2_Utilities|Tc2_XmlDataSrv|Tc3_BA|Tc3_BA2_Common|Tc3_BACnetRev14|Tc3_BA_Common|Tc3_DALI|Tc3_Database|Tc3_DriveMotionControl|Tc3_DynamicMemory|Tc3_EtherCATExtSync|Tc3_EventLogger|Tc3_Interfaces|Tc3_IotBase|Tc3_IotCommunicator|Tc3_IotFunctions|Tc3_IPCDiag|Tc3_JsonXml|Tc3_LS|Tc3_MC2_AdvancedHoming|Tc3_MC2_AdvancedHoming_XFC|Tc3_Module|Tc3_mxAutomation|Tc3_mxAutomationV3_0|Tc3_mxAutomationV3_1|Tc3_PackML|Tc3_PackML_V2|Tc3_PLCopen_OpcUa|Tc3_RealtimeMonitoring|Tc3_uniValPlc|Tc3_uniValPlc_v4|Tc3_uniValPlc_v4_3|Tc3_uniValPlc_v4_4|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|4024.12|3.3.9.0|3.1.2.0|2.5.18.1|3.3.3031.10|3.3.3031.41|3.3.3031.11|3.3.3031.10|3.4.3.0|3.3.1.0|3.6.18.0|3.3.20.2|3.3.5.0|3.5.5.0|3.3.5.0|3.3.10.0|3.4.6.0|3.3.15.0|1.0.2.0|3.3.5.2|3.3.1.0|3.3.8.0|3.3.13.0|3.4.6.0|3.3.4.0|3.3.1.0|3.4.8.0|3.3.42.0|3.3.11.0|3.3.22.0|3.3.1.0|3.3.17.0|3.3.7.0|3.4.2.0|3.3.2.0|3.4.12.0|3.3.1.0|3.3.3.0|3.3.2.0|3.3.12.0|3.3.5.0|3.3.16.0|1.2.3.0|3.3.7.0|3.3.1.0|3.3.7.0|3.3.8.0|3.3.1.0|3.3.2.0|3.3.2.0|3.3.3.0|3.3.8.0|3.4.24.0|3.3.1.0|3.3.6.0|3.3.6.0|3.3.4.0|3.3.41.0|3.3.1.0|1.1.5.0|2.1.3.23|4.0.22.12|2.1.4.0|3.5.0.0|3.4.0.15|3.0.3.0|1.0.2.0|3.3.1.0|3.1.24.0|3.4.3.0|3.1.18.0|1.0.7.0|3.3.1.0|1.0.5.0|3.3.14.0|1.1.5.0|3.0.13.0|3.0.4.0|3.3.21.0|2.1.3.3|3.0.4.0|3.1.0.0|3.3.3.0|3.3.14.0|3.2.9.0|1.0.2.0|3.1.0.2|4.1.1.3|4.3.0.1|4.4.1.0|
|4024.11|3.3.9.0|3.1.2.0|2.5.18.1|3.3.3031.10|3.3.3031.41|3.3.3031.11|3.3.3031.10|3.4.3.0|3.3.1.0|3.6.18.0|3.3.20.2|3.3.5.0|3.5.5.0|3.3.5.0|3.3.10.0|3.4.6.0|3.3.15.0|1.0.2.0|3.3.5.2|3.3.1.0|3.3.8.0|3.3.13.0|3.4.6.0|3.3.4.0|3.3.1.0|3.4.8.0|3.3.42.0|3.3.11.0|3.3.22.0|3.3.1.0|3.3.17.0|3.3.7.0|3.4.2.0|3.3.2.0|3.4.12.0|3.3.1.0|3.3.3.0|3.3.2.0|3.3.12.0|3.3.5.0|3.3.16.0|1.2.3.0|3.3.7.0|3.3.1.0|3.3.7.0|3.3.8.0|3.3.1.0|3.3.2.0|3.3.2.0|3.3.3.0|3.3.8.0|3.4.24.0|3.3.1.0|3.3.6.0|3.3.6.0|3.3.4.0|3.3.41.0|3.3.1.0|1.1.5.0|2.1.3.23|4.0.22.12|2.1.4.0|3.5.0.0|3.4.0.15|3.0.3.0|1.0.2.0|3.3.1.0|3.1.24.0|3.4.3.0|3.1.18.0|1.0.7.0|3.3.1.0|1.0.5.0|3.3.14.0|1.1.5.0|3.0.13.0|3.0.4.0|3.3.21.0|2.1.3.3|3.0.4.0|3.1.0.0|3.3.3.0|3.3.14.0|3.2.9.0|1.0.2.0|3.1.0.2|4.1.1.3|4.3.0.1|4.4.1.0|
|4024.10|3.3.9.0|3.1.2.0|2.5.18.1|3.3.3031.10|3.3.3031.41|3.3.3031.11|3.3.3031.10|3.4.3.0|3.3.1.0|3.6.18.0|3.3.20.2|3.3.5.0|3.5.5.0|3.3.5.0|3.3.10.0|3.4.6.0|3.3.15.0|1.0.2.0|3.3.5.2|3.3.1.0|3.3.8.0|3.3.13.0|3.4.6.0|3.3.4.0|3.3.1.0|3.4.8.0|3.3.42.0|3.3.11.0|3.3.22.0|3.3.1.0|3.3.17.0|3.3.7.0|3.4.2.0|3.3.2.0|3.4.12.0|3.3.1.0|3.3.3.0|3.3.2.0|3.3.12.0|3.3.5.0|3.3.16.0|1.2.3.0|3.3.7.0|3.3.1.0|3.3.7.0|3.3.8.0|3.3.1.0|3.3.2.0|3.3.2.0|3.3.3.0|3.3.8.0|3.4.24.0|3.3.1.0|3.3.6.0|3.3.6.0|3.3.4.0|3.3.41.0|3.3.1.0|1.1.5.0|2.1.3.23|4.0.22.12|2.1.4.0|3.5.0.0|3.4.0.15|3.0.3.0|1.0.2.0|3.3.1.0|3.1.24.0|3.4.3.0|3.1.18.0|1.0.7.0|3.3.1.0|1.0.5.0|3.3.14.0|1.1.5.0|3.0.13.0|3.0.4.0|3.3.21.0|2.1.3.3|3.0.4.0|3.1.0.0|3.3.3.0|3.3.14.0|3.2.9.0|1.0.2.0|3.1.0.2|4.1.1.3|4.3.0.1|4.4.1.0|
