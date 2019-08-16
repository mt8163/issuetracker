Build Number:google/lineage_karnak/karnak:9/PQ3A.190801.002/kai08160902:userdebug/test-keys

issue title : Video codecs doesnt work [wip]

What type of issue is this?
video codecs


What happens?
when i start playing video this spams out the logcat and w

Logcat snippet:
```
08-16 13:22:30.211   318   318 D MtkOmxMp3Dec: JB MtkOmxMp3Dec::MtkOmxMp3Dec this= 0xf3bf3000
08-16 13:22:30.212   318   318 D MtkOmxMp3Dec: JB MtkOmxMp3Dec::InitAudioParams(MP3)
08-16 13:22:30.213   318   318 D MtkOmxMp3Dec: JB ~MtkOmxMp3Dec this= 0xf3bf3000
08-16 14:05:56.582  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.592  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.616  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.630  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.649  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.662  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.680  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.680  2142  2270 W OmxInfoBuilder: Fail to add mime audio/gsm to codec OMX.MTK.AUDIO.DECODER.GSM after software codecs
08-16 14:05:56.686  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.687  2142  2270 W OmxInfoBuilder: Fail to add mime audio/mpeg-L2 to codec OMX.MTK.AUDIO.DECODER.MP2 after software codecs
08-16 14:05:56.692  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.707  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.710   318   356 D MtkOmxMp3Dec: JB MtkOmxMp3Dec::MtkOmxMp3Dec this= 0xf3bf3000
08-16 14:05:56.710   318   356 D MtkOmxMp3Dec: JB MtkOmxMp3Dec::InitAudioParams(MP3)
08-16 14:05:56.716   318   355 D MtkOmxMp3Dec: JB ~MtkOmxMp3Dec this= 0xf3bf3000
08-16 14:05:56.719  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.738  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.750  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.759  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.766  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.770  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.785  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:56.790  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:57.272  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:57.761  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:57.772  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:58.143  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:58.155  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:58.485  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:58.784  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:58.792  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:59.076  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:59.357  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:59.364  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:59.629  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:59.635  2142  2270 I OMXClient: IOmx service obtained
08-16 14:05:59.908  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.179  2142  2270 W OmxInfoBuilder: Fail to add mime video/x-vnd.on2.vp9 to codec OMX.MTK.VIDEO.DECODER.VP9.secure
08-16 14:06:00.184  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.225  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.312   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 10, color format = 21
08-16 14:06:00.312   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetConfig (0x6F60000A)
08-16 14:06:00.313   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetState (mState=OMX_StateLoaded)
08-16 14:06:00.313   318   356 D MtkOmxCore: Mtk_OMX_FreeHandle
08-16 14:06:00.313   318   356 D MtkOmxVenc: [0xf3bf3000] +MtkOmxVenc::ComponentDeInit
08-16 14:06:00.313   318  2720 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread terminated pVenc=0xF3BF3000
08-16 14:06:00.313   318  2721 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread terminated pVenc=0xF3BF3000
08-16 14:06:00.313   318  2719 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread terminated
08-16 14:06:00.313   318   356 D MtkOmxVenc: [0xf3bf3000] -MtkOmxVenc::ComponentDeInit
08-16 14:06:00.313   318   356 D MtkOmxVenc: [0xf3bf3000] ~MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.313   318   356 D MtkOmxMVAMgr: [0xf3bbb540] remove ion MVA Map, count 0
08-16 14:06:00.313   318   356 D MtkOmxMVAMgr: [0xf3bbb520] remove ion MVA Map, count 0
08-16 14:06:00.313   318   356 D MtkOmxMVAMgr: [0xf3bbb380] remove ion MVA Map, count 0
08-16 14:06:00.313   318  2722 D MtkOmxCore: ## MtkOmxCoreCpuControlThread terminated
08-16 14:06:00.313   318   356 D MtkOmxCore: free_inst_handle dlclose(0x0x494d5225), free(0x0xf3bf3004)
08-16 14:06:00.325  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.345  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.346   318   356 D MtkOmxCore: Mtk_OMX_GetHandle (OMX.MTK.VIDEO.ENCODER.H263)
08-16 14:06:00.346   318   356 D MtkOmxCore: comp_index(23), path(libMtkOmxVenc.so) max_instance(20)
08-16 14:06:00.384   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.384   318   356 D MtkOmxMVAMgr: [0xf3bbb380] Create ion MVA Map!
08-16 14:06:00.384   318   356 D MtkOmxMVAMgr: [0xf3bbb520] Create ion MVA Map!
08-16 14:06:00.384   318   356 D MtkOmxMVAMgr: [0xf3bbb540] Create ion MVA Map!
08-16 14:06:00.384   318   356 D MtkOmxVenc: [0xf3bf3000] dump flag=0x0
08-16 14:06:00.384   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxComponentCreate mCompHandle(0xF3BF3004)
08-16 14:06:00.384   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::ComponentInit (OMX.MTK.VIDEO.ENCODER.H263)
08-16 14:06:00.385   318   356 D MtkOmxCore: MtkOmxCoreCpuControlThread created (0xF1B4D970)
08-16 14:06:00.385   318   356 D MtkOmxCore: +++++ dump_inst_handle_pool +++++
08-16 14:06:00.385   318   356 D MtkOmxCore: gCoreCompInstance[0].comp_module=0x0x8d3f0d2d, comp_handle=0x0x0, comp_name=(null)
08-16 14:06:00.385   318   356 D MtkOmxCore: gCoreCompInstance[1].comp_module=0x0xdde29c17, comp_handle=0x0x0, comp_name=(null)
08-16 14:06:00.385   318   356 D MtkOmxCore: gCoreCompInstance[2].comp_module=0x0x6bde96ef, comp_handle=0x0xf3bf3004, comp_name=OMX.MTK.VIDEO.ENCODER.H263
08-16 14:06:00.385   318   356 D MtkOmxCore: ----- dump_inst_handle_pool -----
08-16 14:06:00.385   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::SetCallbacks
08-16 14:06:00.386   318  2739 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread created pVenc=0xF3BF3000
08-16 14:06:00.386   318  2741 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread created pVenc=0xF3BF3000, tid=2741
08-16 14:06:00.387   318  2740 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread created pVenc=0xF3BF3000, tid=2740
08-16 14:06:00.387   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::SetParameter index(0x01000017)
08-16 14:06:00.388   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.388   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.388   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.388   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.389   318   356 E MtkOmxVenc: [0xf3bf3000] [ERROR] Unsupported H263 Level
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 0, color format = 2130706944
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.389   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.389   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.389   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 1, color format = 2130708361
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.390   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.390   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 2, color format = 2130706944
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.390   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.390   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 3, color format = 19
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.390   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.390   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 4, color format = 6
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.390   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.390   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.390   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.391   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.391   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 5, color format = 11
08-16 14:06:00.391   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.391   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.392   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.392   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.392   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.392   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 6, color format = 16
08-16 14:06:00.392   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.392   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.392   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.392   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 7, color format = 2130707200
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.393   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.393   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 8, color format = 15
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.393   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.393   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 9, color format = 15
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetConfig (0x6F60000A)
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetState (mState=OMX_StateLoaded)
08-16 14:06:00.393   318   356 D MtkOmxCore: Mtk_OMX_FreeHandle
08-16 14:06:00.393   318   356 D MtkOmxVenc: [0xf3bf3000] +MtkOmxVenc::ComponentDeInit
08-16 14:06:00.394   318  2740 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread terminated pVenc=0xF3BF3000
08-16 14:06:00.394   318  2741 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread terminated pVenc=0xF3BF3000
08-16 14:06:00.394   318  2739 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread terminated
08-16 14:06:00.394   318   356 D MtkOmxVenc: [0xf3bf3000] -MtkOmxVenc::ComponentDeInit
08-16 14:06:00.394   318   356 D MtkOmxVenc: [0xf3bf3000] ~MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.394   318   356 D MtkOmxMVAMgr: [0xf3bbb540] remove ion MVA Map, count 0
08-16 14:06:00.394   318   356 D MtkOmxMVAMgr: [0xf3bbb520] remove ion MVA Map, count 0
08-16 14:06:00.394   318   356 D MtkOmxMVAMgr: [0xf3bbb380] remove ion MVA Map, count 0
08-16 14:06:00.394   318  2742 D MtkOmxCore: ## MtkOmxCoreCpuControlThread terminated
08-16 14:06:00.394   318   356 D MtkOmxCore: free_inst_handle dlclose(0x0x6bde96ef), free(0x0xf3bf3004)
08-16 14:06:00.407  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.418  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.420   318   356 D MtkOmxCore: Mtk_OMX_GetHandle (OMX.MTK.VIDEO.ENCODER.HEVC)
08-16 14:06:00.420   318   356 D MtkOmxCore: comp_index(25), path(libMtkOmxVenc.so) max_instance(20)
08-16 14:06:00.449   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.449   318   356 D MtkOmxMVAMgr: [0xf3bbb380] Create ion MVA Map!
08-16 14:06:00.450   318   356 D MtkOmxMVAMgr: [0xf3bbb520] Create ion MVA Map!
08-16 14:06:00.450   318   356 D MtkOmxMVAMgr: [0xf3bbb540] Create ion MVA Map!
08-16 14:06:00.450   318   356 D MtkOmxVenc: [0xf3bf3000] dump flag=0x0
08-16 14:06:00.450   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxComponentCreate mCompHandle(0xF3BF3004)
08-16 14:06:00.450   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::ComponentInit (OMX.MTK.VIDEO.ENCODER.HEVC)
08-16 14:06:00.450   318   356 E MtkOmxVenc: [0xf3bf3000] bufk = 0
08-16 14:06:00.450   318  2747 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread created pVenc=0xF3BF3000
08-16 14:06:00.450   318  2749 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread created pVenc=0xF3BF3000, tid=2749
08-16 14:06:00.450   318   356 D MtkOmxCore: MtkOmxCoreCpuControlThread created (0xF1B54970)
08-16 14:06:00.450   318   356 D MtkOmxCore: +++++ dump_inst_handle_pool +++++
08-16 14:06:00.450   318   356 D MtkOmxCore: gCoreCompInstance[0].comp_module=0x0x8d3f0d2d, comp_handle=0x0x0, comp_name=(null)
08-16 14:06:00.450   318   356 D MtkOmxCore: gCoreCompInstance[1].comp_module=0x0xdde29c17, comp_handle=0x0x0, comp_name=(null)
08-16 14:06:00.450   318   356 D MtkOmxCore: gCoreCompInstance[2].comp_module=0x0x25e2cab5, comp_handle=0x0xf3bf3004, comp_name=OMX.MTK.VIDEO.ENCODER.HEVC
08-16 14:06:00.450   318   356 D MtkOmxCore: ----- dump_inst_handle_pool -----
08-16 14:06:00.450   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::SetCallbacks
08-16 14:06:00.450   318  2748 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread created pVenc=0xF3BF3000, tid=2748
08-16 14:06:00.450   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::SetParameter index(0x01000017)
08-16 14:06:00.451   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.453   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.453   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.453   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.453   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.454   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.454   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.454   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 0, color format = 2130706944
08-16 14:06:00.454   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.454   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.456   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.456   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.456   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.456   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 1, color format = 2130708361
08-16 14:06:00.456   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.456   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.456   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.456   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 2, color format = 2130706944
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.457   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.457   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 3, color format = 19
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.457   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.457   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 4, color format = 6
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.457   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.457   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 5, color format = 11
08-16 14:06:00.457   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.457   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.458   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.458   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.458   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.458   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 6, color format = 16
08-16 14:06:00.458   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.458   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.458   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.458   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.458   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.458   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 7, color format = 2130707200
08-16 14:06:00.458   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.458   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.459   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.459   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.460   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.460   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 8, color format = 15
08-16 14:06:00.460   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.460   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.460   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.460   318   356 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.460   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.460   318   356 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 9, color format = 15
08-16 14:06:00.460   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetConfig (0x6F60000A)
08-16 14:06:00.461   318   356 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetState (mState=OMX_StateLoaded)
08-16 14:06:00.461   318   356 D MtkOmxCore: Mtk_OMX_FreeHandle
08-16 14:06:00.461   318   356 D MtkOmxVenc: [0xf3bf3000] +MtkOmxVenc::ComponentDeInit
08-16 14:06:00.461   318  2749 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread terminated pVenc=0xF3BF3000
08-16 14:06:00.461   318  2748 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread terminated pVenc=0xF3BF3000
08-16 14:06:00.462   318  2747 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread terminated
08-16 14:06:00.462   318   356 D MtkOmxVenc: [0xf3bf3000] -MtkOmxVenc::ComponentDeInit
08-16 14:06:00.462   318   356 D MtkOmxVenc: [0xf3bf3000] ~MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.462   318   356 D MtkOmxMVAMgr: [0xf3bbb540] remove ion MVA Map, count 0
08-16 14:06:00.462   318   356 D MtkOmxMVAMgr: [0xf3bbb520] remove ion MVA Map, count 0
08-16 14:06:00.462   318   356 D MtkOmxMVAMgr: [0xf3bbb380] remove ion MVA Map, count 0
08-16 14:06:00.462   318  2750 D MtkOmxCore: ## MtkOmxCoreCpuControlThread terminated
08-16 14:06:00.462   318   356 D MtkOmxCore: free_inst_handle dlclose(0x0x25e2cab5), free(0x0xf3bf3004)
08-16 14:06:00.470  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.470   318   355 D MtkOmxCore: Mtk_OMX_GetHandle (OMX.MTK.VIDEO.ENCODER.MPEG4)
08-16 14:06:00.470   318   355 D MtkOmxCore: comp_index(24), path(libMtkOmxVenc.so) max_instance(20)
08-16 14:06:00.494   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.494   318   355 D MtkOmxMVAMgr: [0xf3bbb380] Create ion MVA Map!
08-16 14:06:00.494   318   355 D MtkOmxMVAMgr: [0xf3bbb520] Create ion MVA Map!
08-16 14:06:00.494   318   355 D MtkOmxMVAMgr: [0xf3bbb540] Create ion MVA Map!
08-16 14:06:00.494   318   355 D MtkOmxVenc: [0xf3bf3000] dump flag=0x0
08-16 14:06:00.494   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxComponentCreate mCompHandle(0xF3BF3004)
08-16 14:06:00.494   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::ComponentInit (OMX.MTK.VIDEO.ENCODER.MPEG4)
08-16 14:06:00.495   318   355 D MtkOmxCore: MtkOmxCoreCpuControlThread created (0xF1B5C970)
08-16 14:06:00.495   318   355 D MtkOmxCore: +++++ dump_inst_handle_pool +++++
08-16 14:06:00.495   318   355 D MtkOmxCore: gCoreCompInstance[0].comp_module=0x0x8d3f0d2d, comp_handle=0x0x0, comp_name=(null)
08-16 14:06:00.495   318   355 D MtkOmxCore: gCoreCompInstance[1].comp_module=0x0xdde29c17, comp_handle=0x0x0, comp_name=(null)
08-16 14:06:00.495   318   355 D MtkOmxCore: gCoreCompInstance[2].comp_module=0x0xdb42721d, comp_handle=0x0xf3bf3004, comp_name=OMX.MTK.VIDEO.ENCODER.MPEG4
08-16 14:06:00.495   318   355 D MtkOmxCore: ----- dump_inst_handle_pool -----
08-16 14:06:00.495   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::SetCallbacks
08-16 14:06:00.499   318  2753 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread created pVenc=0xF3BF3000, tid=2753
08-16 14:06:00.501   318  2754 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread created pVenc=0xF3BF3000, tid=2754
08-16 14:06:00.501   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::SetParameter index(0x01000017)
08-16 14:06:00.502   318  2752 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread created pVenc=0xF3BF3000
08-16 14:06:00.503   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.503   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.503   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.504   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.504   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.506   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.508   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.509   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.509   318   355 E MtkOmxVenc: [0xf3bf3000] QueryVideoProfileLevel(1) fail, profile(16384)/level(16)
08-16 14:06:00.509   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.509   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 0, color format = 2130706944
08-16 14:06:00.514   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.514   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.516   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.516   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.516   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.516   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 1, color format = 2130708361
08-16 14:06:00.517   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.517   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.520   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.520   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.521   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.521   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 2, color format = 2130706944
08-16 14:06:00.521   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.521   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.522   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.522   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.522   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.522   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 3, color format = 19
08-16 14:06:00.522   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.522   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.522   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.522   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 4, color format = 6
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.523   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.523   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 5, color format = 11
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.523   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.523   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.523   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 6, color format = 16
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.524   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.524   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 7, color format = 2130707200
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.524   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.524   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 8, color format = 15
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.524   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.524   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.524   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.525   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.525   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 9, color format = 15
08-16 14:06:00.525   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetConfig (0x6F60000A)
08-16 14:06:00.525   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetState (mState=OMX_StateLoaded)
08-16 14:06:00.525   318   355 D MtkOmxCore: Mtk_OMX_FreeHandle
08-16 14:06:00.525   318   355 D MtkOmxVenc: [0xf3bf3000] +MtkOmxVenc::ComponentDeInit
08-16 14:06:00.525   318  2753 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread terminated pVenc=0xF3BF3000
08-16 14:06:00.525   318  2752 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread terminated
08-16 14:06:00.525   318  2754 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread terminated pVenc=0xF3BF3000
08-16 14:06:00.525   318   355 D MtkOmxVenc: [0xf3bf3000] -MtkOmxVenc::ComponentDeInit
08-16 14:06:00.525   318   355 D MtkOmxVenc: [0xf3bf3000] ~MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.525   318   355 D MtkOmxMVAMgr: [0xf3bbb540] remove ion MVA Map, count 0
08-16 14:06:00.525   318   355 D MtkOmxMVAMgr: [0xf3bbb520] remove ion MVA Map, count 0
08-16 14:06:00.525   318   355 D MtkOmxMVAMgr: [0xf3bbb380] remove ion MVA Map, count 0
08-16 14:06:00.526   318  2755 D MtkOmxCore: ## MtkOmxCoreCpuControlThread terminated
08-16 14:06:00.526   318   355 D MtkOmxCore: free_inst_handle dlclose(0x0xdb42721d), free(0x0xf3bf3004)
08-16 14:06:00.531  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.545  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.545   318   355 D MtkOmxCore: Mtk_OMX_GetHandle (OMX.MTK.VIDEO.ENCODER.VPX)
08-16 14:06:00.545   318   355 D MtkOmxCore: comp_index(26), path(libMtkOmxVenc.so) max_instance(20)
08-16 14:06:00.568   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.568   318   355 D MtkOmxMVAMgr: [0xf3bbb380] Create ion MVA Map!
08-16 14:06:00.568   318   355 D MtkOmxMVAMgr: [0xf3bbb520] Create ion MVA Map!
08-16 14:06:00.568   318   355 D MtkOmxMVAMgr: [0xf3bbb540] Create ion MVA Map!
08-16 14:06:00.568   318   355 D MtkOmxVenc: [0xf3bf3000] dump flag=0x0
08-16 14:06:00.568   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxComponentCreate mCompHandle(0xF3BF3004)
08-16 14:06:00.568   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::ComponentInit (OMX.MTK.VIDEO.ENCODER.VPX)
08-16 14:06:00.568   318   355 E MtkOmxVenc: [0xf3bf3000] bufk = 0
08-16 14:06:00.569   318   355 D MtkOmxCore: MtkOmxCoreCpuControlThread created (0xF1B71970)
08-16 14:06:00.569   318   355 D MtkOmxCore: +++++ dump_inst_handle_pool +++++
08-16 14:06:00.569   318   355 D MtkOmxCore: gCoreCompInstance[0].comp_module=0x0x8d3f0d2d, comp_handle=0x0x0, comp_name=(null)
08-16 14:06:00.569   318   355 D MtkOmxCore: gCoreCompInstance[1].comp_module=0x0xdde29c17, comp_handle=0x0x0, comp_name=(null)
08-16 14:06:00.569   318   355 D MtkOmxCore: gCoreCompInstance[2].comp_module=0x0xe9dedb03, comp_handle=0x0xf3bf3004, comp_name=OMX.MTK.VIDEO.ENCODER.VPX
08-16 14:06:00.569   318   355 D MtkOmxCore: ----- dump_inst_handle_pool -----
08-16 14:06:00.569   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::SetCallbacks
08-16 14:06:00.570   318  2761 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread created pVenc=0xF3BF3000, tid=2761
08-16 14:06:00.570   318  2760 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread created pVenc=0xF3BF3000, tid=2760
08-16 14:06:00.571   318  2759 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread created pVenc=0xF3BF3000
08-16 14:06:00.572   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::SetParameter index(0x01000017)
08-16 14:06:00.573   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.574   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.575   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x0600000F)
08-16 14:06:00.575   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.575   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 0, color format = 2130706944
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.576   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.576   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 1, color format = 2130708361
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.576   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.576   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 2, color format = 2130706944
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.576   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.576   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.576   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.577   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.577   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 3, color format = 19
08-16 14:06:00.577   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.577   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.578   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.578   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.578   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.578   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 4, color format = 6
08-16 14:06:00.578   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.578   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.578   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.578   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 5, color format = 11
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.579   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.579   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 6, color format = 16
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.579   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.579   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 7, color format = 2130707200
08-16 14:06:00.579   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.580   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.580   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 8, color format = 15
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.580   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex
08-16 14:06:00.580   318   355 E MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetExtensionIndex Unknown parameter name: OMX.google.android.index.describeColorFormat2
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetParameter (0x06000001)
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] [GetParameter] OMX_IndexParamVideoPortFormat index = 9, color format = 15
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetConfig (0x6F60000A)
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] MtkOmxVenc::GetState (mState=OMX_StateLoaded)
08-16 14:06:00.580   318   355 D MtkOmxCore: Mtk_OMX_FreeHandle
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] +MtkOmxVenc::ComponentDeInit
08-16 14:06:00.580   318  2760 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencEncodeThread terminated pVenc=0xF3BF3000
08-16 14:06:00.580   318  2761 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencConvertThread terminated pVenc=0xF3BF3000
08-16 14:06:00.580   318  2759 D MtkOmxVenc: [0xf3bf3000] MtkOmxVencThread terminated
08-16 14:06:00.580   318   355 D MtkOmxVenc: [0xf3bf3000] -MtkOmxVenc::ComponentDeInit
08-16 14:06:00.581   318   355 D MtkOmxVenc: [0xf3bf3000] ~MtkOmxVenc this= 0xF3BF3000
08-16 14:06:00.581   318   355 D MtkOmxMVAMgr: [0xf3bbb540] remove ion MVA Map, count 0
08-16 14:06:00.581   318   355 D MtkOmxMVAMgr: [0xf3bbb520] remove ion MVA Map, count 0
08-16 14:06:00.581   318   355 D MtkOmxMVAMgr: [0xf3bbb380] remove ion MVA Map, count 0
08-16 14:06:00.581   318  2762 D MtkOmxCore: ## MtkOmxCoreCpuControlThread terminated
08-16 14:06:00.581   318   355 D MtkOmxCore: free_inst_handle dlclose(0x0xe9dedb03), free(0x0xf3bf3004)
08-16 14:06:00.592  2142  2270 I OMXClient: IOmx service obtained
08-16 14:06:00.627  2369  2504 I OMXClient: IOmx service obtained
08-16 14:06:00.782  2369  2778 I OMXClient: IOmx service obtained
08-16 14:06:00.885  2369  2787 I OMXClient: IOmx service obtained
08-16 14:12:05.420  3366  3384 I OMXClient: IOmx service obtained
```


software/hardware:
Software


Developers's task:
 * Fix up Codecs
 * Try to fix the media_profiles.xml and media_codecs.xml
 * try to fix frameworks/av and frameworks/native to try to make the camera to work.
Testing:
* go to settings>general>gestures>gestures and the video doesnt play and crashes surfaceflinger






