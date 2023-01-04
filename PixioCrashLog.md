# PICXIO crash log

---

## `Translated Report (Full Report Below)`

`Incident Identifier: 3D0E8E2C-BE27-4BF1-9305-849139E63B9B`

`CrashReporter Key:   b61e142826e16bb63a98a6aac5262af9c6bb9ea8`

`Hardware Model:      iPhone11,8`

`Process:             Pixio [64385]`

`Path:                /private/var/containers/Bundle/Application/D7BCF619-928F-427F-8FE5-45F23D8B8B25/Pixio.app/Pixio`

`Identifier:          site.pixio.pixio`

`Version:             3.0.1 (55)`

`AppStoreTools:       13F100`

`AppVariant:          1:iPhone11,8:15`

`Code Type:           ARM-64 (Native)`

`Role:                Background`

`Parent Process:      launchd [1]`

`Coalition:           site.pixio.pixio [4029]`

`Date/Time:           2022-11-07 08:47:13.6399 +0200`

`Launch Time:         2022-11-07 08:42:17.5421 +0200`

`OS Version:          iPhone OS 16.1 (20B82)`

`Release Type:        User`

`Baseband Version:    5.01.01`

`Report Version:      104`

`Exception Type:  EXC_CRASH (SIGKILL)`

`Exception Codes: 0x0000000000000000, 0x0000000000000000`

`Termination Reason: FRONTBOARD 2343432205`

`<RBSTerminateContext| domain:10 code:0x8BADF00D explanation:scene-update watchdog transgression: application<site.pixio.pixio>:64385 exhausted real (wall clock) time allowance of 10.00 seconds`

`ProcessVisibility: Background`

`ProcessState: Running`

`WatchdogEvent: scene-update`

`WatchdogVisibility: Background`

`WatchdogCPUStatistics: (`

`"Elapsed total CPU time (seconds): 20.190 (user 20.190, system 0.000), 34% CPU",`

`"Elapsed application CPU time (seconds): 0.286, 0% CPU"`

`) reportType:CrashLog maxTerminationResistance:Interactive>`

`Triggered by Thread:  0`

`Kernel Triage:`

`VM - pmap_enter retried due to resource shortage`

`VM - pmap_enter retried due to resource shortage`

`VM - pmap_enter retried due to resource shortage`

`VM - pmap_enter retried due to resource shortage`

`VM - pmap_enter retried due to resource shortage`

`Thread 0 name:   Dispatch queue: com.apple.main-thread`

`Thread 0 Crashed:`

`0   libsystem_kernel.dylib                   0x202ed241c __psynch_cvwait + 8`

`1   libsystem_pthread.dylib                  0x21333b06c _pthread_cond_wait + 1232`

`2   QuartzCore                               0x1c7a1d7bc -[CADisplayLink invalidate] + 92`

`3   SceneKit                                 0x211835da0 -[SCNDisplayLink invalidate] + 64`

`4   SceneKit                                 0x211865c18 -[SCNView dealloc] + 116`

`5   Pixio                                    0x102a470cc 0x1027dc000 + 2535628`

`6   SwiftUI                                  0x1c9cd6adc 0x1c9c6b000 + 441052`

`7   libswiftCore.dylib                       0x1c04f8558 (anonymous namespace)destroyGenericBox(swiftHeapObject*) + 152`

`8   libswiftCore.dylib                       0x1c04f7134 _swift_release_dealloc + 56`

`9   SwiftUI                                  0x1caaf278c 0x1c9c6b000 + 15234956`

`10  libswiftCore.dylib                       0x1c04f7134 _swift_release_dealloc + 56`

`11  libswiftCore.dylib                       0x1c04e8294 swift_arrayDestroy + 124`

`12  libswiftCore.dylib                       0x1c01bf474 _ContiguousArrayStorage.__deallocating_deinit + 96`

`13  libswiftCore.dylib                       0x1c04f7134 _swift_release_dealloc + 56`

`14  libswiftCore.dylib                       0x1c04e8294 swift_arrayDestroy + 124`

`15  libswiftCore.dylib                       0x1c01bf474 _ContiguousArrayStorage.__deallocating_deinit + 96`

`16  libswiftCore.dylib                       0x1c04f7134 _swift_release_dealloc + 56`

`17  SwiftUI                                  0x1cac55088 0x1c9c6b000 + 16687240`

`18  SwiftUI                                  0x1cadb05bc 0x1c9c6b000 + 18109884`

`19  SwiftUI                                  0x1ca41cf34 0x1c9c6b000 + 8068916`

`20  SwiftUI                                  0x1ca41f788 0x1c9c6b000 + 8079240`

`21  SwiftUI                                  0x1c9d37ef8 0x1c9c6b000 + 839416`

`22  SwiftUI                                  0x1c9e82fa0 0x1c9c6b000 + 2195360`

`23  UIKitCore                                0x1c84be564 +[UIView(Animation) performWithoutAnimation:] + 76`

`24  SwiftUI                                  0x1c9ccce54 0x1c9c6b000 + 400980`

`25  SwiftUI                                  0x1c9c88acc 0x1c9c6b000 + 121548`

`26  SwiftUI                                  0x1c9d2bbf0 0x1c9c6b000 + 789488`

`27  SwiftUI                                  0x1c9c79b8c 0x1c9c6b000 + 60300`

`28  SwiftUI                                  0x1c9c77790 0x1c9c6b000 + 51088`

`29  SwiftUI                                  0x1c9c78da4 0x1c9c6b000 + 56740`

`30  QuartzCore                               0x1c7986f9c CADisplayDisplayLink::dispatch_items(unsigned long long, unsigned long long, unsigned long long) + 756`

`31  QuartzCore                               0x1c79988a4 display_timer_callback(__CFMachPort*, void*, long, void*) + 372`

`32  CoreFoundation                           0x1c634b820 __CFMachPortPerform + 176`

`33  CoreFoundation                           0x1c6368d00 CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE1_PERFORM_FUNCTION + 60`

`34  CoreFoundation                           0x1c636a908 __CFRunLoopDoSource1 + 520`

`35  CoreFoundation                           0x1c634c13c __CFRunLoopRun + 2264`

`36  CoreFoundation                           0x1c6350ed4 CFRunLoopRunSpecific + 612`

`37  GraphicsServices                         0x1ff652368 GSEventRunModal + 164`

`38  UIKitCore                                0x1c882f3d0 -[UIApplication _run] + 888`

`39  UIKitCore                                0x1c882f034 UIApplicationMain + 340`

`40  libswiftUIKit.dylib                      0x1cee1f308 UIApplicationMain(::::) + 104`

`41  Pixio                                    0x1027e7370 0x1027dc000 + 45936`

`42  dyld                                     0x1e49b8960 start + 2528`

`Thread 1 name:  com.apple.uikit.eventfetch-thread`

`Thread 1:`

`0   libsystem_kernel.dylib                   0x202ed1b48 mach_msg2_trap + 8`

`1   libsystem_kernel.dylib                   0x202ee4008 mach_msg2_internal + 80`

`2   libsystem_kernel.dylib                   0x202ee4248 mach_msg_overwrite + 388`

`3   libsystem_kernel.dylib                   0x202ed208c mach_msg + 24`

`4   CoreFoundation                           0x1c634aaf0 __CFRunLoopServiceMachPort + 160`

`5   CoreFoundation                           0x1c634bd34 __CFRunLoopRun + 1232`

`6   CoreFoundation                           0x1c6350ed4 CFRunLoopRunSpecific + 612`

`7   Foundation                               0x1c06fa334 -[NSRunLoop(NSRunLoop) runMode:beforeDate:] + 212`

`8   Foundation                               0x1c06fa21c -[NSRunLoop(NSRunLoop) runUntilDate:] + 64`

`9   UIKitCore                                0x1c896433c -[UIEventFetcher threadMain] + 436`

`10  Foundation                               0x1c0713808 NSThread__start + 716`

`11  libsystem_pthread.dylib                  0x2133346cc _pthread_start + 148`

`12  libsystem_pthread.dylib                  0x213333ba4 thread_start + 8`

`Thread 2 name:  com.google.firebase.crashlytics.MachExceptionServer`

`Thread 2:`

`0   libsystem_kernel.dylib                   0x202ed1b48 mach_msg2_trap + 8`

`1   libsystem_kernel.dylib                   0x202ee4008 mach_msg2_internal + 80`

`2   libsystem_kernel.dylib                   0x202ee4248 mach_msg_overwrite + 388`

`3   libsystem_kernel.dylib                   0x202ed208c mach_msg + 24`

`4   Pixio                                    0x10395247c 0x1027dc000 + 18310268`

`5   libsystem_pthread.dylib                  0x2133346cc _pthread_start + 148`

`6   libsystem_pthread.dylib                  0x213333ba4 thread_start + 8`

`Thread 3 name:  com.apple.NSURLConnectionLoader`

`Thread 3:`

`0   libsystem_kernel.dylib                   0x202ed1b48 mach_msg2_trap + 8`

`1   libsystem_kernel.dylib                   0x202ee4008 mach_msg2_internal + 80`

`2   libsystem_kernel.dylib                   0x202ee4248 mach_msg_overwrite + 388`

`3   libsystem_kernel.dylib                   0x202ed208c mach_msg + 24`

`4   CoreFoundation                           0x1c634aaf0 __CFRunLoopServiceMachPort + 160`

`5   CoreFoundation                           0x1c634bd34 __CFRunLoopRun + 1232`

`6   CoreFoundation                           0x1c6350ed4 CFRunLoopRunSpecific + 612`

`7   CFNetwork                                0x1c76a85a8 0x1c7452000 + 2450856`

`8   Foundation                               0x1c0713808 NSThread__start + 716`

`9   libsystem_pthread.dylib                  0x2133346cc _pthread_start + 148`

`10  libsystem_pthread.dylib                  0x213333ba4 thread_start + 8`

---

`Thread 4 name:   Dispatch queue: com.apple.root.user-initiated-qos`

`Thread 4:`

`0   libsystem_kernel.dylib                   0x202ed1b48 mach_msg2_trap + 8`

`1   libsystem_kernel.dylib                   0x202ee4008 mach_msg2_internal + 80`

`2   libsystem_kernel.dylib                   0x202ee4248 mach_msg_overwrite + 388`

`3   libsystem_kernel.dylib                   0x202ed208c mach_msg + 24`

`4   CoreFoundation                           0x1c634aaf0 __CFRunLoopServiceMachPort + 160`

`5   CoreFoundation                           0x1c634bd34 __CFRunLoopRun + 1232`

`6   CoreFoundation                           0x1c6350ed4 CFRunLoopRunSpecific + 612`

`7   Foundation                               0x1c06fa334 -[NSRunLoop(NSRunLoop) runMode:beforeDate:] + 212`

`8   Foundation                               0x1c06fa1c8 -[NSRunLoop(NSRunLoop) run] + 64`

`9   Pixio                                    0x10304fdb0 0x1027dc000 + 8863152`

`10  Pixio                                    0x10295334c 0x1027dc000 + 1536844`

`11  libdispatch.dylib                        0x1cd8a84b4 _dispatch_call_block_and_release + 32`

`12  libdispatch.dylib                        0x1cd8a9fdc _dispatch_client_callout + 20`

`13  libdispatch.dylib                        0x1cd8bbb8c _dispatch_root_queue_drain + 684`

`14  libdispatch.dylib                        0x1cd8bc284 _dispatch_worker_thread2 + 164`

`15  libsystem_pthread.dylib                  0x213333dbc _pthread_wqthread + 228`

`16  libsystem_pthread.dylib                  0x213333b98 start_wqthread + 8`

---

`Thread 5 name:  com.apple.CoreMotion.MotionThread`

`Thread 5:`

`0   libsystem_kernel.dylib                   0x202ed1b48 mach_msg2_trap + 8`

`1   libsystem_kernel.dylib                   0x202ee4008 mach_msg2_internal + 80`

`2   libsystem_kernel.dylib                   0x202ee4248 mach_msg_overwrite + 388`

`3   libsystem_kernel.dylib                   0x202ed208c mach_msg + 24`

`4   CoreFoundation                           0x1c634aaf0 __CFRunLoopServiceMachPort + 160`

`5   CoreFoundation                           0x1c634bd34 __CFRunLoopRun + 1232`

`6   CoreFoundation                           0x1c6350ed4 CFRunLoopRunSpecific + 612`

`7   CoreFoundation                           0x1c6394d04 CFRunLoopRun + 64`

`8   CoreMotion                               0x1d1874ec0 0x1d1861000 + 81600`

`9   libsystem_pthread.dylib                  0x2133346cc _pthread_start + 148`

`10  libsystem_pthread.dylib                  0x213333ba4 thread_start + 8`

`Thread 6:`

`0   libsystem_pthread.dylib                  0x213333b90 start_wqthread + 0`

`Thread 7:`

`0   libsystem_pthread.dylib                  0x213333b90 start_wqthread + 0`

`Thread 8 name:  com.apple.SwiftUI.AsyncRenderer`

`Thread 8:`

`0   libsystem_kernel.dylib                   0x202ed2b48 __psynch_mutexwait + 8`

`1   libsystem_pthread.dylib                  0x213335150 _pthread_mutex_firstfit_lock_wait + 84`

`2   libsystem_pthread.dylib                  0x21333c310 _pthread_mutex_firstfit_lock_slow + 248`

`3   SwiftUI                                  0x1c9c7cdb4 _MovableLockLock + 48`

`4   SwiftUI                                  0x1c9d15038 0x1c9c6b000 + 696376`

`5   SwiftUI                                  0x1c9d13168 0x1c9c6b000 + 688488`

`6   Foundation                               0x1c0713808 NSThread__start + 716`

`7   libsystem_pthread.dylib                  0x2133346cc _pthread_start + 148`

`8   libsystem_pthread.dylib                  0x213333ba4 thread_start + 8`

`Thread 9:`

`0   libsystem_pthread.dylib                  0x213333b90 start_wqthread + 0`

`Thread 10:`

`0   libsystem_pthread.dylib                  0x213333b90 start_wqthread + 0`

`Thread 11:`

`0   libsystem_pthread.dylib                  0x213333b90 start_wqthread + 0`

`Thread 12 name:  com.apple.scenekit.scnview-renderer`

`Thread 12:`

`0   libsystem_kernel.dylib                   0x202ed1b48 mach_msg2_trap + 8`

`1   libsystem_kernel.dylib                   0x202ee4008 mach_msg2_internal + 80`

`2   libsystem_kernel.dylib                   0x202ee4248 mach_msg_overwrite + 388`

`3   libsystem_kernel.dylib                   0x202ed208c mach_msg + 24`

`4   CoreFoundation                           0x1c634aaf0 __CFRunLoopServiceMachPort + 160`

`5   CoreFoundation                           0x1c634bd34 __CFRunLoopRun + 1232`

`6   CoreFoundation                           0x1c6350ed4 CFRunLoopRunSpecific + 612`

`7   Foundation                               0x1c06fa334 -[NSRunLoop(NSRunLoop) runMode:beforeDate:] + 212`

`8   SceneKit                                 0x21174d474 __85-[SCNView(SCNDisplayLink) _initializeDisplayLinkWithScreen:policy:completionHandler:]_block_invoke + 460`

`9   SceneKit                                 0x21174d57c SCNRenderThread_start + 80`

`10  libsystem_pthread.dylib                  0x2133346cc _pthread_start + 148`

`11  libsystem_pthread.dylib                  0x213333ba4 thread_start + 8`

`Thread 13 name:  com.apple.scenekit.scnview-renderer`

`Thread 13:`

`0   libsystem_kernel.dylib                   0x202ed2b48 __psynch_mutexwait + 8`

`1   libsystem_pthread.dylib                  0x21333bc94 _pthread_mutex_fairshare_lock_wait + 84`

`2   libsystem_pthread.dylib                  0x21333bbec _pthread_mutex_fairshare_lock_slow + 196`

`3   SceneKit                                 0x211835bec -[SCNDisplayLink _displayLinkCallbackWaitingOnFrameCompletionWithTime:] + 48`

`4   QuartzCore                               0x1c7986f9c CADisplayDisplayLink::dispatch_items(unsigned long long, unsigned long long, unsigned long long) + 756`

`5   QuartzCore                               0x1c79988a4 display_timer_callback(__CFMachPort*, void*, long, void*) + 372`

`6   CoreFoundation                           0x1c634b820 __CFMachPortPerform + 176`

`7   CoreFoundation                           0x1c6368d00 CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE1_PERFORM_FUNCTION + 60`

`8   CoreFoundation                           0x1c636a908 __CFRunLoopDoSource1 + 520`

`9   CoreFoundation                           0x1c634c13c __CFRunLoopRun + 2264`

`10  CoreFoundation                           0x1c6350ed4 CFRunLoopRunSpecific + 612`

`11  Foundation                               0x1c06fa334 -[NSRunLoop(NSRunLoop) runMode:beforeDate:] + 212`

`12  SceneKit                                 0x21174d474 __85-[SCNView(SCNDisplayLink) _initializeDisplayLinkWithScreen:policy:completionHandler:]_block_invoke + 460`

`13  SceneKit                                 0x21174d57c SCNRenderThread_start + 80`

`14  libsystem_pthread.dylib                  0x2133346cc _pthread_start + 148`

`15  libsystem_pthread.dylib                  0x213333ba4 thread_start + 8`

`Thread 14 name:  com.apple.scenekit.scnview-renderer`

`Thread 14:`

`0   libsystem_kernel.dylib                   0x202ed1b48 mach_msg2_trap + 8`

`1   libsystem_kernel.dylib                   0x202ee4008 mach_msg2_internal + 80`

`2   libsystem_kernel.dylib                   0x202ee4248 mach_msg_overwrite + 388`

`3   libsystem_kernel.dylib                   0x202ed208c mach_msg + 24`

`4   CoreFoundation                           0x1c634aaf0 __CFRunLoopServiceMachPort + 160`

`5   CoreFoundation                           0x1c634bd34 __CFRunLoopRun + 1232`

`6   CoreFoundation                           0x1c6350ed4 CFRunLoopRunSpecific + 612`

`7   Foundation                               0x1c06fa334 -[NSRunLoop(NSRunLoop) runMode:beforeDate:] + 212`

`8   SceneKit                                 0x21174d474 __85-[SCNView(SCNDisplayLink) _initializeDisplayLinkWithScreen:policy:completionHandler:]_block_invoke + 460`

`9   SceneKit                                 0x21174d57c SCNRenderThread_start + 80`

`10  libsystem_pthread.dylib                  0x2133346cc _pthread_start + 148`

`11  libsystem_pthread.dylib                  0x213333ba4 thread_start + 8`

`Thread 0 crashed with ARM Thread State (64-bit): x0: 0x0000000000000104   x1: 0x0000000000000000   x2: 0x0000000000000000   x3: 0x0000000000000000
x4: 0x0000000000000000   x5: 0x00000000000000a0   x6: 0x0000000000000000   x7: 0x0000000000000000
x8: 0x000000016d620b48   x9: 0x0000000000000000  x10: 0x0000000135e88750  x11: 0x0000000000000002`

`x12: 0x0000000000000000  x13: 0x0000000000000000  x14: 0x0000000000000000  x15: 0x0000000000000000`

`x16: 0x0000000000000131  x17: 0x00000002219d2a98  x18: 0x0000000000000000  x19: 0x0000000135e88738`

`x20: 0x0000000135e88778  x21: 0x000000021c9459e0  x22: 0x0000000000000000  x23: 0x0000000000000000`

`x24: 0x0000000000000000  x25: 0x0000000000000001  x26: 0x0000000000000100  x27: 0x00000001c04f9050`

`x28: 0x000000021d28da20   fp: 0x000000016d620bc0   lr: 0x000000021333b06c
sp: 0x000000016d620b30   pc: 0x0000000202ed241c cpsr: 0x60000000`

`far: 0xffffffe01cca7054  esr: 0x56000080  Address size fault`

`Binary Images: 0x202ed1000 - 0x202f07ffb libsystem_kernel.dylib arm64e /usr/lib/system/libsystem_kernel.dylib 0x213333000 - 0x21333efff libsystem_pthread.dylib arm64e <1aa3a4b6f9e730568c8b4e4dd81312a4> /usr/lib/system/libsystem_pthread.dylib 0x1c795e000 - 0x1c7cbafff QuartzCore arm64e <046338bf09cf3414bc9331296b97eb2d> /System/Library/Frameworks/QuartzCore.framework/QuartzCore 0x211621000 - 0x211b05fff SceneKit arm64e <5d296524c7b43c39b5f772333e51f852> /System/Library/Frameworks/SceneKit.framework/SceneKit 0x1027dc000 - 0x10409ffff Pixio arm64 /private/var/containers/Bundle/Application/D7BCF619-928F-427F-8FE5-45F23D8B8B25/Pixio.app/Pixio 0x1c9c6b000 - 0x1cb5aefff SwiftUI arm64e <494a7d5790af3e9096237038275b8d87> /System/Library/Frameworks/SwiftUI.framework/SwiftUI 0x1c011d000 - 0x1c0685fff libswiftCore.dylib arm64e /usr/lib/swift/libswiftCore.dylib 0x1c848d000 - 0x1c9c6afff UIKitCore arm64e <179501b60fc2344ab969b4e3961ebe10> /System/Library/PrivateFrameworks/UIKitCore.framework/UIKitCore 0x1c62d0000 - 0x1c66b5fff CoreFoundation arm64e <5cdc5d9ae5063740b64ebb30867b4f1b> /System/Library/Frameworks/CoreFoundation.framework/CoreFoundation 0x1ff651000 - 0x1ff659fff GraphicsServices arm64e /System/Library/PrivateFrameworks/GraphicsServices.framework/GraphicsServices 0x1cedea000 - 0x1cee5efff libswiftUIKit.dylib arm64e <6383e8e8672633918d95bb5ee497e9aa> /usr/lib/swift/libswiftUIKit.dylib 0x1e49a3000 - 0x1e4a2600f dyld arm64e /usr/lib/dyld 0x1c06b8000 - 0x1c1001fff Foundation arm64e /System/Library/Frameworks/Foundation.framework/Foundation 0x1c7452000 - 0x1c7819fff CFNetwork arm64e /System/Library/Frameworks/CFNetwork.framework/CFNetwork 0x1cd8a6000 - 0x1cd8ecfff libdispatch.dylib arm64e /usr/lib/system/libdispatch.dylib 0x1d1861000 - 0x1d1c4dfff CoreMotion arm64e <958c1c714f383d53a2b65f0182d618e1> /System/Library/Frameworks/CoreMotion.framework/CoreMotion`

`EOF`

---

## `Full Report`

`{"app_name":"Pixio","timestamp":"2022-11-07 08:47:15.00 +0200","app_version":"3.0.1","slice_uuid":"cd2c3937-e0ba-3626-b5fa-08a4f3d77505","adam_id":"1251460891","build_version":"55","platform":2,"bundleID":"site.pixio.pixio","share_with_app_devs":0,"is_first_party":0,"bug_type":"309","os_version":"iPhone OS 16.1 (20B82)","roots_installed":0,"name":"Pixio","incident_id":"3D0E8E2C-BE27-4BF1-9305-849139E63B9B"}`

`{`

`"uptime" : 430000,`

`"procRole" : "Background",`

`"version" : 2,`

`"userID" : 501,`

`"deployVersion" : 210,`

`"modelCode" : "iPhone11,8",`

`"coalitionID" : 4029,`

`"osVersion" : {
"isEmbedded" : true,
"train" : "iPhone OS 16.1",
"releaseType" : "User",
"build" : "20B82"`

`},`

`"captureTime" : "2022-11-07 08:47:13.6399 +0200",`

`"incident" : "3D0E8E2C-BE27-4BF1-9305-849139E63B9B",`

`"pid" : 64385,`

`"cpuType" : "ARM-64",`

`"roots_installed" : 0,`

`"bug_type" : "309",`

`"procLaunch" : "2022-11-07 08:42:17.5421 +0200",`

`"procStartAbsTime" : 10332803676439,`

`"procExitAbsTime" : 10339907730813,`

`"procName" : "Pixio",`

`"procPath" : "/private/var/containers/Bundle/Application/D7BCF619-928F-427F-8FE5-45F23D8B8B25/Pixio.app/Pixio",`

`"bundleInfo" : {"CFBundleShortVersionString":"3.0.1","CFBundleVersion":"55","CFBundleIdentifier":"site.pixio.pixio","DTAppStoreToolsBuild":"13F100"},`

`"storeInfo" : {"storeCohortMetadata":"10|date=1667048400000&sf=143492&pgtp=Software&pgid=1251460891&prpg=Search_fef4f99b-bd35-4829-ba40-7c0bf8387403&ctxt=Search&issrch=1&lngid=29","itemID":"1251460891","deviceIdentifierForVendor":"48FB28B2-CF3C-4E87-B33E-7D31C2F52688","softwareVersionExternalIdentifier":"851779253","thirdParty":true,"applicationVariant":"1:iPhone11,8:15"},`

`"parentProc" : "launchd",`

`"parentPid" : 1,`

`"coalitionName" : "site.pixio.pixio",`

`"crashReporterKey" : "b61e142826e16bb63a98a6aac5262af9c6bb9ea8",`

`"basebandVersion" : "5.01.01",`

`"exception" : {"codes":"0x0000000000000000, 0x0000000000000000","rawCodes":[0,0],"type":"EXC_CRASH","signal":"SIGKILL"},`

`"termination" : {"code":2343432205,"flags":6,"namespace":"FRONTBOARD","reasons":["<RBSTerminateContext| domain:10 code:0x8BADF00D explanation:scene-update watchdog transgression: application<site.pixio.pixio>:64385 exhausted real (wall clock) time allowance of 10.00 seconds","ProcessVisibility: Background","ProcessState: Running","WatchdogEvent: scene-update","WatchdogVisibility: Background","WatchdogCPUStatistics: (",""Elapsed total CPU time (seconds): 20.190 (user 20.190, system 0.000), 34% CPU",",""Elapsed application CPU time (seconds): 0.286, 0% CPU"",") reportType:CrashLog maxTerminationResistance:Interactive>"]},`

`"ktriageinfo" : "VM - pmap_enter retried due to resource shortage\nVM - pmap_enter retried due to resource shortage\nVM - pmap_enter retried due to resource shortage\nVM - pmap_enter retried due to resource shortage\nVM - pmap_enter retried due to resource shortage\n",`

`"faultingThread" : 0,`

`"threads" : [{"triggered":true,"id":3405943,"threadState":{"x":[{"value":260},{"value":0},{"value":0},{"value":0},{"value":0},{"value":160},{"value":0},{"value":0},{"value":6130109256},{"value":0},{"value":5199398736},{"value":2},{"value":0},{"value":0},{"value":0},{"value":0},{"value":305},{"value":9153882776},{"value":0},{"value":5199398712},{"value":5199398776},{"value":9069418976,"symbolLocation":224,"symbol":"main_thread"},{"value":0},{"value":0},{"value":0},{"value":1},{"value":256},{"value":7521407056,"symbolLocation":0,"symbol":"swiftmetadataimplFixedSizeBufferValueWitnesses<swiftmetadataimplValueWitnesses<swiftmetadataimplNativeBox<unsigned long long, 8ul, 8ul, 8ul> >, true, 8ul, 8ul, false>getEnumTagSinglePayload(swiftOpaqueValue const*, unsigned int, swiftTargetMetadata`[`swift::InProcess`](swift::InProcess)` const*)"},{"value":9079151136,"symbolLocation":0,"symbol":"_swiftEmptyArrayStorage"}],"flavor":"ARM_THREAD_STATE64","lr":{"value":8912089196},"cpsr":{"value":1610612736},"fp":{"value":6130109376},"sp":{"value":6130109232},"esr":{"value":1442840704,"description":" Address size fault"},"pc":{"value":8639030300,"matchesCrashFrame":1},"far":{"value":18446743936753627220}},"queue":"com.apple.main-thread","frames":[{"imageOffset":5148,"symbol":"__psynch_cvwait","symbolLocation":8,"imageIndex":0},{"imageOffset":32876,"symbol":"_pthread_cond_wait","symbolLocation":1232,"imageIndex":1},{"imageOffset":784316,"symbol":"-[CADisplayLink invalidate]","symbolLocation":92,"imageIndex":2},{"imageOffset":2182560,"symbol":"-[SCNDisplayLink invalidate]","symbolLocation":64,"imageIndex":3},{"imageOffset":2378776,"symbol":"-[SCNView dealloc]","symbolLocation":116,"imageIndex":3},{"imageOffset":2535628,"imageIndex":4},{"imageOffset":441052,"imageIndex":5},{"imageOffset":4044120,"symbol":"(anonymous namespace)destroyGenericBox(swiftHeapObject*)","symbolLocation":152,"imageIndex":6},{"imageOffset":4038964,"symbol":"_swift_release_dealloc","symbolLocation":56,"imageIndex":6},{"imageOffset":15234956,"imageIndex":5},{"imageOffset":4038964,"symbol":"_swift_release_dealloc","symbolLocation":56,"imageIndex":6},{"imageOffset":3977876,"symbol":"swift_arrayDestroy","symbolLocation":124,"imageIndex":6},{"imageOffset":664692,"symbol":"_ContiguousArrayStorage.__deallocating_deinit","symbolLocation":96,"imageIndex":6},{"imageOffset":4038964,"symbol":"_swift_release_dealloc","symbolLocation":56,"imageIndex":6},{"imageOffset":3977876,"symbol":"swift_arrayDestroy","symbolLocation":124,"imageIndex":6},{"imageOffset":664692,"symbol":"_ContiguousArrayStorage.__deallocating_deinit","symbolLocation":96,"imageIndex":6},{"imageOffset":4038964,"symbol":"_swift_release_dealloc","symbolLocation":56,"imageIndex":6},{"imageOffset":16687240,"imageIndex":5},{"imageOffset":18109884,"imageIndex":5},{"imageOffset":8068916,"imageIndex":5},{"imageOffset":8079240,"imageIndex":5},{"imageOffset":839416,"imageIndex":5},{"imageOffset":2195360,"imageIndex":5},{"imageOffset":202084,"symbol":"+[UIView(Animation) performWithoutAnimation:]","symbolLocation":76,"imageIndex":7},{"imageOffset":400980,"imageIndex":5},{"imageOffset":121548,"imageIndex":5},{"imageOffset":789488,"imageIndex":5},{"imageOffset":60300,"imageIndex":5},{"imageOffset":51088,"imageIndex":5},{"imageOffset":56740,"imageIndex":5},{"imageOffset":167836,"symbol":"CADisplayDisplayLinkdispatch_items(unsigned long long, unsigned long long, unsigned long long)","symbolLocation":756,"imageIndex":2},{"imageOffset":239780,"symbol":"display_timer_callback(__CFMachPort*, void*, long, void*)","symbolLocation":372,"imageIndex":2},{"imageOffset":505888,"symbol":"__CFMachPortPerform","symbolLocation":176,"imageIndex":8},{"imageOffset":625920,"symbol":"CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE1_PERFORM_FUNCTION","symbolLocation":60,"imageIndex":8},{"imageOffset":633096,"symbol":"__CFRunLoopDoSource1","symbolLocation":520,"imageIndex":8},{"imageOffset":508220,"symbol":"__CFRunLoopRun","symbolLocation":2264,"imageIndex":8},{"imageOffset":528084,"symbol":"CFRunLoopRunSpecific","symbolLocation":612,"imageIndex":8},{"imageOffset":4968,"symbol":"GSEventRunModal","symbolLocation":164,"imageIndex":9},{"imageOffset":3810256,"symbol":"-[UIApplication run]","symbolLocation":888,"imageIndex":7},{"imageOffset":3809332,"symbol":"UIApplicationMain","symbolLocation":340,"imageIndex":7},{"imageOffset":217864,"symbol":"UIApplicationMain(::::)","symbolLocation":104,"imageIndex":10},{"imageOffset":45936,"imageIndex":4},{"imageOffset":88416,"symbol":"start","symbolLocation":2528,"imageIndex":11}]},{"id":3405971,"name":"com.apple.uikit.eventfetch-thread","frames":[{"imageOffset":2888,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":0},{"imageOffset":77832,"symbol":"mach_msg2_internal","symbolLocation":80,"imageIndex":0},{"imageOffset":78408,"symbol":"mach_msg_overwrite","symbolLocation":388,"imageIndex":0},{"imageOffset":4236,"symbol":"mach_msg","symbolLocation":24,"imageIndex":0},{"imageOffset":502512,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":160,"imageIndex":8},{"imageOffset":507188,"symbol":"__CFRunLoopRun","symbolLocation":1232,"imageIndex":8},{"imageOffset":528084,"symbol":"CFRunLoopRunSpecific","symbolLocation":612,"imageIndex":8},{"imageOffset":271156,"symbol":"-[NSRunLoop(NSRunLoop) runMode:beforeDate:]","symbolLocation":212,"imageIndex":12},{"imageOffset":270876,"symbol":"-[NSRunLoop(NSRunLoop) runUntilDate:]","symbolLocation":64,"imageIndex":12},{"imageOffset":5075772,"symbol":"-[UIEventFetcher threadMain]","symbolLocation":436,"imageIndex":7},{"imageOffset":374792,"symbol":"NSThread__start","symbolLocation":716,"imageIndex":12},{"imageOffset":5836,"symbol":"_pthread_start","symbolLocation":148,"imageIndex":1},{"imageOffset":2980,"symbol":"thread_start","symbolLocation":8,"imageIndex":1}]},{"id":3405998,"name":"com.google.firebase.crashlytics.MachExceptionServer","frames":[{"imageOffset":2888,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":0},{"imageOffset":77832,"symbol":"mach_msg2_internal","symbolLocation":80,"imageIndex":0},{"imageOffset":78408,"symbol":"mach_msg_overwrite","symbolLocation":388,"imageIndex":0},{"imageOffset":4236,"symbol":"mach_msg","symbolLocation":24,"imageIndex":0},{"imageOffset":18310268,"imageIndex":4},{"imageOffset":5836,"symbol":"_pthread_start","symbolLocation":148,"imageIndex":1},{"imageOffset":2980,"symbol":"thread_start","symbolLocation":8,"imageIndex":1}]},{"id":3406004,"name":"com.apple.NSURLConnectionLoader","frames":[{"imageOffset":2888,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":0},{"imageOffset":77832,"symbol":"mach_msg2_internal","symbolLocation":80,"imageIndex":0},{"imageOffset":78408,"symbol":"mach_msg_overwrite","symbolLocation":388,"imageIndex":0},{"imageOffset":4236,"symbol":"mach_msg","symbolLocation":24,"imageIndex":0},{"imageOffset":502512,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":160,"imageIndex":8},{"imageOffset":507188,"symbol":"__CFRunLoopRun","symbolLocation":1232,"imageIndex":8},{"imageOffset":528084,"symbol":"CFRunLoopRunSpecific","symbolLocation":612,"imageIndex":8},{"imageOffset":2450856,"imageIndex":13},{"imageOffset":374792,"symbol":"NSThread__start","symbolLocation":716,"imageIndex":12},{"imageOffset":5836,"symbol":"_pthread_start","symbolLocation":148,"imageIndex":1},{"imageOffset":2980,"symbol":"thread_start","symbolLocation":8,"imageIndex":1}]},{"id":3406012,"queue":"com.apple.root.user-initiated-qos","frames":[{"imageOffset":2888,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":0},{"imageOffset":77832,"symbol":"mach_msg2_internal","symbolLocation":80,"imageIndex":0},{"imageOffset":78408,"symbol":"mach_msg_overwrite","symbolLocation":388,"imageIndex":0},{"imageOffset":4236,"symbol":"mach_msg","symbolLocation":24,"imageIndex":0},{"imageOffset":502512,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":160,"imageIndex":8},{"imageOffset":507188,"symbol":"__CFRunLoopRun","symbolLocation":1232,"imageIndex":8},{"imageOffset":528084,"symbol":"CFRunLoopRunSpecific","symbolLocation":612,"imageIndex":8},{"imageOffset":271156,"symbol":"-[NSRunLoop(NSRunLoop) runMode:beforeDate:]","symbolLocation":212,"imageIndex":12},{"imageOffset":270792,"symbol":"-[NSRunLoop(NSRunLoop) run]","symbolLocation":64,"imageIndex":12},{"imageOffset":8863152,"imageIndex":4},{"imageOffset":1536844,"imageIndex":4},{"imageOffset":9396,"symbol":"_dispatch_call_block_and_release","symbolLocation":32,"imageIndex":14},{"imageOffset":16348,"symbol":"_dispatch_client_callout","symbolLocation":20,"imageIndex":14},{"imageOffset":88972,"symbol":"_dispatch_root_queue_drain","symbolLocation":684,"imageIndex":14},{"imageOffset":90756,"symbol":"_dispatch_worker_thread2","symbolLocation":164,"imageIndex":14},{"imageOffset":3516,"symbol":"_pthread_wqthread","symbolLocation":228,"imageIndex":1},{"imageOffset":2968,"symbol":"start_wqthread","symbolLocation":8,"imageIndex":1}]},{"id":3407158,"name":"com.apple.CoreMotion.MotionThread","frames":[{"imageOffset":2888,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":0},{"imageOffset":77832,"symbol":"mach_msg2_internal","symbolLocation":80,"imageIndex":0},{"imageOffset":78408,"symbol":"mach_msg_overwrite","symbolLocation":388,"imageIndex":0},{"imageOffset":4236,"symbol":"mach_msg","symbolLocation":24,"imageIndex":0},{"imageOffset":502512,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":160,"imageIndex":8},{"imageOffset":507188,"symbol":"__CFRunLoopRun","symbolLocation":1232,"imageIndex":8},{"imageOffset":528084,"symbol":"CFRunLoopRunSpecific","symbolLocation":612,"imageIndex":8},{"imageOffset":806148,"symbol":"CFRunLoopRun","symbolLocation":64,"imageIndex":8},{"imageOffset":81600,"imageIndex":15},{"imageOffset":5836,"symbol":"_pthread_start","symbolLocation":148,"imageIndex":1},{"imageOffset":2980,"symbol":"thread_start","symbolLocation":8,"imageIndex":1}]},{"id":3408482,"frames":[{"imageOffset":2960,"symbol":"start_wqthread","symbolLocation":0,"imageIndex":1}]},{"id":3409011,"frames":[{"imageOffset":2960,"symbol":"start_wqthread","symbolLocation":0,"imageIndex":1}]},{"id":3409075,"name":"com.apple.SwiftUI.AsyncRenderer","frames":[{"imageOffset":6984,"symbol":"__psynch_mutexwait","symbolLocation":8,"imageIndex":0},{"imageOffset":8528,"symbol":"_pthread_mutex_firstfit_lock_wait","symbolLocation":84,"imageIndex":1},{"imageOffset":37648,"symbol":"_pthread_mutex_firstfit_lock_slow","symbolLocation":248,"imageIndex":1},{"imageOffset":73140,"symbol":"_MovableLockLock","symbolLocation":48,"imageIndex":5},{"imageOffset":696376,"imageIndex":5},{"imageOffset":688488,"imageIndex":5},{"imageOffset":374792,"symbol":"NSThread__start","symbolLocation":716,"imageIndex":12},{"imageOffset":5836,"symbol":"_pthread_start","symbolLocation":148,"imageIndex":1},{"imageOffset":2980,"symbol":"thread_start","symbolLocation":8,"imageIndex":1}]},{"id":3409080,"frames":[{"imageOffset":2960,"symbol":"start_wqthread","symbolLocation":0,"imageIndex":1}]},{"id":3409100,"frames":[{"imageOffset":2960,"symbol":"start_wqthread","symbolLocation":0,"imageIndex":1}]},{"id":3409101,"frames":[{"imageOffset":2960,"symbol":"start_wqthread","symbolLocation":0,"imageIndex":1}]},{"id":3409129,"name":"com.apple.scenekit.scnview-renderer","frames":[{"imageOffset":2888,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":0},{"imageOffset":77832,"symbol":"mach_msg2_internal","symbolLocation":80,"imageIndex":0},{"imageOffset":78408,"symbol":"mach_msg_overwrite","symbolLocation":388,"imageIndex":0},{"imageOffset":4236,"symbol":"mach_msg","symbolLocation":24,"imageIndex":0},{"imageOffset":502512,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":160,"imageIndex":8},{"imageOffset":507188,"symbol":"__CFRunLoopRun","symbolLocation":1232,"imageIndex":8},{"imageOffset":528084,"symbol":"CFRunLoopRunSpecific","symbolLocation":612,"imageIndex":8},{"imageOffset":271156,"symbol":"-[NSRunLoop(NSRunLoop) runMode:beforeDate:]","symbolLocation":212,"imageIndex":12},{"imageOffset":1229940,"symbol":"__85-[SCNView(SCNDisplayLink) _initializeDisplayLinkWithScreen:policy:completionHandler:]_block_invoke","symbolLocation":460,"imageIndex":3},{"imageOffset":1230204,"symbol":"SCNRenderThread_start","symbolLocation":80,"imageIndex":3},{"imageOffset":5836,"symbol":"_pthread_start","symbolLocation":148,"imageIndex":1},{"imageOffset":2980,"symbol":"thread_start","symbolLocation":8,"imageIndex":1}]},{"id":3409130,"name":"com.apple.scenekit.scnview-renderer","frames":[{"imageOffset":6984,"symbol":"__psynch_mutexwait","symbolLocation":8,"imageIndex":0},{"imageOffset":35988,"symbol":"_pthread_mutex_fairshare_lock_wait","symbolLocation":84,"imageIndex":1},{"imageOffset":35820,"symbol":"_pthread_mutex_fairshare_lock_slow","symbolLocation":196,"imageIndex":1},{"imageOffset":2182124,"symbol":"-[SCNDisplayLink _displayLinkCallbackWaitingOnFrameCompletionWithTime:]","symbolLocation":48,"imageIndex":3},{"imageOffset":167836,"symbol":"CADisplayDisplayLink::dispatch_items(unsigned long long, unsigned long long, unsigned long long)","symbolLocation":756,"imageIndex":2},{"imageOffset":239780,"symbol":"display_timer_callback(__CFMachPort*, void*, long, void*)","symbolLocation":372,"imageIndex":2},{"imageOffset":505888,"symbol":"__CFMachPortPerform","symbolLocation":176,"imageIndex":8},{"imageOffset":625920,"symbol":"CFRUNLOOP_IS_CALLING_OUT_TO_A_SOURCE1_PERFORM_FUNCTION","symbolLocation":60,"imageIndex":8},{"imageOffset":633096,"symbol":"__CFRunLoopDoSource1","symbolLocation":520,"imageIndex":8},{"imageOffset":508220,"symbol":"__CFRunLoopRun","symbolLocation":2264,"imageIndex":8},{"imageOffset":528084,"symbol":"CFRunLoopRunSpecific","symbolLocation":612,"imageIndex":8},{"imageOffset":271156,"symbol":"-[NSRunLoop(NSRunLoop) runMode:beforeDate:]","symbolLocation":212,"imageIndex":12},{"imageOffset":1229940,"symbol":"__85-[SCNView(SCNDisplayLink) _initializeDisplayLinkWithScreen:policy:completionHandler:]_block_invoke","symbolLocation":460,"imageIndex":3},{"imageOffset":1230204,"symbol":"SCNRenderThread_start","symbolLocation":80,"imageIndex":3},{"imageOffset":5836,"symbol":"_pthread_start","symbolLocation":148,"imageIndex":1},{"imageOffset":2980,"symbol":"thread_start","symbolLocation":8,"imageIndex":1}]},{"id":3409134,"name":"com.apple.scenekit.scnview-renderer","frames":[{"imageOffset":2888,"symbol":"mach_msg2_trap","symbolLocation":8,"imageIndex":0},{"imageOffset":77832,"symbol":"mach_msg2_internal","symbolLocation":80,"imageIndex":0},{"imageOffset":78408,"symbol":"mach_msg_overwrite","symbolLocation":388,"imageIndex":0},{"imageOffset":4236,"symbol":"mach_msg","symbolLocation":24,"imageIndex":0},{"imageOffset":502512,"symbol":"__CFRunLoopServiceMachPort","symbolLocation":160,"imageIndex":8},{"imageOffset":507188,"symbol":"__CFRunLoopRun","symbolLocation":1232,"imageIndex":8},{"imageOffset":528084,"symbol":"CFRunLoopRunSpecific","symbolLocation":612,"imageIndex":8},{"imageOffset":271156,"symbol":"-[NSRunLoop(NSRunLoop) runMode:beforeDate:]","symbolLocation":212,"imageIndex":12},{"imageOffset":1229940,"symbol":"__85-[SCNView(SCNDisplayLink) _initializeDisplayLinkWithScreen:policy:completionHandler:]_block_invoke","symbolLocation":460,"imageIndex":3},{"imageOffset":1230204,"symbol":"SCNRenderThread_start","symbolLocation":80,"imageIndex":3},{"imageOffset":5836,"symbol":"_pthread_start","symbolLocation":148,"imageIndex":1},{"imageOffset":2980,"symbol":"thread_start","symbolLocation":8,"imageIndex":1}]}],`

`"usedImages" : [`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 8639025152,
"size" : 225276,
"uuid" : "ff27fc8f-90ba-3332-ab7a-c5bc2d9ca7b1",
"path" : "/usr/lib/system/libsystem_kernel.dylib",
"name" : "libsystem_kernel.dylib"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 8912056320,
"size" : 49152,
"uuid" : "1aa3a4b6-f9e7-3056-8c8b-4e4dd81312a4",
"path" : "/usr/lib/system/libsystem_pthread.dylib",
"name" : "libsystem_pthread.dylib"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7643455488,
"size" : 3526656,
"uuid" : "046338bf-09cf-3414-bc93-31296b97eb2d",
"path" : "/System/Library/Frameworks/QuartzCore.framework/QuartzCore",
"name" : "QuartzCore"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 8881573888,
"size" : 5132288,
"uuid" : "5d296524-c7b4-3c39-b5f7-72333e51f852",
"path" : "/System/Library/Frameworks/SceneKit.framework/SceneKit",
"name" : "SceneKit"`

`},`

`{
"source" : "P",
"arch" : "arm64",
"base" : 4336762880,
"size" : 25968640,
"uuid" : "cd2c3937-e0ba-3626-b5fa-08a4f3d77505",
"path" : "/private/var/containers/Bundle/Application/D7BCF619-928F-427F-8FE5-45F23D8B8B25/Pixio.app/Pixio",
"name" : "Pixio"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7680208896,
"size" : 26492928,
"uuid" : "494a7d57-90af-3e90-9623-7038275b8d87",
"path" : "/System/Library/Frameworks/SwiftUI.framework/SwiftUI",
"name" : "SwiftUI"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7517360128,
"size" : 5672960,
"uuid" : "f896d145-e025-39d6-afd3-bc0a2ad4f839",
"path" : "/usr/lib/swift/libswiftCore.dylib",
"name" : "libswiftCore.dylib"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7655182336,
"size" : 25026560,
"uuid" : "179501b6-0fc2-344a-b969-b4e3961ebe10",
"path" : "/System/Library/PrivateFrameworks/UIKitCore.framework/UIKitCore",
"name" : "UIKitCore"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7619805184,
"size" : 4087808,
"uuid" : "5cdc5d9a-e506-3740-b64e-bb30867b4f1b",
"path" : "/System/Library/Frameworks/CoreFoundation.framework/CoreFoundation",
"name" : "CoreFoundation"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 8579780608,
"size" : 36864,
"uuid" : "a633a095-1226-3942-8f41-3877660185ee",
"path" : "/System/Library/PrivateFrameworks/GraphicsServices.framework/GraphicsServices",
"name" : "GraphicsServices"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7765663744,
"size" : 479232,
"uuid" : "6383e8e8-6726-3391-8d95-bb5ee497e9aa",
"path" : "/usr/lib/swift/libswiftUIKit.dylib",
"name" : "libswiftUIKit.dylib"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 8130277376,
"size" : 536592,
"uuid" : "cb3ff411-4762-34d2-86a4-eca13f9fb6c3",
"path" : "/usr/lib/dyld",
"name" : "dyld"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7523237888,
"size" : 9740288,
"uuid" : "c431acb6-fe04-3d28-b677-4de6e1c7d81f",
"path" : "/System/Library/Frameworks/Foundation.framework/Foundation",
"name" : "Foundation"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7638163456,
"size" : 3964928,
"uuid" : "edb0559f-c996-327f-9b3a-6616e316f24d",
"path" : "/System/Library/Frameworks/CFNetwork.framework/CFNetwork",
"name" : "CFNetwork"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7743365120,
"size" : 290816,
"uuid" : "fea36690-a000-3c55-b700-9120b05aa69b",
"path" : "/usr/lib/system/libdispatch.dylib",
"name" : "libdispatch.dylib"`

`},`

`{
"source" : "P",
"arch" : "arm64e",
"base" : 7810191360,
"size" : 4116480,
"uuid" : "958c1c71-4f38-3d53-a2b6-5f0182d618e1",
"path" : "/System/Library/Frameworks/CoreMotion.framework/CoreMotion",
"name" : "CoreMotion"`

`}`

`],`

`"sharedCache" : {`

`"base" : 7504920576,`

`"size" : 2890694656,`

`"uuid" : "06b67cff-3b92-3043-800e-0f483723ed91"`

`},`

`"vmSummary" : "ReadOnly portion of Libraries: Total=1.1G resident=0K(0%) swapped_out_or_unallocated=1.1G(100%)\nWritable regions: Total=654.7M written=0K(0%) resident=0K(0%) swapped_out=0K(0%) unallocated=654.7M(100%)\n\n                                VIRTUAL   REGION \nREGION TYPE                        SIZE    COUNT (non-coalesced) \n=                     =  = \nAccelerate framework               128K        1 \nActivity Tracing                   256K        1 \nCG raster data                     480K        8 \nColorSync                          496K       26 \nCoreAnimation                      608K       35 \nFoundation                        1248K        6 \nKernel Alloc Once                   32K        1 \nMALLOC                           624.1M      440 \nMALLOC guard page                  192K       12 \nSQLite page cache                 2048K       16 \nSTACK GUARD                        224K       14 \nStack                             18.5M      353 \nVM_ALLOCATE                       4384K       17 \nVM_ALLOCATE (reserved)             128K        2         reserved VM address space (unallocated)\n__AUTH                            3885K      563 \n__AUTH_CONST                      30.8M      782 \n__CTF                               756        1 \n__DATA                            16.1M      772 \n__DATA_CONST                      37.5M      788 \n__DATA_DIRTY                      3481K      632 \n__FONT_DATA                        2352        1 \n__LINKEDIT                       307.5M        3 \n__OBJC_CONST                      7138K      533 \n__OBJC_RO                         78.4M        1 \n__OBJC_RW                         2427K        1 \n__TEXT                           834.5M      803 \ndyld private memory                256K        1 \nlibnetwork                        1664K       24 \nmapped file                      340.4M      141 \nshared memory                     2096K        5 \n=                     =  = \nTOTAL                              2.3G     5983 \nTOTAL, minus reserved VM space     2.3G     5983 \n",`

`"legacyInfo" : {`

`"threadTriggered" : {
"queue" : "com.apple.main-thread"`

`}`

`},`

`"trialInfo" : {`

`"rollouts" : [
{
"rolloutId" : "62fe74515312cd4599bd3c80",
"factorPackIds" : {
"MYRIAD_BOOSTS" : "62fe74805312cd4599bd3c81"
},
"deploymentId" : 240000006
},
{
"rolloutId" : "6081ed9716bb6d61d81d5014",
"factorPackIds" : {
"BIFROST_PROD_1" : "636541ec7ea6e25a76dc2019"
},
"deploymentId" : 240002047
}`

`],`

`"experiments" : [
{
"treatmentId" : "c1eda467-5c09-4fd6-8d90-7034cc98438f",
"experimentId" : "62cf21389a1c885618978432",
"deploymentId" : 400000006
},
{
"treatmentId" : "a2c66376-6910-4142-b340-3476dd2ce1bf",
"experimentId" : "621923057b59736391be1571",
"deploymentId" : 400000011
}`

`]`

`}`

`}`
