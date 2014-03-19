Building-info-and-errors
========================

hhp211@hhp211-Q500A:~$ rm -rf /home/hhp211/android_vendor_samsung_fascinatemtd
hhp211@hhp211-Q500A:~$ rm -rf /home/hhp211/Source/AOSPA/device/samsung
hhp211@hhp211-Q500A:~$ rm -rf /home/hhp211/Source/AOSPA/vendor
hhp211@hhp211-Q500A:~$ rm -rf /home/hhp211/Source/AOSPA/kernel
hhp211@hhp211-Q500A:~$ rm -rf /home/hhp211/Source/AOSPA/out


hhp211@hhp211-Q500A:~$ cd ~/Source/AOSPA
hhp211@hhp211-Q500A:~/Source/AOSPA$ repo sync -j6
Traceback (most recent call last):
  File "/home/hhp211/Source/AOSPA/.repo/repo/main.py", line 408, in <module>
    _Main(sys.argv[1:])
  File "/home/hhp211/Source/AOSPA/.repo/repo/main.py", line 384, in _Main
    result = repo._Run(argv) or 0
  File "/home/hhp211/Source/AOSPA/.repo/repo/main.py", line 127, in _Run
    copts, cargs = cmd.OptionParser.parse_args(argv)
  File "/home/hhp211/Source/AOSPA/.repo/repo/command.py", line 67, in OptionParser
    self._Options(self._optparse)
  File "/home/hhp211/Source/AOSPA/.repo/repo/subcmds/sync.py", line 163, in _Options
    self.jobs = self.manifest.default.sync_j
  File "/home/hhp211/Source/AOSPA/.repo/repo/manifest_xml.py", line 314, in default
    self._Load()
  File "/home/hhp211/Source/AOSPA/.repo/repo/manifest_xml.py", line 354, in _Load
    b = m.GetBranch(m.CurrentBranch).merge
  File "/home/hhp211/Source/AOSPA/.repo/repo/project.py", line 590, in CurrentBranch
    b = self.work_git.GetHead()
  File "/home/hhp211/Source/AOSPA/.repo/repo/project.py", line 2265, in GetHead
    raise NoManifestException(path)
error.NoManifestException: /home/hhp211/Source/AOSPA/.repo/manifests/.git/HEAD


hhp211@hhp211-Q500A:~/Source/AOSPA$ repo init -u git://github.com/AOSPA-legacy/manifest.git -b kitkat
Get git://github.com/AOSPA-legacy/manifest.git
remote: Counting objects: 519, done.
remote: Compressing objects: 100% (254/254), done.
remote: Total 519 (delta 231), reused 504 (delta 218)
Receiving objects: 100% (519/519), 110.25 KiB | 0 bytes/s, done.
Resolving deltas: 100% (231/231), done.
From git://github.com/AOSPA-legacy/manifest
 * [new branch]      kitkat     -> origin/kitkat

Your identity is: hhp211 <hhp211@gmail.com>
If you want to change this, please re-run 'repo init' with --config-name

repo has been initialized in /home/hhp211/Source/AOSPA
hhp211@hhp211-Q500A:~/Source/AOSPA$ repo sync -j6


Fetching project AOSPA-legacy/android_system_core
Fetching project platform/external/eclipse-basebuilder
Fetching project CyanogenMod/android_external_libnfc-nci
Fetching project CyanogenMod/android_dalvik
Fetching project platform/prebuilts/clang/linux-x86/x86/3.3
Fetching project CyanogenMod/android_external_libpng
Fetching projects:   0% (1/390)  Fetching project platform/external/icu4c
Fetching project platform/frameworks/opt/mailcommon
Fetching project platform/external/speex
Fetching projects:   1% (4/390)  Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-eabi-4.7
Fetching project platform/external/jdiff
Fetching project platform/prebuilts/runtime
Fetching project platform/external/mksh
Fetching projects:   2% (8/390)  Fetching project platform/external/linux-tools-perf
Fetching project platform/external/chromium_org/tools/gyp
Fetching project platform/developers/samples/android
Fetching project platform/packages/experimental
Fetching projects:   3% (12/390)  Fetching project platform/frameworks/opt/colorpicker
Fetching project platform/external/fsck_msdos
Fetching project platform/external/arduino
Fetching project platform/external/ipsec-tools
Fetching projects:   4% (16/390)  Fetching project AOSPA-legacy/android_frameworks_native
Fetching project platform/prebuilts/python/linux-x86/2.7.5
Fetching project platform/packages/apps/VideoEditor
Fetching project platform/packages/apps/DeskClock
Fetching projects:   5% (20/390)  Fetching project CyanogenMod/android_device_common
Fetching project platform/external/pixman
Fetching project platform/external/libphonenumber
Fetching project platform/external/nist-sip
Fetching projects:   6% (24/390)  Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-eabi-4.7
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-eabi-4.6
Fetching project platform/frameworks/volley
Fetching project platform/packages/apps/SpareParts
Fetching projects:   7% (28/390)  Fetching project platform/external/dhcpcd
Fetching project platform/prebuilts/clang/linux-x86/host/3.3
Fetching project CyanogenMod/android_external_connectivity
Fetching project device/google/accessory/arduino
Fetching projects:   8% (32/390)  Fetching project platform/external/bison
Fetching project platform/packages/providers/ApplicationsProvider
Fetching project platform/external/tinyxml
Fetching project platform/external/openssl
Fetching projects:   9% (36/390)  Fetching project platform/packages/providers/UserDictionaryProvider
Fetching project platform/prebuilts/clang/darwin-x86/arm/3.3
Fetching project platform/external/lzma
Fetching projects:  10% (39/390)  Fetching project platform/external/libxslt
Fetching project platform/external/neven
Fetching project platform/packages/apps/CertInstaller
Fetching project platform/external/harfbuzz
Fetching projects:  11% (43/390)  Fetching project platform/external/ganymed-ssh2
Fetching project platform/packages/wallpapers/HoloSpiral
Fetching project platform/external/libgsm
Fetching project platform/external/open-vcdiff
Fetching projects:  12% (47/390)  Fetching project platform/prebuilts/tools
Fetching project CyanogenMod/android_external_clang
Fetching project platform/external/valgrind
Fetching project AOSPA-legacy/android_frameworks_opt_telephony
Fetching projects:  13% (51/390)  Fetching project platform/prebuilts/clang/darwin-x86/3.1
Fetching project platform/prebuilts/gcc/linux-x86/x86/i686-linux-android-4.7
Fetching project CyanogenMod/android_external_crda
Fetching project platform/external/chromium_org/third_party/yasm/source/patched-yasm
Fetching projects:  14% (55/390)  Fetching project platform/external/blktrace
Fetching project CyanogenMod/android_external_libusb
Fetching project platform/external/qemu-pc-bios
Fetching project platform/prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.7
Fetching projects:  15% (59/390)  Fetching project device/generic/armv7-a-neon
remote: Counting objects: 17, done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 17 (delta 2), reused 6 (delta 0)
Fetching project platform/frameworks/ex
Unpacking objects: 100% (17/17), done.
Fetching project platform/external/chromium_org/third_party/leveldatabase/src
From https://github.com/AOSPA-legacy/android_frameworks_opt_telephony
 + 223177e...f1dbd17 kitkat     -> github/kitkat  (forced update)
Fetching project platform/prebuilts/clang/darwin-x86/3.2
Fetching projects:  16% (63/390)  Fetching project CyanogenMod/android_packages_providers_MediaProvider
Fetching project device/generic/common
Fetching project platform/prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.7-4.6
Fetching project CyanogenMod/android_frameworks_webview
Fetching projects:  17% (67/390)  Fetching project platform/external/gtest
Fetching project CyanogenMod/android_packages_apps_Contacts
Fetching project CyanogenMod/android_prebuilts_misc
Fetching project platform/packages/apps/OneTimeInitializer
Fetching projects:  18% (71/390)  Fetching project platform/frameworks/opt/carddav
Fetching project platform/external/liblzf
Fetching project platform/external/hyphenation
Fetching project platform/prebuilts/gcc/darwin-x86/x86/i686-linux-android-4.7
Fetching projects:  19% (75/390)  Fetching project platform/external/doclava
Fetching project CyanogenMod/android_external_qrngd
Fetching project platform/external/eigen
Fetching projects:  20% (78/390)  Fetching project platform/external/guava
Fetching project device/generic/mini-emulator-mips
Fetching project platform/external/nist-pkits
Fetching project platform/packages/providers/CalendarProvider
Fetching projects:  21% (82/390)  Fetching project device/generic/x86
Fetching project platform/external/iproute2
Fetching project platform/external/chromium_org/third_party/WebKit
Fetching project platform/packages/wallpapers/MagicSmoke
Fetching projects:  22% (86/390)  Fetching project platform/external/openssh
Fetching project platform/packages/screensavers/WebView
Fetching project AOSPA-legacy/android_packages_apps_Mms
Fetching project platform/prebuilts/ndk
Fetching projects:  23% (90/390)  Fetching project platform/external/bouncycastle
Fetching project platform/external/libogg
Fetching project CyanogenMod/android_packages_apps_ContactsCommonFetching project platform/external/dropbear

Fetching projects:  24% (94/390)  Fetching project platform/external/gcc-demangle
Fetching project platform/prebuilts/gcc/darwin-x86/host/i686-apple-darwin-4.2.1
Fetching project AOSPA-legacy/android_external_bluetooth_bluedroid
Fetching project AOSPA-legacy/android_packages_apps_ScreenRecorder
Fetching projects:  25% (98/390)  Fetching project AOSPA-legacy/android_frameworks_av
Fetching project CyanogenMod/android_frameworks_opt_vcard
Fetching project platform/packages/providers/PartnerBookmarksProvider
Fetching project CyanogenMod/android_system_qcom
Fetching projects:  26% (102/390)  Fetching project device/generic/mini-emulator-x86
Fetching project platform/external/embunit
Fetching project platform/prebuilts/clang/linux-x86/3.2
Fetching project CyanogenMod/android_external_skia
Fetching projects:  27% (106/390)  Fetching project platform/external/chromium_org/third_party/libphonenumber/src/resources
Fetching project platform/external/dexmaker
Fetching project platform/external/mesa3d
Fetching project platform/prebuilts/gcc/linux-x86/x86/x86_64-linux-android-4.7
Fetching projects:  28% (110/390)  Fetching project platform/external/noto-fonts
Fetching project platform/external/chromium_org/third_party/libphonenumber/src/phonenumbers
Fetching project platform/external/libyuv
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.7
Fetching projects:  29% (114/390)  Fetching project platform/external/tinycompress
Fetching project CyanogenMod/android_system_netd
Fetching project platform/pdk
Fetching projects:  30% (117/390)  Fetching project CyanogenMod/android_system_extras
Fetching project AOSPA-legacy/android_packages_apps_InCallUI
Fetching project platform/external/v8
remote: Counting objects: 5, done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 5 (delta 0), reused 1 (delta 0)
Unpacking objects: 100% (5/5), done.
Fetching project platform/external/xmlwriter
Fetching projects:  31% (121/390)  Fetching project platform/external/libxml2
Fetching project device/generic/mips
Fetching project platform/external/javasqlite
Fetching project platform/external/smack
Fetching projects:  32% (125/390)  Fetching project platform/frameworks/opt/datetimepicker
Fetching project platform/frameworks/compile/libbcc
From https://github.com/AOSPA-legacy/android_frameworks_av
   47b4d24..44bf96c  kitkat     -> github/kitkat
Fetching project platform/external/safe-iop
Fetching project platform/ndk
Fetching projects:  33% (129/390)  Fetching project platform/tools/external/fat32lib
Fetching project CyanogenMod/android_external_sepolicy
Fetching project platform/docs/source.android.com
Fetching project platform/external/sil-fonts
Fetching projects:  34% (133/390)  Fetching project platform/packages/wallpapers/LivePicker
Fetching project platform/external/qemu
Fetching project platform/external/kernel-headers
Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-eabi-4.6
Fetching projects:  35% (137/390)  Fetching project platform/packages/apps/VoiceDialer
Fetching project platform/external/sfntly
Fetching project platform/frameworks/opt/photoviewer
Fetching project device/generic/goldfish
Fetching projects:  36% (141/390)  Fetching project CyanogenMod/android_frameworks_support
Fetching project platform/external/hamcrest
Fetching project platform/frameworks/testing
Fetching project platform/packages/apps/SpeechRecorder
Fetching projects:  37% (145/390)  Fetching project platform/external/okhttp
Fetching project platform/developers/demos
Fetching project platform/frameworks/opt/emoji
Fetching project platform/prebuilts/gcc/darwin-x86/host/headers
Fetching projects:  38% (149/390)  Fetching project platform/external/chromium_org/testing/gtest
Fetching project CyanogenMod/android_packages_apps_Gallery2
Fetching project CyanogenMod/android_bionic
Fetching project platform/external/chromium_org/third_party/openssl
Fetching projects:  39% (153/390)  Fetching project CyanogenMod/android_external_flac
Fetching project AOSPA-legacy/android_packages_services_Telephony
Fetching project platform/prebuilts/devtools
Fetching projects:  40% (156/390)  Fetching project platform/prebuilts/clang/linux-x86/arm/3.3
Fetching project platform/packages/wallpapers/MusicVisualization
Fetching project platform/external/libnl-headers
Fetching project platform/external/opencv
Fetching projects:  41% (160/390)  Fetching project platform/external/emma
Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.7
remote: Counting objects: 9, done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 9 (delta 0), reused 6 (delta 0)
Unpacking objects: 100% (9/9), done.
From git://github.com/CyanogenMod/android_packages_apps_Gallery2
   dea0b2c..701f333  cm-11.0    -> cm/cm-11.0
Fetching project platform/external/chromium_org/third_party/skia/src
Fetching project platform/external/libppp
Fetching projects:  42% (164/390)  Fetching project platform/packages/apps/CellBroadcastReceiver
Fetching project platform/frameworks/opt/inputmethodcommon
Fetching project platform/prebuilts/clang/linux-x86/3.1
Fetching project AOSPA-legacy/android_art
Fetching projects:  43% (168/390)  Fetching project platform/external/libvorbis
Fetching project platform/packages/apps/KeyChain
Fetching project platform/external/tagsoup
Fetching project AOSPA-legacy/android_packages_apps_Bluetooth
Fetching projects:  44% (172/390)  Fetching project CyanogenMod/Widgets
Fetching project platform/external/sqlite
Fetching project CyanogenMod/android_external_busybox
Fetching project CyanogenMod/android_external_e2fsprogs
Fetching projects:  45% (176/390)  Fetching project platform/external/oprofile
Fetching project platform/external/jpeg
Fetching project platform/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.4.3
Fetching project platform/external/elfutils
Fetching projects:  46% (180/390)  Fetching project platform/prebuilts/clang/darwin-x86/x86/3.3
Fetching project AOSPA-legacy/android_frameworks_base
Fetching project platform/external/libmtp
Fetching project platform/external/ant-glob
Fetching projects:  47% (184/390)  Fetching project platform/external/jsr305
Fetching project CyanogenMod/android_frameworks_opt_hardware
Fetching project platform/external/srec
Fetching project platform/packages/apps/Tag
Fetching projects:  48% (188/390)  Fetching project platform/external/apache-harmony
Fetching project platform/frameworks/opt/calendar
Fetching project CyanogenMod/android_packages_apps_Exchange
Fetching project CyanogenMod/android_frameworks_rs
Fetching projects:  49% (192/390)  Fetching project platform/external/stressapptest
Fetching project platform/external/webrtc
Fetching project platform/external/chromium_org/third_party/freetype
Fetching projects:  50% (195/390)  Fetching project platform/external/aac
Fetching project platform/external/proguard
Fetching project platform/frameworks/uiautomator
remote: Counting objects: 238, done.
remote: Compressing objects: 100% (146/146), done.
Fetching project AOSPA-legacy/manifest
Fetching projects:  51% (199/390)  Fetching project platform/external/tcpdump
Fetching project platform/bootable/recovery
Fetching project platform/external/chromium_org/third_party/mesa/src
Fetching project platform/external/chromium_org/third_party/opus/src
Fetching projects:  52% (203/390)  Fetching project CyanogenMod/android_packages_apps_Camera2
Fetching project platform/prebuilts/clang/linux-x86/mips/3.3
Fetching project AOSPA-legacy/android_vendor_pa
Fetching project platform/prebuilts/gcc/darwin-x86/x86/i686-linux-android-4.6
remote: Counting objects: 3, done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Unpacking objects: 100% (3/3), done.
Fetching projects:  53% (207/390)  Fetching project CyanogenMod/android_external_libsepol
From https://github.com/AOSPA-legacy/manifest
   e65548c..09315d1  kitkat     -> github/kitkat
Fetching project platform/external/replicaisland
Fetching project device/google/accessory/demokit00 KiB/s   
remote: Counting objects: 28, done.
remote: Compressing objects: 100% (18/18), done.
remote: Total 28 (delta 6), reused 4 (delta 0)
Unpacking objects: 100% (28/28), done.
Fetching project platform/prebuilts/python/darwin-x86/2.7.5
From https://github.com/AOSPA-legacy/android_vendor_pa
   b939e17..3f988b1  kitkat     -> github/kitkat
Fetching projects:  54% (211/390)  Fetching project CyanogenMod/android_packages_apps_Launcher3
Fetching project platform/external/giflib
Fetching project AOSPA-legacy/android_packages_apps_ParanoidOTA
Fetching project platform/external/chromium_org/third_party/libjingle/source/talk
Fetching projects:  55% (215/390)  Fetching project platform/prebuilts/clang/darwin-x86/host/3.3
Fetching project CyanogenMod/android_hardware_broadcom_wlan
Fetching project CyanogenMod/android_hardware_ril00 KiB/s   
Fetching project platform/packages/inputmethods/OpenWnn
remote: Counting objects: 21, done.
remote: Compressing objects: 100% (13/13), done.
remote: Total 21 (delta 6), reused 10 (delta 2)
remote: Counting objects: 19, done.
remote: Compressing objects: 100% (17/17), done.
remote: Total 19 (delta 5), reused 4 (delta 0)
Unpacking objects: 100% (19/19), done.
From https://github.com/AOSPA-legacy/android_packages_apps_ParanoidOTA
   31d8702..cb49091  kitkat     -> github/kitkat
Fetching projects:  56% (219/390)  Fetching project platform/sdk
Unpacking objects: 100% (21/21), done.
Fetching project platform/external/sonivox
Fetching project platform/packages/apps/MusicFX
From git://github.com/CyanogenMod/android_packages_apps_Camera2
   32e1952..d8d065d  cm-11.0    -> cm/cm-11.0
Fetching project platform/cts238), 44.01 KiB | 8.00 KiB/s   
Fetching projects:  57% (223/390)  Fetching project platform/external/scrypt
Fetching project AOSPA-legacy/android_frameworks_opt_telephony-msim
Fetching project platform/frameworks/opt/timezonepicker
Fetching project CyanogenMod/android_packages_apps_Emails   
Fetching projects:  58% (227/390)  Fetching project platform/external/chromium_org/third_party/angle_dx11
Fetching project CyanogenMod/android_external_gson0 KiB/s   
Fetching project platform/external/apache-qp | 8.00 KiB/s   
Fetching project platform/external/llvm1 KiB | 8.00 KiB/s   
Fetching projects:  59% (231/390)  Fetching project platform/external/chromium_org/third_party/skia/gyp
Fetching project platform/external/chromiumB | 6.00 KiB/s   
remote: Total 238 (delta 99), reused 125 (delta 39)
Fetching project platform/prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.6
Fetching projects:  60% (234/390)  Fetching project platform/external/jack
Fetching project platform/external/smali
Fetching project platform/frameworks/compile/slang.00 KiB/s   
Fetching project platform/external/libvpx
Fetching projects:  61% (238/390)  Fetching project platform/prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.7
Fetching project platform/external/harfbuzz_ng| 19.00 KiB/s   
Fetching project platform/external/robolectric
Fetching project platform/prebuilts/qemu-kernel
Fetching projects:  62% (242/390)  Fetching project platform/external/regex-re2
Fetching project platform/frameworks/opt/mms
Fetching project platform/external/fdlibm
Fetching project CyanogenMod/android_packages_providers_DownloadProvider
Receiving objects: 100% (238/238), 188.54 KiB | 20.00 KiB/s, done.
Fetching projects:  63% (246/390)  Fetching project platform/external/yaffs2
Fetching project platform/external/tremolo
Fetching project platform/external/objenesis
Fetching project platform/external/jmonkeyengine
Fetching projects:  64% (250/390)  Fetching project CyanogenMod/android_external_libnfc-nxp
Fetching project platform/external/oauth
Fetching project platform/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.6
Fetching project platform/external/marisa-trie
Fetching projects:  65% (254/390)  Fetching project platform/prebuilts/gcc/darwin-x86/x86/x86_64-linux-android-4.7
Fetching project repo
Fetching project platform/packages/wallpapers/NoiseField
Fetching project platform/external/jsilver
Fetching projects:  66% (258/390)  Fetching project platform/frameworks/wilhelm
Fetching project platform/external/libusb-compat
Fetching project platform/external/webp
Fetching project platform/external/genext2fs
Fetching projects:  67% (262/390)  Fetching project platform/packages/wallpapers/Basic
Fetching project platform/prebuilts/eclipse
Fetching project platform/external/droiddriver
Fetching project platform/external/mdnsresponder
Fetching projects:  68% (266/390)  Fetching project platform/prebuilts/clang/darwin-x86/mips/3.3
Fetching project platform/external/timezonepicker-support
Fetching project platform/external/android-mock
Fetching project platform/external/eclipse-windowbuilder
Fetching projects:  69% (270/390)  Fetching project platform/bootable/bootloader/legacy
Resolving deltas: 100% (99/99), done.
Fetching project AOSPA-legacy/android_packages_apps_Settings
Fetching project platform/external/jmdns
Fetching projects:  70% (273/390)  Fetching project platform/external/libffi
Fetching project CyanogenMod/ion
Fetching project platform/external/javassist
Fetching project AOSPA-legacy/android_packages_apps_BluetoothExt
Fetching projects:  71% (277/390)  Fetching project platform/external/mp4parser
Fetching project platform/external/eyes-free
remote: Counting objects: 12, done.
remote: Compressing objects: 100% (12/12), done.
remote: Total 12 (delta 2), reused 7 (delta 0)
Fetching project platform/developers/docs
Fetching project platform/external/junit
Unpacking objects: 100% (12/12), done.
Fetching projects:  72% (281/390)  Fetching project platform/packages/inputmethods/LatinIME
Fetching project platform/frameworks/ml
Fetching project platform/external/strace
Fetching project platform/external/grub
Fetching projects:  73% (285/390)  Fetching project CyanogenMod/android_external_chromium_org
Fetching project platform/packages/apps/PackageInstaller
Fetching project platform/external/expat
From https://github.com/AOSPA-legacy/android_packages_apps_Settings
   2cd3140..ab73498  kitkat     -> github/kitkat
Fetching project CyanogenMod/android_system_security
remote: Counting objects: 6, done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 0), reused 1 (delta 0)
Fetching projects:  74% (289/390)  Fetching project platform/packages/apps/Nfc
Unpacking objects: 100% (6/6), done.
Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.6
Fetching project device/generic/mini-emulator-armv7-a-neon
Fetching project platform/external/netperf
Fetching projects:  75% (293/390)  Fetching project platform/packages/apps/HTMLViewer
Fetching project platform/bootable/diskinstaller
From https://github.com/AOSPA-legacy/android_frameworks_base
   22815a6..4dd4bc7  kitkat     -> github/kitkat
Fetching project platform/packages/screensavers/PhotoTable
Fetching project platform/external/mtpd
Fetching projects:  76% (297/390)  Fetching project platform/prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.6
Fetching project platform/external/libpcap
Fetching project platform/prebuilts/gcc/linux-x86/x86/i686-linux-android-4.6
Fetching project AOSPA/android_packages_apps_Lightbulb
Fetching projects:  77% (301/390)  Fetching project platform/packages/apps/SmartCardService
Fetching project CyanogenMod/android_system_media
Fetching project platform/developers/build
Fetching project platform/external/libcap-ng
Fetching projects:  78% (305/390)  Fetching project AOSPA-legacy/android_hardware_libhardware
Fetching project platform/external/openfst
Fetching project CyanogenMod/android_external_libselinux
Fetching project platform/external/chromium_org/tools/grit
Fetching projects:  79% (309/390)  Fetching project platform/packages/wallpapers/PhaseBeam
remote: Counting objects: 32, done.
Fetching project CyanogenMod/android_packages_apps_VoicePlus
remote: Compressing objects: 100% (15/15), done.
remote: Total 32 (delta 17), reused 25 (delta 13)
Unpacking objects: 100% (32/32), done.
Fetching project platform/external/iputils
Fetching projects:  80% (312/390)  Fetching project AOSPA-legacy/android_build
Fetching project CyanogenMod/android_packages_apps_UnifiedEmail
Fetching project platform/external/markdown
Fetching project CyanogenMod/android_hardware_broadcom_libbt
From https://github.com/AOSPA/android_packages_apps_Lightbulb
   0aea23a..c6e339f  kitkat     -> github/kitkat
Fetching projects:  81% (316/390)  Fetching project platform/external/netcat
Fetching project platform/external/chromium_org/third_party/icu
Fetching project CyanogenMod/android_hardware_cm
remote: Counting objects: 5, done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 5 (delta 0), reused 0 (delta 0)
Unpacking objects: 100% (5/5), done.
Fetching project CyanogenMod/android_packages_apps_Calendar
From https://github.com/AOSPA-legacy/android_build
   588724c..c716c96  kitkat     -> github/kitkat
Fetching projects:  82% (320/390)  Fetching project platform/packages/apps/BasicSmsReceiver
Fetching project platform/external/apache-http
Fetching project platform/packages/apps/SoundRecorder
Fetching project platform/packages/wallpapers/Galaxy4
Fetching projects:  83% (324/390)  Fetching project CyanogenMod/android_external_tinyalsa
Fetching project AOSPA-legacy/android_packages_apps_Dialer
Fetching project platform/external/checkpolicy
Fetching project CyanogenMod/android_external_zlib
Fetching projects:  84% (328/390)  Fetching project platform/external/chromium-trace
Fetching project CyanogenMod/android_external_wpa_supplicant_8
Fetching project platform/abi/cpp
Fetching project platform/external/esd
Fetching projects:  85% (332/390)  Fetching project CyanogenMod/android_packages_providers_ContactsProvider
Fetching project device/sample
Fetching project platform/external/chromium_org/v8
Fetching project platform/external/ceres-solver
Fetching projects:  86% (336/390)  Fetching project platform/external/bzip2
Fetching project platform/external/jhead
Fetching project platform/packages/apps/Provision
Fetching project platform/external/littlemock
Fetching projects:  87% (340/390)  Fetching project platform/external/ppp
Fetching project platform/external/antlr
Fetching project platform/external/mockwebserver
Fetching project platform/tools/external/gradle
Fetching projects:  88% (344/390)  Fetching project CyanogenMod/android_packages_apps_Browser
Fetching project platform/external/chromium_org/sdch/open-vcdiff
Fetching project CyanogenMod/android_packages_apps_Stk
Fetching project platform/external/android-clat
Fetching projects:  89% (348/390)  Fetching project platform/external/apache-xml
Fetching project platform/external/chromium_org/third_party/eyesfree/src/android/java/src/com/googlecode/eyesfree/braille
Fetching project platform/frameworks/opt/net/voip
Fetching projects:  90% (351/390)  Fetching project platform/external/easymock
Fetching project platform/external/chromium-libpac
Fetching project platform/external/compiler-rt
Fetching project AOSPA-legacy/android_hardware_libhardware_legacy
Fetching projects:  91% (355/390)  Fetching project platform/external/srtp
Fetching project platform/packages/apps/PhoneCommon
Fetching project platform/external/mockito
Fetching project platform/external/chromium_org/third_party/smhasher/src
Fetching projects:  92% (359/390)  Fetching project platform/external/zxing
Fetching project CyanogenMod/android_development
Fetching project platform/packages/screensavers/Basic
Fetching project CyanogenMod/android_packages_apps_Calculator
Fetching projects:  93% (363/390)  Fetching project platform/external/iptables
Fetching project platform/packages/apps/Protips
Fetching project platform/prebuilts/sdk
Fetching project CyanogenMod/android_libcore
Fetching projects:  94% (367/390)  Fetching project AOSPA-legacy/android_packages_providers_TelephonyProvider
Fetching project platform/external/google-diff-match-patch
Fetching project platform/external/naver-fonts
Fetching project CyanogenMod/AndroidAsync
Fetching projects:  95% (371/390)  Fetching project platform/external/protobuf
Fetching project platform/external/bsdiff
Fetching project platform/external/chromium_org/third_party/ots
Fetching project platform/frameworks/compile/mclinker
Fetching projects:  96% (375/390)  Fetching project platform/external/xmp_toolkit
Fetching project platform/frameworks/mff
Fetching project platform/external/freetype
Fetching project platform/external/chromium_org/third_party/skia/include
Fetching projects:  97% (379/390)  Fetching project CyanogenMod/android_system_vold
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.6
Fetching project platform/external/stlport
Fetching project platform/external/dnsmasq
Fetching projects:  98% (383/390)  Fetching project platform/libnativehelper
Fetching project platform/external/tinyxml2
Fetching projects:  99% (387/390)  From git://github.com/CyanogenMod/android_external_chromium_org
   ff0a1c9..5130af6  cm-11.0    -> cm/cm-11.0
Fetching projects: 100% (390/390), done.  
Deleting obsolete path /home/hhp211/Source/AOSPA/hardware/samsung
Deleting obsolete path /home/hhp211/Source/AOSPA/packages/apps/QuickSearchBox
Syncing work tree: 100% (389/389), done.  

frameworks/opt/telephony/: discarding 1 commits
hhp211@hhp211-Q500A:~/Source/AOSPA$ cd .repo
hhp211@hhp211-Q500A:~/Source/AOSPA/.repo$ mkdir local_manifests
hhp211@hhp211-Q500A:~/Source/AOSPA/.repo$ cd ..
hhp211@hhp211-Q500A:~/Source/AOSPA$ repo sync -j6
Fetching project AOSPA-legacy/android_system_core
Fetching project platform/external/eclipse-basebuilder
Fetching project CyanogenMod/android_external_libnfc-nci
Fetching project CyanogenMod/android_dalvik
Fetching project platform/prebuilts/clang/linux-x86/x86/3.3
Fetching project CyanogenMod/android_external_libpng
Fetching project platform/external/icu4c
Fetching project platform/external/dhcpcd
Fetching project platform/external/speex
Fetching project platform/external/mdnsresponder
Fetching project TeamRegular/android_device_samsung_fascinatemtd
Fetching project platform/external/jdiff
Fetching project platform/prebuilts/runtime
Fetching project platform/external/mksh
Fetching project platform/external/linux-tools-perf
Fetching project platform/external/chromium_org/tools/gyp
Fetching project platform/developers/samples/android
Fetching project platform/packages/experimental
Fetching project platform/frameworks/opt/colorpicker
Fetching project platform/external/fsck_msdos
Fetching project platform/external/arduino
Fetching project platform/external/ipsec-tools
Fetching project AOSPA-legacy/android_frameworks_native
Fetching project platform/prebuilts/python/linux-x86/2.7.5
Fetching projects:   4% (19/390)  Fetching project platform/packages/apps/VideoEditor
Fetching projects:   5% (20/390)  Fetching project platform/packages/apps/DeskClock
Fetching project CyanogenMod/android_device_common
Fetching project platform/external/pixman
Fetching project platform/external/libphonenumber
Fetching projects:   6% (24/390)  Fetching project platform/external/nist-sip
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-eabi-4.7
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-eabi-4.6
Fetching project platform/frameworks/volley
Fetching projects:   7% (28/390)  Fetching project platform/packages/apps/SpareParts
Fetching project platform/frameworks/opt/mailcommon
Fetching project platform/prebuilts/clang/linux-x86/host/3.3
Fetching project CyanogenMod/android_external_connectivity
Fetching projects:   8% (32/390)  Fetching project device/google/accessory/arduino
Fetching project platform/external/bison
Fetching project platform/packages/providers/ApplicationsProvider
Fetching project platform/external/tinyxml
Fetching projects:   9% (36/390)  Fetching project platform/external/openssl
Fetching project platform/prebuilts/python/darwin-x86/2.7.5
Fetching project platform/prebuilts/clang/darwin-x86/arm/3.3
Fetching projects:  10% (39/390)  Fetching project platform/external/lzma
Fetching project platform/external/libxslt
Fetching project platform/packages/apps/OneTimeInitializer
Fetching project platform/packages/apps/CertInstaller
Fetching projects:  11% (43/390)  Fetching project platform/external/harfbuzz
Fetching project platform/external/ganymed-ssh2
Fetching project platform/packages/wallpapers/HoloSpiral
Fetching projects:  12% (47/390)  Fetching project platform/external/libgsm
Fetching project platform/external/open-vcdiff
Fetching project platform/prebuilts/tools
Fetching project CyanogenMod/android_external_clang
Fetching project platform/external/valgrind
Fetching projects:  13% (51/390)  Fetching project AOSPA-legacy/android_frameworks_opt_telephony
Fetching project platform/prebuilts/clang/darwin-x86/3.1
Fetching project platform/prebuilts/gcc/linux-x86/x86/i686-linux-android-4.7
Fetching project CyanogenMod/android_external_crda
Fetching projects:  14% (55/390)  Fetching project platform/external/chromium_org/third_party/yasm/source/patched-yasm
Fetching project platform/external/bzip2
Fetching project CyanogenMod/android_external_libusb
Fetching project platform/external/qemu-pc-bios
Fetching projects:  15% (59/390)  Fetching project platform/prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.7
Fetching project device/generic/armv7-a-neon
Fetching project platform/frameworks/ex
Fetching project platform/external/chromium_org/third_party/leveldatabase/src
Fetching projects:  16% (63/390)  Fetching project platform/prebuilts/clang/darwin-x86/3.2
Fetching project CyanogenMod/android_packages_providers_MediaProvider
Fetching project device/generic/common
Fetching project platform/prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.7-4.6
Fetching projects:  17% (67/390)  Fetching project CyanogenMod/android_frameworks_webview
Fetching project platform/external/gtest
Fetching project CyanogenMod/android_packages_apps_Contacts
Fetching project CyanogenMod/android_prebuilts_misc
Fetching projects:  18% (71/390)  Fetching project platform/external/neven
Fetching project platform/frameworks/opt/carddav
Fetching project platform/external/liblzf
Fetching project platform/external/hyphenation
Fetching projects:  19% (75/390)  Fetching project platform/prebuilts/gcc/darwin-x86/x86/i686-linux-android-4.7
Fetching project platform/external/doclava
Fetching project AOSPA-legacy/android_external_bluetooth_bluedroid
Fetching projects:  20% (78/390)  Fetching project platform/external/eigen
Fetching project platform/external/guava
Fetching project device/generic/mini-emulator-mips
Fetching project platform/external/nist-pkits
Fetching projects:  21% (82/390)  Fetching project platform/packages/providers/CalendarProvider
Fetching project device/generic/x86
Fetching project platform/external/iproute2
Fetching project platform/external/chromium_org/third_party/WebKit
Fetching projects:  22% (86/390)  Fetching project platform/packages/wallpapers/MagicSmoke
Fetching project platform/external/openssh
Fetching project platform/packages/screensavers/WebView
Fetching project AOSPA-legacy/android_packages_apps_Mms
Fetching projects:  23% (90/390)  Fetching project platform/prebuilts/ndk
Fetching project platform/external/bouncycastle
Fetching project platform/external/libogg
Fetching project CyanogenMod/android_packages_apps_ContactsCommon
Fetching projects:  24% (94/390)  Fetching project platform/external/dropbear
Fetching project platform/external/gcc-demangle
Fetching project platform/prebuilts/gcc/darwin-x86/host/i686-apple-darwin-4.2.1
Fetching project CyanogenMod/android_external_qrngd
Fetching projects:  25% (98/390)  Fetching project AOSPA-legacy/android_packages_apps_ScreenRecorder
Fetching project AOSPA-legacy/android_frameworks_av
Fetching project CyanogenMod/android_frameworks_opt_vcard
Fetching project platform/packages/providers/PartnerBookmarksProvider
Fetching projects:  26% (102/390)  Fetching project CyanogenMod/android_system_qcom
Fetching project device/generic/mini-emulator-x86
Fetching project platform/external/embunit
Fetching project platform/prebuilts/clang/linux-x86/3.2
Fetching projects:  27% (106/390)  Fetching project CyanogenMod/android_external_skia
Fetching project platform/external/chromium_org/third_party/libphonenumber/src/resources
Fetching project platform/external/dexmaker
Fetching project platform/external/mesa3d
Fetching projects:  28% (110/390)  Fetching project platform/prebuilts/gcc/linux-x86/x86/x86_64-linux-android-4.7
Fetching project platform/external/noto-fonts
Fetching project platform/external/chromium_org/third_party/libphonenumber/src/phonenumbers
Fetching project platform/external/libyuv
Fetching projects:  29% (114/390)  Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.7
Fetching project platform/external/tinycompress
Fetching project CyanogenMod/android_system_netd
Fetching projects:  30% (117/390)  Fetching project platform/pdk
remote: Counting objects: 18, done.
remote: Compressing objects: 100% (18/18), done.
Fetching project CyanogenMod/android_system_extras
Fetching project AOSPA-legacy/android_packages_apps_InCallUI
Fetching project platform/external/v8
Fetching projects:  31% (121/390)  Fetching project platform/external/xmlwriter
Fetching project platform/external/libxml2
remote: Total 18 (delta 8), reused 0 (delta 0)
Fetching project device/generic/mips
Fetching project platform/external/javasqlite
Fetching projects:  32% (125/390)  Fetching project platform/external/smack
Unpacking objects: 100% (18/18), done.
Fetching project platform/frameworks/opt/datetimepicker
Fetching project platform/frameworks/compile/libbcc
Fetching project platform/external/safe-iop
Fetching projects:  33% (129/390)  Fetching project platform/ndk
Fetching project platform/tools/external/fat32lib
Fetching project CyanogenMod/android_external_sepolicy
Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-eabi-4.7
Fetching projects:  34% (133/390)  Fetching project platform/external/sil-fonts
Fetching project platform/packages/wallpapers/LivePicker
Fetching project platform/external/qemu
Fetching project platform/external/kernel-headers
Fetching projects:  35% (137/390)  Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-eabi-4.6
Fetching project platform/packages/apps/VoiceDialer
Fetching project platform/external/sfntly
Fetching project platform/frameworks/opt/photoviewer
Fetching projects:  36% (141/390)  Fetching project platform/external/libffi
Fetching project CyanogenMod/android_frameworks_support
Fetching project platform/external/hamcrest
Fetching project platform/frameworks/testing
Fetching projects:  37% (145/390)  Fetching project platform/packages/apps/SpeechRecorder
Fetching project platform/external/okhttp
Fetching project platform/external/chromium_org/sdch/open-vcdiff
Fetching project platform/frameworks/opt/emoji
Fetching projects:  38% (149/390)  Fetching project platform/prebuilts/gcc/darwin-x86/host/headers
From https://github.com/TeamRegular/android_device_samsung_fascinatemtd
 * [new branch]      kitkat     -> github/kitkat
Fetching project platform/external/chromium_org/testing/gtest
Fetching project CyanogenMod/android_packages_apps_Gallery2
Fetching project CyanogenMod/android_bionic
Fetching projects:  39% (153/390)  Fetching project platform/external/chromium_org/third_party/openssl
Fetching project CyanogenMod/android_external_flac
Fetching project AOSPA-legacy/android_packages_services_Telephony
Fetching projects:  40% (156/390)  Fetching project platform/prebuilts/devtools
Fetching project platform/prebuilts/clang/linux-x86/arm/3.3
Fetching project platform/packages/wallpapers/MusicVisualization
Fetching project platform/external/libnl-headers
Fetching projects:  41% (160/390)  Fetching project platform/external/opencv
Fetching project platform/external/emma
Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.7
Fetching project platform/external/chromium_org/third_party/skia/src
Fetching projects:  42% (164/390)  Fetching project platform/external/libppp
Fetching project platform/packages/apps/CellBroadcastReceiver
Fetching project platform/frameworks/opt/inputmethodcommon
Fetching project platform/prebuilts/clang/linux-x86/3.1
Fetching projects:  43% (168/390)  Fetching project AOSPA-legacy/android_art
Fetching project platform/external/libvorbis
Fetching project platform/packages/apps/KeyChain
Fetching project platform/external/tagsoup
Fetching projects:  44% (172/390)  Fetching project AOSPA-legacy/android_packages_apps_Bluetooth
Fetching project CyanogenMod/Widgets
Fetching project platform/external/sqlite
Fetching project CyanogenMod/android_external_busybox
Fetching projects:  45% (176/390)  Fetching project CyanogenMod/android_external_e2fsprogs
Fetching project platform/external/oprofile
Fetching project platform/external/jpeg
Fetching project platform/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.4.3
Fetching projects:  46% (180/390)  Fetching project platform/external/elfutils
Fetching project platform/prebuilts/clang/darwin-x86/x86/3.3
Fetching project AOSPA-legacy/android_frameworks_base
Fetching project platform/external/libmtp
Fetching projects:  47% (184/390)  Fetching project platform/external/ant-glob
Fetching project platform/external/jsr305
Fetching project CyanogenMod/android_frameworks_opt_hardware
Fetching project platform/external/srec
Fetching projects:  48% (188/390)  Fetching project platform/packages/apps/Tag
Fetching project platform/external/apache-harmony
Fetching project platform/frameworks/opt/calendar
Fetching project CyanogenMod/android_packages_apps_Exchange
Fetching projects:  49% (192/390)  Fetching project CyanogenMod/android_frameworks_rs
Fetching project platform/external/stressapptest
Fetching project platform/external/webrtc
Fetching projects:  50% (195/390)  Fetching project platform/external/chromium_org/third_party/freetype
Fetching project platform/external/aac
Fetching project platform/external/proguard
Fetching project platform/frameworks/uiautomator
Fetching projects:  51% (199/390)  Fetching project AOSPA-legacy/manifest
Fetching project platform/external/tcpdump
Fetching project platform/bootable/recovery
Fetching project platform/external/chromium_org/third_party/mesa/src
Fetching projects:  52% (203/390)  Fetching project platform/external/chromium_org/third_party/opus/src
Fetching project CyanogenMod/android_packages_apps_Camera2
Fetching project platform/prebuilts/clang/linux-x86/mips/3.3
Fetching project AOSPA-legacy/android_vendor_pa
Fetching projects:  53% (207/390)  Fetching project platform/prebuilts/gcc/darwin-x86/x86/i686-linux-android-4.6
Fetching project CyanogenMod/android_external_libsepol
Fetching project platform/external/replicaisland
Fetching project device/google/accessory/demokit
Fetching projects:  54% (211/390)  Fetching project platform/packages/providers/UserDictionaryProvider
Fetching project CyanogenMod/android_packages_apps_Launcher3
Fetching project platform/external/giflib
Fetching project AOSPA-legacy/android_packages_apps_ParanoidOTA
Fetching projects:  55% (215/390)  Fetching project platform/external/chromium_org/third_party/libjingle/source/talk
Fetching project platform/prebuilts/clang/darwin-x86/host/3.3
Fetching project CyanogenMod/android_hardware_broadcom_wlan
Fetching project CyanogenMod/android_hardware_ril
Fetching projects:  56% (219/390)  Fetching project platform/packages/inputmethods/OpenWnn
Fetching project platform/sdk
Fetching project platform/external/sonivox
Fetching project platform/packages/apps/MusicFX
Fetching projects:  57% (223/390)  Fetching project platform/cts
Fetching project platform/external/scrypt
Fetching project AOSPA-legacy/android_frameworks_opt_telephony-msim
Fetching project platform/frameworks/opt/timezonepicker
Fetching projects:  58% (227/390)  Fetching project CyanogenMod/android_packages_apps_Email
Fetching project platform/external/chromium_org/third_party/angle_dx11
Fetching project CyanogenMod/android_external_gson
Fetching project platform/external/apache-qp
Fetching projects:  59% (231/390)  Fetching project platform/external/llvm
Fetching project platform/external/chromium_org/third_party/skia/gyp
Fetching project platform/external/chromium
Fetching projects:  60% (234/390)  Fetching project platform/prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.6
Fetching project platform/external/jack
Fetching project platform/external/compiler-rt
Fetching project platform/frameworks/compile/slang
Fetching projects:  61% (238/390)  Fetching project platform/external/libvpx
Fetching project platform/prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.7
Fetching project platform/external/harfbuzz_ng
Fetching project platform/external/robolectric
Fetching projects:  62% (242/390)  Fetching project platform/prebuilts/qemu-kernel
Fetching project platform/external/regex-re2
Fetching project platform/frameworks/opt/mms
Fetching project platform/external/fdlibm
Fetching projects:  63% (246/390)  Fetching project CyanogenMod/android_packages_providers_DownloadProvider
Fetching project platform/external/yaffs2
Fetching project platform/external/tremolo
Fetching project platform/external/objenesis
Fetching projects:  64% (250/390)  Fetching project platform/external/jmonkeyengine
Fetching project CyanogenMod/android_external_libnfc-nxp
Fetching project platform/external/oauth
Fetching project platform/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.6
Fetching projects:  65% (254/390)  Fetching project platform/external/marisa-trie
Fetching project platform/prebuilts/gcc/darwin-x86/x86/x86_64-linux-android-4.7
Fetching project platform/packages/wallpapers/NoiseField
Fetching project platform/external/jsilver
Fetching projects:  66% (258/390)  Fetching project platform/frameworks/wilhelm
Fetching project platform/external/libusb-compat
Fetching project platform/external/webp
Fetching project platform/external/genext2fs
Fetching projects:  67% (262/390)  Fetching project platform/packages/wallpapers/Basic
Fetching project platform/prebuilts/eclipse
Fetching project platform/external/droiddriver
Fetching project platform/prebuilts/clang/darwin-x86/mips/3.3
Fetching projects:  68% (266/390)  Fetching project platform/external/timezonepicker-support
Fetching project platform/external/android-mock
Fetching project platform/external/eclipse-windowbuilder
Fetching project platform/bootable/bootloader/legacy
Fetching projects:  69% (270/390)  Fetching project AOSPA-legacy/android_packages_apps_Settings
Fetching project platform/external/jmdns
Fetching project device/generic/goldfish
Fetching projects:  70% (273/390)  Fetching project CyanogenMod/ion
Fetching project platform/external/javassist
Fetching project AOSPA-legacy/android_packages_apps_BluetoothExt
Fetching project platform/external/mp4parser
Fetching projects:  71% (277/390)  Fetching project platform/external/eyes-free
Fetching project platform/developers/docs
Fetching project platform/external/junit
Fetching project platform/packages/inputmethods/LatinIME
Fetching projects:  72% (281/390)  Fetching project platform/frameworks/ml
Fetching project platform/external/strace
Fetching project platform/external/grub
Fetching project CyanogenMod/android_external_chromium_org
Fetching projects:  73% (285/390)  Fetching project platform/packages/apps/PackageInstaller
Fetching project platform/external/expat
Fetching project CyanogenMod/android_system_security
Fetching project platform/packages/apps/Nfc
Fetching projects:  74% (289/390)  Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.6
Fetching project device/generic/mini-emulator-armv7-a-neon
Fetching project platform/external/netperf
Fetching project platform/packages/apps/HTMLViewer
Fetching projects:  75% (293/390)  Fetching project platform/bootable/diskinstaller
Fetching project platform/packages/screensavers/PhotoTable
Fetching project platform/external/mtpd
Fetching project platform/prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.6
Fetching projects:  76% (297/390)  Fetching project platform/external/libpcap
Fetching project platform/prebuilts/gcc/linux-x86/x86/i686-linux-android-4.6
Fetching project AOSPA/android_packages_apps_Lightbulb
Fetching project platform/packages/apps/SmartCardService
Fetching projects:  77% (301/390)  Fetching project CyanogenMod/android_system_media
Fetching project platform/developers/build
Fetching project platform/external/libcap-ng
Fetching project AOSPA-legacy/android_hardware_libhardware
Fetching projects:  78% (305/390)  Fetching project platform/external/openfst
Fetching project CyanogenMod/android_external_libselinux
Fetching project platform/external/chromium_org/tools/grit
Fetching project platform/packages/wallpapers/PhaseBeam
Fetching projects:  79% (309/390)  Fetching project CyanogenMod/android_packages_apps_VoicePlus
Fetching project platform/external/iputils
Fetching project AOSPA-legacy/android_build
Fetching projects:  80% (312/390)  Fetching project CyanogenMod/android_packages_apps_UnifiedEmail
Fetching project platform/external/markdown
Fetching project CyanogenMod/android_hardware_broadcom_libbt
Fetching project platform/external/netcat
Fetching projects:  81% (316/390)  Fetching project platform/external/chromium_org/third_party/icu
Fetching project CyanogenMod/android_hardware_cm
Fetching project CyanogenMod/android_packages_apps_Calendar
Fetching project platform/packages/apps/BasicSmsReceiver
Fetching projects:  82% (320/390)  Fetching project platform/external/apache-http
Fetching project platform/packages/apps/SoundRecorder
Fetching project platform/packages/wallpapers/Galaxy4
Fetching project CyanogenMod/android_external_tinyalsa
Fetching projects:  83% (324/390)  Fetching project AOSPA-legacy/android_packages_apps_Dialer
Fetching project platform/external/checkpolicy
Fetching project CyanogenMod/android_external_zlib
Fetching project platform/external/chromium-trace
Fetching projects:  84% (328/390)  Fetching project CyanogenMod/android_external_wpa_supplicant_8
Fetching project platform/abi/cpp
Fetching project platform/external/esd
Fetching project CyanogenMod/android_packages_providers_ContactsProvider
Fetching projects:  85% (332/390)  Fetching project device/sample
Fetching project platform/external/chromium_org/v8
Fetching project platform/external/ceres-solver
Fetching project platform/external/blktrace
Fetching projects:  86% (336/390)  Fetching project platform/external/jhead
Fetching project platform/packages/apps/Provision
Fetching project platform/external/littlemock
Fetching project platform/external/ppp
Fetching projects:  87% (340/390)  Fetching project platform/external/antlr
Fetching project platform/external/mockwebserver
Fetching project platform/tools/external/gradle
Fetching project CyanogenMod/android_packages_apps_Browser
Fetching projects:  88% (344/390)  Fetching project platform/developers/demos
Fetching project platform/docs/source.android.com
Fetching project CyanogenMod/android_packages_apps_Stk
Fetching project platform/external/android-clat
Fetching projects:  89% (348/390)  Fetching project platform/external/apache-xml
Fetching project platform/external/chromium_org/third_party/eyesfree/src/android/java/src/com/googlecode/eyesfree/braille
Fetching project platform/frameworks/opt/net/voip
Fetching projects:  90% (351/390)  Fetching project platform/external/easymock
Fetching project platform/external/chromium-libpac
Fetching project platform/external/smali
Fetching project AOSPA-legacy/android_hardware_libhardware_legacy
Fetching projects:  91% (355/390)  Fetching project platform/external/srtp
Fetching project platform/packages/apps/PhoneCommon
Fetching project platform/external/mockito
Fetching project platform/external/chromium_org/third_party/smhasher/src
Fetching projects:  92% (359/390)  Fetching project platform/external/zxing
Fetching project CyanogenMod/android_development
Fetching project platform/packages/screensavers/Basic
Fetching project CyanogenMod/android_packages_apps_Calculator
Fetching projects:  93% (363/390)  Fetching project platform/external/iptables
Fetching project platform/packages/apps/Protips
Fetching project platform/prebuilts/sdk
Fetching project CyanogenMod/android_libcore
Fetching projects:  94% (367/390)  Fetching project AOSPA-legacy/android_packages_providers_TelephonyProvider
Fetching project platform/external/google-diff-match-patch
Fetching project platform/external/naver-fonts
Fetching project CyanogenMod/AndroidAsync
Fetching projects:  95% (371/390)  Fetching project platform/external/protobuf
Fetching project platform/external/bsdiff
Fetching project platform/external/chromium_org/third_party/ots
Fetching project platform/frameworks/compile/mclinker
Fetching projects:  96% (375/390)  Fetching project platform/external/xmp_toolkit
Fetching project platform/frameworks/mff
Fetching project platform/external/freetype
Fetching project platform/external/chromium_org/third_party/skia/include
Fetching projects:  97% (379/390)  Fetching project CyanogenMod/android_system_vold
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.6
Fetching project platform/external/stlport
Fetching project platform/external/dnsmasq
Fetching projects:  98% (383/390)  Fetching project platform/libnativehelper
Fetching project platform/external/tinyxml2
Fetching projects: 100% (390/390), done.  
Syncing work tree: 100% (390/390), done.  




hhp211@hhp211-Q500A:~/Source/AOSPA$ . build/envsetup.sh
including device/generic/armv7-a-neon/vendorsetup.sh
including device/generic/mips/vendorsetup.sh
including device/generic/x86/vendorsetup.sh
including vendor/pa/vendorsetup.sh
including sdk/bash_completion/adb.bash
hhp211@hhp211-Q500A:~/Source/AOSPA$ lunch

You're building on Linux

Lunch menu... pick a combo:
     1. mini_armv7a_neon-userdebug
     2. mini_mips-userdebug
     3. mini_x86-userdebug
     4. pa_d2lte-userdebug
     5. pa_d800-userdebug
     6. pa_d801-userdebug
     7. pa_d802-userdebug
     8. pa_d803-userdebug
     9. pa_dlx-userdebug
     10. pa_galaxysmtd-userdebug
     11. pa_gee-userdebug
     12. pa_geeb-userdebug
     13. pa_hercules-userdebug
     14. pa_hlte-userdebug
     15. pa_i605-userdebug
     16. pa_i9300-userdebug
     17. pa_i9500-userdebug
     18. pa_jflte-userdebug
     19. pa_l900-userdebug
     20. pa_ls980-userdebug
     21. pa_m7-userdebug
     22. pa_moto_msm8960-userdebug
     23. pa_moto_msm8960dt-userdebug
     24. pa_n7000-userdebug
     25. pa_n7100-userdebug
     26. pa_p880-userdebug
     27. pa_skyrocket-userdebug
     28. pa_togari-userdebug
     29. pa_v500-userdebug
     30. pa_vs980-userdebug
     31. pa_yuga-userdebug

Which would you like? [aosp_arm-eng] 
you device can't be found in device sources..
Traceback (most recent call last):
  File "build/tools/roomservice.py", line 295, in <module>
    fetch_dependencies(device)
  File "build/tools/roomservice.py", line 248, in fetch_dependencies
    raise Exception("ERROR: could not find your device "
Exception: ERROR: could not find your device folder location, bailing out

** Don't have a product spec for: 'aosp_arm'
** Do you have the right repo manifest?


hhp211@hhp211-Q500A:~/Source/AOSPA$ make pa_fascinatemtd-userdeug

============================================
PLATFORM_VERSION_CODENAME=REL
PLATFORM_VERSION=4.4.2
TARGET_PRODUCT=full
TARGET_BUILD_VARIANT=eng
TARGET_BUILD_TYPE=release
TARGET_BUILD_APPS=
TARGET_ARCH=arm
TARGET_ARCH_VARIANT=armv7-a
TARGET_CPU_VARIANT=generic
HOST_ARCH=x86
HOST_OS=linux
HOST_OS_EXTRA=Linux-3.14.0-031400rc1-generic-x86_64-with-Ubuntu-12.04-precise
HOST_BUILD_TYPE=release
BUILD_ID=KVT49L
OUT_DIR=/home/hhp211/Source/AOSPA/out
============================================
Checking build tools versions...
/home/hhp211/Source/AOSPA/out/target/product/generic/obj/APPS/SignatureTest_intermediates
find: `src': No such file or directory
build/core/tasks/kernel.mk:91: **********************************************************
build/core/tasks/kernel.mk:92: * Kernel source found, but no configuration was defined  *
build/core/tasks/kernel.mk:93: * Please add the TARGET_KERNEL_CONFIG variable to your   *
build/core/tasks/kernel.mk:94: * BoardConfig.mk file                                    *
build/core/tasks/kernel.mk:95: **********************************************************
make: *** No rule to make target `pa_fascinatemtd-userdeug'.  Stop.


hhp211@hhp211-Q500A:~/Source/AOSPA$ make pa_fascinatemtd-userdebug


============================================
PLATFORM_VERSION_CODENAME=REL
PLATFORM_VERSION=4.4.2
TARGET_PRODUCT=full
TARGET_BUILD_VARIANT=eng
TARGET_BUILD_TYPE=release
TARGET_BUILD_APPS=
TARGET_ARCH=arm
TARGET_ARCH_VARIANT=armv7-a
TARGET_CPU_VARIANT=generic
HOST_ARCH=x86
HOST_OS=linux
HOST_OS_EXTRA=Linux-3.14.0-031400rc1-generic-x86_64-with-Ubuntu-12.04-precise
HOST_BUILD_TYPE=release
BUILD_ID=KVT49L
OUT_DIR=/home/hhp211/Source/AOSPA/out
============================================
/home/hhp211/Source/AOSPA/out/target/product/generic/obj/APPS/SignatureTest_intermediates
find: `src': No such file or directory
build/core/tasks/kernel.mk:91: **********************************************************
build/core/tasks/kernel.mk:92: * Kernel source found, but no configuration was defined  *
build/core/tasks/kernel.mk:93: * Please add the TARGET_KERNEL_CONFIG variable to your   *
build/core/tasks/kernel.mk:94: * BoardConfig.mk file                                    *
build/core/tasks/kernel.mk:95: **********************************************************
make: *** No rule to make target `pa_fascinatemtd-userdebug'.  Stop.


hhp211@hhp211-Q500A:~/Source/AOSPA$ . build/envsetup.sh
including device/generic/armv7-a-neon/vendorsetup.sh
including device/generic/mips/vendorsetup.sh
including device/generic/x86/vendorsetup.sh
including vendor/pa/vendorsetup.sh
including sdk/bash_completion/adb.bash

hhp211@hhp211-Q500A:~/Source/AOSPA$ lunch

You're building on Linux

Lunch menu... pick a combo:
     1. mini_armv7a_neon-userdebug
     2. mini_mips-userdebug
     3. mini_x86-userdebug
     4. pa_d2lte-userdebug
     5. pa_d800-userdebug
     6. pa_d801-userdebug
     7. pa_d802-userdebug
     8. pa_d803-userdebug
     9. pa_dlx-userdebug
     10. pa_fascinatemtd-userdebug
     11. pa_galaxysmtd-userdebug
     12. pa_gee-userdebug
     13. pa_geeb-userdebug
     14. pa_hercules-userdebug
     15. pa_hlte-userdebug
     16. pa_i605-userdebug
     17. pa_i9300-userdebug
     18. pa_i9500-userdebug
     19. pa_jflte-userdebug
     20. pa_l900-userdebug
     21. pa_ls980-userdebug
     22. pa_m7-userdebug
     23. pa_moto_msm8960-userdebug
     24. pa_moto_msm8960dt-userdebug
     25. pa_n7000-userdebug
     26. pa_n7100-userdebug
     27. pa_p880-userdebug
     28. pa_skyrocket-userdebug
     29. pa_togari-userdebug
     30. pa_v500-userdebug
     31. pa_vs980-userdebug
     32. pa_yuga-userdebug

Which would you like? [aosp_arm-eng] 10
build/core/product_config.mk:227: *** _nic.PRODUCTS.[[vendor/pa/products/pa_fascinatemtd.mk]]: "vendor/samsung/fascinatemtd/fascinatemtd-vendor.mk" does not exist.  Stop.
WARNING: Trying to fetch a device that's already there
wrote the new roomservice manifest
wrote the new roomservice manifest
wrote the new roomservice manifest
wrote the new roomservice manifest
wrote the new roomservice manifest
wrote the new roomservice manifest
fatal: duplicate path bootable/recovery in /home/hhp211/Source/AOSPA/.repo/manifest.xml
build/core/product_config.mk:227: *** _nic.PRODUCTS.[[vendor/pa/products/pa_fascinatemtd.mk]]: "vendor/samsung/fascinatemtd/fascinatemtd-vendor.mk" does not exist.  Stop.

** Don't have a product spec for: 'pa_fascinatemtd'
** Do you have the right repo manifest?



hhp211@hhp211-Q500A:~/Source/AOSPA$ make pa_fascinatemtd-userdebug


============================================
PLATFORM_VERSION_CODENAME=REL
PLATFORM_VERSION=4.4.2
TARGET_PRODUCT=full
TARGET_BUILD_VARIANT=eng
TARGET_BUILD_TYPE=release
TARGET_BUILD_APPS=
TARGET_ARCH=arm
TARGET_ARCH_VARIANT=armv7-a
TARGET_CPU_VARIANT=generic
HOST_ARCH=x86
HOST_OS=linux
HOST_OS_EXTRA=Linux-3.14.0-031400rc1-generic-x86_64-with-Ubuntu-12.04-precise
HOST_BUILD_TYPE=release
BUILD_ID=KVT49L
OUT_DIR=/home/hhp211/Source/AOSPA/out
============================================
/home/hhp211/Source/AOSPA/out/target/product/generic/obj/APPS/SignatureTest_intermediates
find: `src': No such file or directory
build/core/tasks/kernel.mk:91: **********************************************************
build/core/tasks/kernel.mk:92: * Kernel source found, but no configuration was defined  *
build/core/tasks/kernel.mk:93: * Please add the TARGET_KERNEL_CONFIG variable to your   *
build/core/tasks/kernel.mk:94: * BoardConfig.mk file                                    *
build/core/tasks/kernel.mk:95: **********************************************************
make: *** No rule to make target `pa_fascinatemtd-userdebug'.  Stop.



hhp211@hhp211-Q500A:~/Source/AOSPA$ repo sync -j6
fatal: duplicate path bootable/recovery in /home/hhp211/Source/AOSPA/.repo/manifest.xml

hhp211@hhp211-Q500A:~/Source/AOSPA$ repo sync -j6
Fetching project AOSPA-legacy/android_system_core
Fetching project platform/external/eclipse-basebuilder
Fetching project platform/tools/external/fat32lib
Fetching project CyanogenMod/android_dalvik
Fetching project platform/prebuilts/clang/linux-x86/x86/3.3
Fetching project CyanogenMod/android_external_libpng
Fetching project platform/external/icu4c
Fetching project platform/external/dhcpcd
Fetching project CyanogenMod/android_hardware_samsung
Fetching project platform/external/speex
Fetching project platform/external/mdnsresponder
Fetching project TeamRegular/android_device_samsung_fascinatemtd
Fetching project platform/external/jdiff
Fetching project platform/prebuilts/runtime
Fetching project platform/external/mksh
Fetching project platform/external/linux-tools-perf
Fetching project platform/external/chromium_org/tools/gyp
Fetching project platform/developers/samples/android
Fetching project platform/packages/experimental
Fetching project platform/frameworks/opt/colorpicker
Fetching project platform/external/fsck_msdos
Fetching project platform/external/arduino
Fetching project platform/external/ipsec-tools
Fetching project AOSPA-legacy/android_frameworks_native
Fetching project platform/prebuilts/python/linux-x86/2.7.5
Fetching project platform/packages/apps/VideoEditor
Fetching project platform/packages/apps/DeskClock
Fetching project CyanogenMod/android_device_common
Fetching project platform/external/pixman
Fetching project platform/external/libphonenumber
Fetching project platform/external/nist-sip
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-eabi-4.7
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-eabi-4.6
Fetching project platform/frameworks/volley
Fetching project platform/packages/apps/SpareParts
Fetching project platform/frameworks/opt/mailcommon
Fetching project platform/prebuilts/clang/linux-x86/host/3.3
Fetching project CyanogenMod/android_external_connectivity
Fetching project device/google/accessory/arduino
Fetching project platform/external/bison
Fetching project platform/packages/providers/ApplicationsProvider
Fetching project platform/external/tinyxml
Fetching project platform/external/openssl
Fetching project platform/prebuilts/python/darwin-x86/2.7.5
Fetching projects:   9% (39/395)  Fetching project platform/prebuilts/clang/darwin-x86/arm/3.3
Fetching projects:  10% (40/395)  Fetching project platform/external/lzma
Fetching project AOSPA-legacy/android_device_samsung_aries-common
Fetching project platform/external/libxslt
Fetching project platform/packages/apps/OneTimeInitializer
Fetching projects:  11% (44/395)  Fetching project platform/packages/apps/CertInstaller
Fetching project platform/external/harfbuzz
Fetching project platform/external/ganymed-ssh2
Fetching project platform/packages/wallpapers/HoloSpiral
Fetching projects:  12% (48/395)  Fetching project platform/external/libgsm
Fetching project platform/external/open-vcdiff
Fetching project platform/prebuilts/tools
Fetching project CyanogenMod/android_external_clang
Fetching projects:  13% (52/395)  Fetching project platform/external/valgrind
Fetching project AOSPA-legacy/android_frameworks_opt_telephony
Fetching project platform/prebuilts/clang/darwin-x86/3.1
Fetching project platform/prebuilts/gcc/linux-x86/x86/i686-linux-android-4.7
Fetching projects:  14% (56/395)  Fetching project CyanogenMod/android_external_crda
Fetching project platform/external/chromium_org/third_party/yasm/source/patched-yasm
Fetching project platform/external/bzip2
Fetching project CyanogenMod/android_external_libusb
Fetching projects:  15% (60/395)  Fetching project platform/external/qemu-pc-bios
Fetching project platform/prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.7
Fetching project device/generic/armv7-a-neon
Fetching project platform/frameworks/ex
Fetching projects:  16% (64/395)  Fetching project platform/external/chromium_org/third_party/leveldatabase/src
Fetching project platform/prebuilts/clang/darwin-x86/3.2
Fetching project CyanogenMod/android_packages_providers_MediaProvider
Fetching project device/generic/common
Fetching projects:  17% (68/395)  Fetching project platform/prebuilts/gcc/linux-x86/host/x86_64-linux-glibc2.7-4.6
Fetching project CyanogenMod/android_frameworks_webview
Fetching project platform/external/gtest
Fetching project CyanogenMod/android_packages_apps_Contacts
Fetching projects:  18% (72/395)  Fetching project CyanogenMod/android_prebuilts_misc
Fetching project platform/external/neven
Fetching project platform/frameworks/opt/carddav
Fetching project platform/external/liblzf
Fetching projects:  19% (76/395)  Fetching project platform/external/hyphenation
Fetching project omnirom/android_bootable_recovery
Fetching project platform/prebuilts/gcc/darwin-x86/x86/i686-linux-android-4.7
remote: Counting objects: 76, done.
remote: Compressing objects: 100% (54/54), done.
Fetching projects:  20% (79/395)  Fetching project platform/external/doclava
Fetching project AOSPA-legacy/android_external_bluetooth_bluedroid
remote: Total 76 (delta 26), reused 60 (delta 19)
Unpacking objects: 100% (76/76), done.
Fetching project platform/external/eigen
Fetching project platform/external/guava
Fetching projects:  21% (83/395)  Fetching project device/generic/mini-emulator-mips
Fetching project platform/external/nist-pkits
From https://github.com/CyanogenMod/android_hardware_samsung
 * [new branch]      cm-11.0    -> github/cm-11.0
 * [new tag]         cm-10.1-M1 -> cm-10.1-M1
 * [new tag]         cm-10.1-M2 -> cm-10.1-M2
 * [new tag]         cm-10.1-M3 -> cm-10.1-M3
 * [new tag]         cm-10.1.0  -> cm-10.1.0
 * [new tag]         cm-10.1.0-RC1 -> cm-10.1.0-RC1
 * [new tag]         cm-10.1.0-RC2 -> cm-10.1.0-RC2
 * [new tag]         cm-10.1.0-RC3 -> cm-10.1.0-RC3
Fetching project platform/packages/providers/CalendarProvider
 * [new tag]         cm-10.1.0-RC4 -> cm-10.1.0-RC4
 * [new tag]         cm-10.1.0-RC5 -> cm-10.1.0-RC5
 * [new tag]         cm-10.1.0.1 -> cm-10.1.0.1
 * [new tag]         cm-10.1.3-RC1 -> cm-10.1.3-RC1
 * [new tag]         cm-10.1.3-RC2 -> cm-10.1.3-RC2
Fetching project device/generic/x86
Fetching projects:  22% (87/395)  Fetching project platform/external/iproute2
Fetching project platform/external/chromium_org/third_party/WebKit
 * [new tag]         cm-10.2-M1 -> cm-10.2-M1
Fetching project platform/packages/wallpapers/MagicSmoke
Fetching project platform/external/openssh
Fetching projects:  23% (91/395)  Fetching project platform/packages/screensavers/WebView
Fetching project AOSPA-legacy/android_packages_apps_Mms
Fetching project platform/prebuilts/ndk
Fetching project platform/external/bouncycastle
Fetching projects:  24% (95/395)  Fetching project platform/external/libogg
Fetching project CyanogenMod/android_packages_apps_ContactsCommon
Fetching project platform/external/dropbear
Fetching project platform/external/gcc-demangle
Fetching projects:  25% (99/395)  Fetching project platform/prebuilts/gcc/darwin-x86/host/i686-apple-darwin-4.2.1
Fetching project CyanogenMod/android_external_qrngd
Fetching project AOSPA-legacy/android_packages_apps_ScreenRecorder
Fetching project AOSPA-legacy/android_frameworks_av
Fetching projects:  26% (103/395)  Fetching project CyanogenMod/android_frameworks_opt_vcard
remote: Counting objects: 80, done.
remote: Compressing objects: 100% (51/51), done.
remote: Total 80 (delta 15), reused 69 (delta 11)
Unpacking objects: 100% (80/80), done.
Fetching project platform/packages/providers/PartnerBookmarksProvider
Fetching project CyanogenMod/android_system_qcom
Fetching project device/generic/mini-emulator-x86
From https://github.com/AOSPA-legacy/android_device_samsung_aries-common
 * [new branch]      kitkat     -> github/kitkat
Fetching projects:  27% (107/395)  Fetching project platform/external/embunit
Fetching project platform/prebuilts/clang/linux-x86/3.2
Fetching project CyanogenMod/android_external_skia
Fetching project platform/external/chromium_org/third_party/libphonenumber/src/resources
Fetching projects:  28% (111/395)  Fetching project platform/external/dexmaker
Fetching project platform/external/mesa3d
Fetching project platform/prebuilts/gcc/linux-x86/x86/x86_64-linux-android-4.7
Fetching project platform/external/noto-fonts
Fetching projects:  29% (115/395)  Fetching project platform/external/chromium_org/third_party/libphonenumber/src/phonenumbers
Fetching project platform/external/libyuv
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.7
Fetching project CyanogenMod/android_packages_apps_Apollo
Fetching projects:  30% (119/395)  Fetching project platform/external/tinycompress
Fetching project CyanogenMod/android_system_netd
Fetching project platform/pdk
Fetching project CyanogenMod/android_system_extras
Fetching projects:  31% (123/395)  Fetching project AOSPA-legacy/android_packages_apps_InCallUI
Fetching project platform/external/v8
Fetching project platform/external/xmlwriter
Fetching project platform/external/libxml2
remote: Counting objects: 5155, done.
Fetching projects:  32% (127/395)  Fetching project device/generic/mips
Fetching project platform/external/javasqlite
Fetching project platform/external/smack
Fetching project platform/frameworks/opt/datetimepicker
remote: Compressing objects: 100% (1923/1923), done.
Fetching projects:  33% (131/395)  Fetching project platform/frameworks/compile/libbcc
Fetching project platform/external/safe-iop
Fetching project platform/ndk
Fetching project CyanogenMod/android_external_libnfc-nci
Fetching projects:  34% (135/395)  Fetching project CyanogenMod/android_external_sepolicy
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-eabi-4.7
Fetching project platform/external/sil-fonts
Fetching project platform/packages/wallpapers/LivePicker
Fetching projects:  35% (139/395)  Fetching project platform/external/qemu
Fetching project platform/external/kernel-headers
Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-eabi-4.6
Fetching project platform/packages/apps/VoiceDialer
Fetching projects:  36% (143/395)  Fetching project platform/external/sfntly
Fetching project platform/external/libffiFetching project platform/frameworks/opt/photoviewer

Fetching project CyanogenMod/android_frameworks_support
Fetching project platform/external/hamcrestg objects:  34% (1753/5155)   
Fetching project platform/frameworks/testing
Fetching project platform/packages/apps/SpeechRecorder
Fetching project platform/external/okhttp
Fetching projects:  38% (151/395)  Fetching project platform/external/chromium_org/sdch/open-vcdiff
Fetching project platform/frameworks/opt/emoji
Fetching project platform/prebuilts/gcc/darwin-x86/host/headers
Fetching project platform/external/chromium_org/testing/gtest
Fetching projects:  39% (155/395)  Fetching project CyanogenMod/android_packages_apps_Gallery2
Fetching project CyanogenMod/android_bionic
Fetching project platform/external/chromium_org/third_party/openssl
Fetching projects:  40% (158/395)  Fetching project CyanogenMod/android_external_flac
Fetching project AOSPA-legacy/android_packages_services_Telephony
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
curl: (22) The requested URL returned error: 404
Server does not provide clone.bundle; ignoring.
Fetching project platform/sdk/5155)   
Fetching project platform/prebuilts/clang/linux-x86/arm/3.3
Fetching projects:  41% (162/395)  Fetching project platform/packages/wallpapers/MusicVisualization
Fetching project platform/external/libnl-headers
Fetching project platform/external/opencv00 KiB | 1.21 MiB/s   
Fetching project platform/external/emma
Fetching projects:  42% (166/395)  Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.7
Fetching project platform/external/chromium_org/third_party/skia/src
Fetching project platform/external/libppp
Fetching project platform/packages/apps/CellBroadcastReceiver
Fetching projects:  43% (170/395)  Fetching project platform/frameworks/opt/inputmethodcommon
Fetching project platform/prebuilts/clang/linux-x86/3.1
Fetching project AOSPA-legacy/android_art
Fetching project platform/external/libvorbis
Fetching projects:  44% (174/395)  Fetching project platform/packages/apps/KeyChain
Fetching project platform/external/tagsoup
Fetching project AOSPA-legacy/android_packages_apps_Bluetooth
Fetching project CyanogenMod/Widgets
Fetching projects:  45% (178/395)  Fetching project platform/external/sqlite
Fetching project CyanogenMod/android_external_busybox
Fetching project CyanogenMod/android_external_e2fsprogsB/s     
Fetching project platform/external/oprofileiB | 1.29 MiB/s   
Fetching projects:  46% (182/395)  Fetching project platform/external/jpeg
Fetching project platform/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.4.3
Fetching project platform/external/elfutils
Fetching project platform/prebuilts/clang/darwin-x86/x86/3.3
Fetching projects:  47% (186/395)  Fetching project AOSPA-legacy/android_frameworks_base
Fetching project platform/external/libmtp
Fetching project platform/external/ant-glob
Fetching project platform/external/jsr305
Fetching projects:  48% (190/395)  Fetching project CyanogenMod/android_frameworks_opt_hardware
Fetching project platform/external/srec
Fetching project platform/packages/apps/Tag
Fetching project platform/external/apache-harmony
Fetching projects:  49% (194/395)  Fetching project platform/frameworks/opt/calendar
Fetching project CyanogenMod/android_packages_apps_Exchange
Fetching project CyanogenMod/android_frameworks_rs
Fetching project platform/external/stressapptest
Fetching projects:  50% (198/395)  Fetching project platform/external/webrtc
Fetching project platform/external/chromium_org/third_party/freetype
Fetching project platform/external/aac
Fetching project platform/external/proguard
Fetching projects:  51% (202/395)  Fetching project platform/frameworks/uiautomator
Fetching project AOSPA-legacy/manifest
Fetching project platform/external/tcpdump
Fetching project platform/external/chromium_org/third_party/mesa/src
Fetching projects:  52% (206/395)  Fetching project platform/external/chromium_org/third_party/opus/src
Fetching project CyanogenMod/android_packages_apps_Camera2
Fetching project platform/prebuilts/clang/linux-x86/mips/3.3
Fetching project AOSPA-legacy/android_vendor_pa
remote: Counting objects: 5660, done.
remote: Compressing objects: 100% (2076/2076), done.
Fetching projects:  53% (210/395)  Fetching project platform/prebuilts/gcc/darwin-x86/x86/i686-linux-android-4.6
Fetching project CyanogenMod/android_external_libsepol
Fetching project platform/external/replicaisland1.24 MiB/s   
Fetching project device/google/accessory/demokit
Fetching projects:  54% (214/395)  Fetching project platform/packages/providers/UserDictionaryProvider
Fetching project CyanogenMod/android_packages_apps_Launcher3
Fetching project platform/external/giflib
Fetching project AOSPA-legacy/android_packages_apps_ParanoidOTA
Fetching projects:  55% (218/395)  Fetching project platform/external/chromium_org/third_party/libjingle/source/talk
Fetching project platform/prebuilts/clang/darwin-x86/host/3.3
Fetching project CyanogenMod/android_hardware_broadcom_wlan
Fetching project CyanogenMod/android_hardware_ril
Fetching projects:  56% (222/395)  Fetching project platform/packages/inputmethods/OpenWnn
Fetching project platform/prebuilts/devtools
Fetching project platform/external/sonivox
Fetching project platform/packages/apps/MusicFX
Fetching projects:  57% (226/395)  Fetching project platform/cts
Fetching project platform/external/scrypt
Fetching project AOSPA-legacy/android_frameworks_opt_telephony-msim
Fetching project platform/frameworks/opt/timezonepicker
Fetching projects:  58% (230/395)  Fetching project CyanogenMod/android_packages_apps_Email
Fetching project platform/external/chromium_org/third_party/angle_dx11
Fetching project CyanogenMod/android_external_gson
Fetching project platform/external/apache-qpKiB | 522.00 KiB/s   
Fetching projects:  59% (234/395)  Fetching project platform/external/llvm
Fetching project platform/external/chromium_org/third_party/skia/gyp
Fetching project platform/external/chromium
Fetching projects:  60% (237/395)  Fetching project platform/prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.6
Fetching project platform/external/jack
Fetching project platform/external/compiler-rt
Fetching project platform/frameworks/compile/slang
Fetching projects:  61% (241/395)  Fetching project platform/external/libvpx
Fetching project platform/prebuilts/gcc/darwin-x86/mips/mipsel-linux-android-4.7
Fetching project platform/external/harfbuzz_ng
Fetching project platform/external/robolectric
Fetching projects:  62% (245/395)  Fetching project platform/prebuilts/qemu-kernel
Fetching project platform/external/regex-re2
Fetching project platform/frameworks/opt/mms
Fetching project platform/external/fdlibm
Fetching projects:  63% (249/395)  Fetching project CyanogenMod/android_packages_providers_DownloadProvider
Fetching project platform/external/yaffs200 KiB | 522.00 KiB/s   
Fetching project platform/external/tremolo
Fetching project platform/external/objenesis
Fetching projects:  64% (253/395)  Fetching project platform/external/jmonkeyengine
Fetching project CyanogenMod/android_external_libnfc-nxp
Fetching project platform/external/oauth
Fetching project platform/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.6
Fetching projects:  65% (257/395)  Fetching project platform/external/marisa-trie
Fetching project platform/prebuilts/gcc/darwin-x86/x86/x86_64-linux-android-4.7
Fetching project platform/packages/wallpapers/NoiseField KiB/s   
Fetching project proprietary_vendor_samsung
Fetching projects:  66% (261/395)  Fetching project platform/external/jsilver
Fetching project platform/frameworks/wilhelm
Fetching project platform/external/libusb-compat
Fetching project platform/external/webp
Fetching projects:  67% (265/395)  Fetching project platform/external/genext2fs
Fetching project platform/packages/wallpapers/Basic22.00 KiB/s   
Fetching project platform/prebuilts/eclipse
Fetching project platform/external/droiddriver
Fetching projects:  68% (269/395)  Fetching project platform/prebuilts/clang/darwin-x86/mips/3.3
Fetching project platform/external/timezonepicker-support
Fetching project platform/external/android-mock
Fetching project platform/external/eclipse-windowbuilder KiB/s   
Fetching projects:  69% (273/395)  Fetching project platform/bootable/bootloader/legacy
Fetching project AOSPA-legacy/android_packages_apps_Settings
Fetching project platform/external/jmdns
Fetching project device/generic/goldfish
Fetching projects:  70% (277/395)  Fetching project CyanogenMod/ion
Fetching project platform/external/javassist
Fetching project AOSPA-legacy/android_packages_apps_BluetoothExt
Fetching project platform/external/mp4parser
Fetching projects:  71% (281/395)  Fetching project platform/external/eyes-free
Fetching project platform/developers/docs
Fetching project platform/external/junit
Fetching project platform/packages/inputmethods/LatinIME
Fetching projects:  72% (285/395)  Fetching project platform/frameworks/ml
Fetching project platform/external/strace
Fetching project platform/external/grub
Fetching project CyanogenMod/android_external_chromium_org
Fetching projects:  73% (289/395)  Fetching project platform/packages/apps/PackageInstaller
Fetching project platform/external/expat
Fetching project CyanogenMod/android_system_security
Fetching project platform/packages/apps/Nfc
Fetching projects:  74% (293/395)  Fetching project platform/prebuilts/gcc/darwin-x86/arm/arm-linux-androideabi-4.6
Fetching project device/generic/mini-emulator-armv7-a-neon
Fetching project platform/external/netperf
Fetching project platform/packages/apps/HTMLViewer
Fetching projects:  75% (297/395)  Fetching project platform/bootable/diskinstaller
Fetching project platform/packages/screensavers/PhotoTable
Fetching project platform/external/mtpd
Fetching project platform/prebuilts/gcc/linux-x86/mips/mipsel-linux-android-4.6
Fetching projects:  76% (301/395)  Fetching project platform/external/libpcap
Fetching project platform/prebuilts/gcc/linux-x86/x86/i686-linux-android-4.6
Fetching project AOSPA/android_packages_apps_Lightbulb
Fetching project platform/packages/apps/SmartCardService
Fetching projects:  77% (305/395)  Fetching project CyanogenMod/android_system_media
Fetching project platform/developers/build
Fetching project platform/external/libcap-ng
Fetching project AOSPA-legacy/android_hardware_libhardware
Fetching projects:  78% (309/395)  Fetching project platform/external/openfst
Fetching project CyanogenMod/android_external_libselinux
Fetching project platform/external/chromium_org/tools/grit
Fetching project platform/packages/wallpapers/PhaseBeam
Fetching projects:  79% (313/395)  Fetching project CyanogenMod/android_packages_apps_VoicePlus
Fetching project platform/external/iputils
Fetching project AOSPA-legacy/android_build
warning: no common commits939/5155), 3.97 MiB | 1.12 MiB/s   
remote: Counting objects: 14146, done.
Fetching projects:  80% (316/395)  Fetching project CyanogenMod/android_packages_apps_UnifiedEmail
Fetching project platform/external/markdown
Fetching project CyanogenMod/android_hardware_broadcom_libbt
remote: Compressing objects: 100% (6399/6399), done.
Fetching project platform/external/netcat
Fetching projects:  81% (320/395)  Fetching project platform/external/chromium_org/third_party/icu
Fetching project CyanogenMod/android_hardware_cm
Fetching project CyanogenMod/android_packages_apps_Calendar
Fetching project platform/packages/apps/BasicSmsReceiver/s   
Fetching projects:  82% (324/395)  Fetching project platform/external/apache-http
Fetching project platform/packages/apps/SoundRecorder0 KiB/s   
Fetching project platform/packages/wallpapers/Galaxy4
Fetching project CyanogenMod/android_external_tinyalsa
Fetching projects:  83% (328/395)  Fetching project AOSPA-legacy/android_packages_apps_Dialer
Fetching project platform/external/checkpolicy
Fetching project CyanogenMod/android_external_zlib
Fetching project platform/external/chromium-trace
Fetching projects:  84% (332/395)  Fetching project CyanogenMod/android_external_wpa_supplicant_8
Fetching project platform/abi/cpp46), 296.00 KiB | 521.00 KiB/s   
Fetching project platform/external/esd.69 MiB | 561.00 KiB/s      
Fetching project CyanogenMod/android_packages_providers_ContactsProvider
Fetching projects:  85% (336/395)  Fetching project device/sample 
Fetching project platform/external/chromium_org/v8 521.00 KiB/s   
Fetching project platform/external/ceres-solver
Fetching project platform/external/blktrace
Fetching projects:  86% (340/395)  Fetching project platform/external/jhead
Fetching project platform/packages/apps/Provision| 521.00 KiB/s   
Fetching project platform/external/littlemockKiB | 521.00 KiB/s   
Fetching project platform/external/ppp
Fetching projects:  87% (344/395)  Fetching project platform/external/antlr
Fetching project platform/external/mockwebserver
Fetching project platform/tools/external/gradle
Fetching project CyanogenMod/android_packages_apps_Browser
Fetching projects:  88% (348/395)  Fetching project platform/developers/demos
Fetching project platform/docs/source.android.com
Fetching project CyanogenMod/android_packages_apps_Stk
Fetching project platform/external/android-clatB | 521.00 KiB/s   
Fetching projects:  89% (352/395)  Fetching project platform/external/apache-xml
Fetching project platform/external/chromium_org/third_party/eyesfree/src/android/java/src/com/googlecode/eyesfree/braille
Fetching project platform/frameworks/opt/net/voip
Fetching project platform/external/easymock
Fetching projects:  90% (356/395)  Fetching project platform/external/chromium-libpac
Fetching project platform/external/smali
Fetching project AOSPA-legacy/android_hardware_libhardware_legacy
Fetching project platform/external/srtp
Fetching projects:  91% (360/395)  Fetching project platform/packages/apps/PhoneCommon
Fetching project platform/external/mockito00 KiB | 765.00 KiB/s   
Fetching project platform/external/chromium_org/third_party/smhasher/src
Fetching project platform/external/zxing
Fetching projects:  92% (364/395)  Fetching project CyanogenMod/android_development
Fetching project platform/packages/screensavers/Basic5.00 KiB/s   
Fetching project CyanogenMod/android_packages_apps_Calculator/s   
Fetching project platform/external/iptablesMiB | 677.00 KiB/s     
Fetching projects:  93% (368/395)  Fetching project platform/packages/apps/Protips
Fetching project platform/prebuilts/sdk
Fetching project CyanogenMod/android_kernel_samsung_aries
Fetching project CyanogenMod/android_libcoreiB | 677.00 KiB/s   
Fetching projects:  94% (372/395)  Fetching project AOSPA-legacy/android_packages_providers_TelephonyProvider
Fetching project platform/external/google-diff-match-patch/s    
Fetching project platform/external/naver-fonts
Fetching project CyanogenMod/AndroidAsync
Fetching projects:  95% (376/395)  Fetching project platform/external/protobuf
Fetching project platform/external/bsdiff
Fetching project platform/external/chromium_org/third_party/ots
Fetching project platform/frameworks/compile/mclinker
Fetching projects:  96% (380/395)  Fetching project platform/external/xmp_toolkit
Fetching project platform/frameworks/mff
Fetching project platform/external/freetype
Fetching project platform/external/chromium_org/third_party/skia/include
Fetching projects:  97% (384/395)  Fetching project CyanogenMod/android_system_vold
Fetching project platform/prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.6
Fetching project platform/external/stlport
Fetching project platform/external/dnsmasq
Fetching projects:  98% (388/395)  Fetching project platform/libnativehelper
Fetching project platform/external/tinyxml2
remote: Total 5155 (delta 2826), reused 5096 (delta 2793)
Receiving objects: 100% (5155/5155), 8.60 MiB | 817.00 KiB/s, done.
Resolving deltas: 100% (2826/2826), done.4 MiB | 394.00 KiB/s   
From https://github.com/omnirom/android_bootable_recoveryB/s   
 * [new branch]      android-4.4 -> github/android-4.4
Fetching projects:  99% (392/395)  Receiving objects:  51% (7332/14146), 3.48 MiB | 441.00 KiB/remote: Counting objects: 139, done.
remote: Compressing objects: 100% (111/111), done.
remote: Total 139 (delta 52), reused 63 (delta 27)
Receiving objects: 100% (139/139), 363.53 KiB | 551.00 KiB/s, done.
Resolving deltas: 100% (52/52), done.
From https://github.com/CyanogenMod/android_kernel_samsung_aries
 + a011897...d859f62 cm-11.0    -> github/cm-11.0  (forced update)
 * [new tag]         cm-10.1-M1 -> cm-10.1-M1
 * [new tag]         cm-10.1-M2 -> cm-10.1-M2
 * [new tag]         cm-10.1-M3 -> cm-10.1-M3
 * [new tag]         cm-10.1.0  -> cm-10.1.0
 * [new tag]         cm-10.1.0-RC1 -> cm-10.1.0-RC1
 * [new tag]         cm-10.1.0-RC2 -> cm-10.1.0-RC2
 * [new tag]         cm-10.1.0-RC3 -> cm-10.1.0-RC3
 * [new tag]         cm-10.1.0-RC4 -> cm-10.1.0-RC4
 * [new tag]         cm-10.1.0-RC5 -> cm-10.1.0-RC5
 * [new tag]         cm-10.1.1  -> cm-10.1.1
 * [new tag]         cm-10.1.2  -> cm-10.1.2
 * [new tag]         cm-10.1.3  -> cm-10.1.3
 * [new tag]         cm-10.1.3-RC1 -> cm-10.1.3-RC1
 * [new tag]         cm-10.1.3-RC2 -> cm-10.1.3-RC2
 * [new tag]         cm-10.2-M1 -> cm-10.2-M1
 * [new tag]         cm-10.2.0  -> cm-10.2.0
remote: Total 5660 (delta 3090), reused 5660 (delta 3090)
Receiving objects: 100% (5660/5660), 10.89 MiB | 917.00 KiB/s, done.
Resolving deltas: 100% (3090/3090), done.
From https://github.com/CyanogenMod/android_packages_apps_Apollo
 * [new branch]      cm-11.0    -> github/cm-11.0
 * [new tag]         cm-10.1-M1 -> cm-10.1-M1
 * [new tag]         cm-10.1-M2 -> cm-10.1-M2
 * [new tag]         cm-10.1-M3 -> cm-10.1-M3
 * [new tag]         cm-10.1.0-RC1 -> cm-10.1.0-RC1
 * [new tag]         cm-10.2-M1 -> cm-10.2-M1
 * [new tag]         cm-10.2.0  -> cm-10.2.0
remote: Total 14146 (delta 7149), reused 14146 (delta 7149)
Receiving objects: 100% (14146/14146), 533.46 MiB | 1.66 MiB/s, done.
Resolving deltas: 100% (7149/7149), done.
From https://github.com/TheMuppets/proprietary_vendor_samsung
 * [new branch]      cm-11.0    -> blobs/cm-11.0
Fetching projects: 100% (395/395), done.  
Checking out files: 100% (37706/37706), done.ut files:   6% (2447/37706)   
Checking out files: 100% (4685/4685), done. out files:  14% (693/4685)   
Syncing work tree: 100% (395/395), done.  

bootable/recovery/: discarding 4 commits


hhp211@hhp211-Q500A:~/Source/AOSPA$ . build/envsetup.sh
including device/generic/armv7-a-neon/vendorsetup.sh
including device/generic/mips/vendorsetup.sh
including device/generic/x86/vendorsetup.sh
including vendor/pa/vendorsetup.sh
including sdk/bash_completion/adb.bash


hhp211@hhp211-Q500A:~/Source/AOSPA$ lunch

You're building on Linux

Lunch menu... pick a combo:
     1. mini_armv7a_neon-userdebug
     2. mini_mips-userdebug
     3. mini_x86-userdebug
     4. pa_d2lte-userdebug
     5. pa_d800-userdebug
     6. pa_d801-userdebug
     7. pa_d802-userdebug
     8. pa_d803-userdebug
     9. pa_dlx-userdebug
     10. pa_fascinatemtd-userdebug
     11. pa_galaxysmtd-userdebug
     12. pa_gee-userdebug
     13. pa_geeb-userdebug
     14. pa_hercules-userdebug
     15. pa_hlte-userdebug
     16. pa_i605-userdebug
     17. pa_i9300-userdebug
     18. pa_i9500-userdebug
     19. pa_jflte-userdebug
     20. pa_l900-userdebug
     21. pa_ls980-userdebug
     22. pa_m7-userdebug
     23. pa_moto_msm8960-userdebug
     24. pa_moto_msm8960dt-userdebug
     25. pa_n7000-userdebug
     26. pa_n7100-userdebug
     27. pa_p880-userdebug
     28. pa_skyrocket-userdebug
     29. pa_togari-userdebug
     30. pa_v500-userdebug
     31. pa_vs980-userdebug
     32. pa_yuga-userdebug

Which would you like? [aosp_arm-eng] 10

============================================
PLATFORM_VERSION_CODENAME=REL
PLATFORM_VERSION=4.4.2
TARGET_PRODUCT=pa_fascinatemtd
TARGET_BUILD_VARIANT=userdebug
TARGET_BUILD_TYPE=release
TARGET_BUILD_APPS=
TARGET_ARCH=arm
TARGET_ARCH_VARIANT=armv7-a-neon
TARGET_CPU_VARIANT=cortex-a8
HOST_ARCH=x86
HOST_OS=linux
HOST_OS_EXTRA=Linux-3.14.0-031400rc1-generic-x86_64-with-Ubuntu-12.04-precise
HOST_BUILD_TYPE=release
BUILD_ID=KVT49L
OUT_DIR=/home/hhp211/Source/AOSPA/out
============================================

hhp211@hhp211-Q500A:~/Source/AOSPA$ lunch

You're building on Linux

Lunch menu... pick a combo:
     1. mini_armv7a_neon-userdebug
     2. mini_mips-userdebug
     3. mini_x86-userdebug
     4. pa_d2lte-userdebug
     5. pa_d800-userdebug
     6. pa_d801-userdebug
     7. pa_d802-userdebug
     8. pa_d803-userdebug
     9. pa_dlx-userdebug
     10. pa_fascinatemtd-userdebug
     11. pa_galaxysmtd-userdebug
     12. pa_gee-userdebug
     13. pa_geeb-userdebug
     14. pa_hercules-userdebug
     15. pa_hlte-userdebug
     16. pa_i605-userdebug
     17. pa_i9300-userdebug
     18. pa_i9500-userdebug
     19. pa_jflte-userdebug
     20. pa_l900-userdebug
     21. pa_ls980-userdebug
     22. pa_m7-userdebug
     23. pa_moto_msm8960-userdebug
     24. pa_moto_msm8960dt-userdebug
     25. pa_n7000-userdebug
     26. pa_n7100-userdebug
     27. pa_p880-userdebug
     28. pa_skyrocket-userdebug
     29. pa_togari-userdebug
     30. pa_v500-userdebug
     31. pa_vs980-userdebug
     32. pa_yuga-userdebug

Which would you like? [aosp_arm-eng] 10

============================================
PLATFORM_VERSION_CODENAME=REL
PLATFORM_VERSION=4.4.2
TARGET_PRODUCT=pa_fascinatemtd
TARGET_BUILD_VARIANT=userdebug
TARGET_BUILD_TYPE=release
TARGET_BUILD_APPS=
TARGET_ARCH=arm
TARGET_ARCH_VARIANT=armv7-a-neon
TARGET_CPU_VARIANT=cortex-a8
HOST_ARCH=x86
HOST_OS=linux
HOST_OS_EXTRA=Linux-3.14.0-031400rc1-generic-x86_64-with-Ubuntu-12.04-precise
HOST_BUILD_TYPE=release
BUILD_ID=KVT49L
OUT_DIR=/home/hhp211/Source/AOSPA/out
============================================

hhp211@hhp211-Q500A:~/Source/AOSPA$ make
============================================
PLATFORM_VERSION_CODENAME=REL
PLATFORM_VERSION=4.4.2
TARGET_PRODUCT=pa_fascinatemtd
TARGET_BUILD_VARIANT=userdebug
TARGET_BUILD_TYPE=release
TARGET_BUILD_APPS=
TARGET_ARCH=arm
TARGET_ARCH_VARIANT=armv7-a-neon
TARGET_CPU_VARIANT=cortex-a8
HOST_ARCH=x86
HOST_OS=linux
HOST_OS_EXTRA=Linux-3.14.0-031400rc1-generic-x86_64-with-Ubuntu-12.04-precise
HOST_BUILD_TYPE=release
BUILD_ID=KVT49L
OUT_DIR=/home/hhp211/Source/AOSPA/out
============================================
/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/APPS/SignatureTest_intermediates
build/core/base_rules.mk:529: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/fsck_msdos'
bootable/recovery/dosfstools/Android.mk:21: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/fsck_msdos'
find: `src': No such file or directory
*** Overlay change detected, clean shared intermediate files...
*** rm -rf /home/hhp211/Source/AOSPA/out/target/common/obj/APPS/TelephonyProvider_intermediates /home/hhp211/Source/AOSPA/out/target/common/obj/APPS/Settings_intermediates /home/hhp211/Source/AOSPA/out/target/common/obj/APPS/framework-res_intermediates /home/hhp211/Source/AOSPA/out/target/common/obj/APPS/Mms_intermediates /home/hhp211/Source/AOSPA/out/target/common/obj/APPS/Gallery2_intermediates /home/hhp211/Source/AOSPA/out/target/common/obj/APPS/SystemUI_intermediates
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libril.so'
build/core/dynamic_binary.mk:117: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libril.so'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libril.so'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libril.so'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/rild'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/rild'
PRODUCT_COPY_FILES device/generic/goldfish/camera/media_profiles.xml:system/etc/media_profiles.xml ignored.
PRODUCT_COPY_FILES device/generic/goldfish/camera/media_codecs.xml:system/etc/media_codecs.xml ignored.
PRODUCT_COPY_FILES hardware/libhardware_legacy/audio/audio_policy.conf:system/etc/audio_policy.conf ignored.
PRODUCT_COPY_FILES vendor/pa/prebuilt/etc/apns-conf.xml:system/etc/apns-conf.xml ignored.
No private recovery resources for TARGET_DEVICE fascinatemtd
device/samsung/fascinatemtd/shbootimg.mk:8: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img'
device/samsung/fascinatemtd/shbootimg.mk:8: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img'
device/samsung/fascinatemtd/shbootimg.mk:12: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery.img'
device/samsung/fascinatemtd/shbootimg.mk:12: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery.img'
Export includes file: frameworks/native/libs/input/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libinput_intermediates/export_includes
Export includes file: system/core/libutils/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libutils_intermediates/export_includes
Export includes file: system/core/libcutils/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libcutils_intermediates/export_includes
Export includes file: system/core/liblog/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/liblog_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/validatekeymaps_intermediates/import_includes
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/libexpat/expat.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/libexpat/expat_external.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libexpat/expat.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libexpat/expat_external.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/libpng/png.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/libpng/pngconf.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/libpng/pngusr.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libpng/png.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libpng/pngconf.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libpng/pngusr.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/selinux/selinux.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/selinux/label.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/selinux/context.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/selinux/avc.h
Header: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/include/selinux/android.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/selinux/selinux.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/selinux/label.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/selinux/context.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/selinux/avc.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/selinux/android.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libsonivox/eas.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libsonivox/eas_types.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libsonivox/eas_reverb.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libsonivox/jet.h
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libsonivox/ARM_synth_constants_gnu.inc
Header: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/libwpa_client/wpa_ctrl.h
host C++: validatekeymaps <= frameworks/base/tools/validatekeymaps/Main.cpp
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libinput_intermediates/import_includes
host C++: libinput <= frameworks/native/libs/input/Input.cpp
host C++: libinput <= frameworks/native/libs/input/InputDevice.cpp
host C++: libinput <= frameworks/native/libs/input/Keyboard.cpp
host C++: libinput <= frameworks/native/libs/input/KeyCharacterMap.cpp
host C++: libinput <= frameworks/native/libs/input/KeyLayoutMap.cpp
host C++: libinput <= frameworks/native/libs/input/VirtualKeyMap.cpp
host StaticLib: libinput (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libinput_intermediates/libinput.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libutils_intermediates/import_includes
host C++: libutils <= system/core/libutils/BasicHashtable.cpp
host C++: libutils <= system/core/libutils/BlobCache.cpp
host C++: libutils <= system/core/libutils/CallStack.cpp
host C++: libutils <= system/core/libutils/FileMap.cpp
host C++: libutils <= system/core/libutils/JenkinsHash.cpp
host C++: libutils <= system/core/libutils/LinearAllocator.cpp
host C++: libutils <= system/core/libutils/LinearTransform.cpp
host C++: libutils <= system/core/libutils/Log.cpp
host C++: libutils <= system/core/libutils/Printer.cpp
host C++: libutils <= system/core/libutils/ProcessCallStack.cpp
host C++: libutils <= system/core/libutils/PropertyMap.cpp
host C++: libutils <= system/core/libutils/RefBase.cpp
host C++: libutils <= system/core/libutils/SharedBuffer.cpp
host C++: libutils <= system/core/libutils/Static.cpp
host C++: libutils <= system/core/libutils/StopWatch.cpp
host C++: libutils <= system/core/libutils/String8.cpp
host C++: libutils <= system/core/libutils/String16.cpp
host C++: libutils <= system/core/libutils/SystemClock.cpp
host C++: libutils <= system/core/libutils/Threads.cpp
host C++: libutils <= system/core/libutils/Timers.cpp
host C++: libutils <= system/core/libutils/Tokenizer.cpp
host C++: libutils <= system/core/libutils/Unicode.cpp
host C++: libutils <= system/core/libutils/VectorImpl.cpp
host C++: libutils <= system/core/libutils/misc.cpp
host C++: libutils <= system/core/libutils/Looper.cpp
host StaticLib: libutils (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libutils_intermediates/libutils.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libcutils_intermediates/import_includes
host C: libcutils <= system/core/libcutils/atomic.c
host C: libcutils <= system/core/libcutils/hashmap.c
host C: libcutils <= system/core/libcutils/native_handle.c
host C: libcutils <= system/core/libcutils/socket_inaddr_any_server.c
host C: libcutils <= system/core/libcutils/socket_local_client.c
host C: libcutils <= system/core/libcutils/socket_local_server.c
host C: libcutils <= system/core/libcutils/socket_loopback_client.c
host C: libcutils <= system/core/libcutils/socket_loopback_server.c
host C: libcutils <= system/core/libcutils/socket_network_client.c
host C: libcutils <= system/core/libcutils/sockets.c
host C: libcutils <= system/core/libcutils/config_utils.c
host C: libcutils <= system/core/libcutils/cpu_info.c
host C: libcutils <= system/core/libcutils/load_file.c
host C: libcutils <= system/core/libcutils/list.c
host C: libcutils <= system/core/libcutils/open_memstream.c
host C: libcutils <= system/core/libcutils/strdup16to8.c
host C: libcutils <= system/core/libcutils/strdup8to16.c
host C: libcutils <= system/core/libcutils/record_stream.c
host C: libcutils <= system/core/libcutils/process_name.c
host C: libcutils <= system/core/libcutils/threads.c
host C: libcutils <= system/core/libcutils/sched_policy.c
host C: libcutils <= system/core/libcutils/iosched_policy.c
host C: libcutils <= system/core/libcutils/str_parms.c
host C: libcutils <= system/core/libcutils/fs.c
host C: libcutils <= system/core/libcutils/multiuser.c
host C: libcutils <= system/core/libcutils/ashmem-host.c
host C: libcutils <= system/core/libcutils/dlmalloc_stubs.c
host StaticLib: libcutils (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libcutils_intermediates/libcutils.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/liblog_intermediates/import_includes
host C: liblog <= system/core/liblog/logd_write.c
system/core/liblog/logd_write.c: In function '__write_to_log_kernel':
system/core/liblog/logd_write.c:205:9: warning: implicit declaration of function 'fakeLogWritev' [-Wimplicit-function-declaration]
system/core/liblog/logd_write.c: In function '__write_to_log_init':
system/core/liblog/logd_write.c:218:9: warning: implicit declaration of function 'fakeLogOpen' [-Wimplicit-function-declaration]
system/core/liblog/logd_write.c:227:13: warning: implicit declaration of function 'fakeLogClose' [-Wimplicit-function-declaration]
host C: liblog <= system/core/liblog/logprint.c
host C: liblog <= system/core/liblog/event_tag_map.c
host C: liblog <= system/core/liblog/fake_log_device.c
host StaticLib: liblog (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/liblog_intermediates/liblog.a)
Export includes file: frameworks/base/tools/validatekeymaps/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/validatekeymaps_intermediates/export_includes
host Executable: validatekeymaps (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/validatekeymaps_intermediates/validatekeymaps)
Export includes file: build/libs/host/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libhost_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/acp_intermediates/import_includes
host C: acp <= build/tools/acp/acp.c
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libhost_intermediates/import_includes
host C: libhost <= build/libs/host/CopyFile.c
host StaticLib: libhost (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libhost_intermediates/libhost.a)
Export includes file: build/tools/acp/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/acp_intermediates/export_includes
host Executable: acp (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/acp_intermediates/acp)
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/acp
Notice file: system/core/libutils/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libutils.a.txt
Notice file: system/core/libcutils/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libcutils.a.txt
Notice file: system/core/liblog/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/liblog.a.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/validatekeymaps
Validating file 'frameworks/base/data/keyboards/AVRCP.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Generic.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/qwerty.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_0079_Product_0011.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_045e_Product_028e.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_046d_Product_c216.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_046d_Product_c219.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_046d_Product_c21f.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_046d_Product_c294.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_046d_Product_c299.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_046d_Product_c532.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_054c_Product_0268.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_0583_Product_2060.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_05ac_Product_0239.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1038_Product_1412.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_12bd_Product_d015.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1689_Product_fd00.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1689_Product_fd01.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1689_Product_fe00.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1bad_Product_f016.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1bad_Product_f023.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1bad_Product_f027.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1bad_Product_f036.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_1d79_Product_0009.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_22b8_Product_093d.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Vendor_2378_Product_100a.kl'...
No errors.

Validating file 'frameworks/base/data/keyboards/Generic.kcm'...
No errors.

Validating file 'frameworks/base/data/keyboards/qwerty2.kcm'...
No errors.

Validating file 'frameworks/base/data/keyboards/qwerty.kcm'...
No errors.

Validating file 'frameworks/base/data/keyboards/Virtual.kcm'...
No errors.

Validating file 'frameworks/base/data/keyboards/qwerty2.idc'...
No errors.

Validating file 'frameworks/base/data/keyboards/qwerty.idc'...
No errors.

Success.
Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_belgian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_brazilian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_bulgarian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_croatian_and_slovenian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_czech.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_danish.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_english_uk.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_english_us_colemak.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_english_us_dvorak.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_english_us_intl.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_english_us.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_estonian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_finnish.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_french_ca.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_french.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_german.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_hungarian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_icelandic.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_italian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_norwegian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_portuguese.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_russian.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_russian_mac.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_slovak.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_spanish.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_swedish.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_swiss_french.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_swiss_german.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_turkish.kcm'...
No errors.

Validating file 'frameworks/base/packages/InputDevices/res/raw/keyboard_layout_ukrainian.kcm'...
No errors.

Success.
host Java: antlr-runtime (/home/hhp211/Source/AOSPA/out/host/common/obj/JAVA_LIBRARIES/antlr-runtime_intermediates/classes)
warning: [options] bootstrap class path not set in conjunction with -source 1.5
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
1 warning
Notice file: external/antlr/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//framework/antlr-runtime.jar.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/framework/antlr-runtime.jar
host Java: jsr305lib (/home/hhp211/Source/AOSPA/out/host/common/obj/JAVA_LIBRARIES/jsr305lib_intermediates/classes)
warning: [options] bootstrap class path not set in conjunction with -source 1.5
1 warning
host Java: guavalib (/home/hhp211/Source/AOSPA/out/host/common/obj/JAVA_LIBRARIES/guavalib_intermediates/classes)
warning: [options] bootstrap class path not set in conjunction with -source 1.5
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: external/guava/guava/src/com/google/common/base/Joiner.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
1 warning
Notice file: external/guava/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//framework/guavalib.jar.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/framework/guavalib.jar
host Java: jsilver (/home/hhp211/Source/AOSPA/out/host/common/obj/JAVA_LIBRARIES/jsilver_intermediates/classes)
warning: [options] bootstrap class path not set in conjunction with -source 1.5
Note: external/jsilver/src/org/clearsilver/FactoryLoader.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
1 warning
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/framework/jsilver.jar
host Java: doclava (/home/hhp211/Source/AOSPA/out/host/common/obj/JAVA_LIBRARIES/doclava_intermediates/classes)
warning: [options] bootstrap class path not set in conjunction with -source 1.5
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
1 warning
Notice file: external/doclava/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//framework/doclava.jar.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/framework/doclava.jar
target Java: core (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/core_intermediates/classes)
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/core_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/core_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/core_intermediates/classes.jar
target Java: conscrypt (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/conscrypt_intermediates/classes)
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
host Prebuilt: jarjar (/home/hhp211/Source/AOSPA/out/host/common/obj/JAVA_LIBRARIES/jarjar_intermediates/javalib.jar)
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/framework/jarjar.jar
JarJar: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/conscrypt_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/conscrypt_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/conscrypt_intermediates/classes.jar
target Java: bouncycastle (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/bouncycastle_intermediates/classes)
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
JarJar: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/bouncycastle_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/bouncycastle_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/bouncycastle_intermediates/classes.jar
target Java: ext (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/ext_intermediates/classes)
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/ext_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/ext_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/ext_intermediates/classes.jar
Yacc: aidl <= frameworks/base/tools/aidl/aidl_language_y.y
prebuilts/misc/linux-x86/bison/bison -d  -o /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.cpp frameworks/base/tools/aidl/aidl_language_y.y
touch /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.hpp
echo '#ifndef 'aidl_language_y_h > /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.h
echo '#define 'aidl_language_y_h >> /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.h
cat /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.hpp >> /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.h
echo '#endif' >> /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.h
rm -f /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.hpp
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/import_includes
host C++: aidl <= frameworks/base/tools/aidl/aidl.cpp
host C++: aidl <= frameworks/base/tools/aidl/aidl_language.cpp
host C++: aidl <= frameworks/base/tools/aidl/options.cpp
host C++: aidl <= frameworks/base/tools/aidl/search_path.cpp
host C++: aidl <= frameworks/base/tools/aidl/AST.cpp
host C++: aidl <= frameworks/base/tools/aidl/Type.cpp
host C++: aidl <= frameworks/base/tools/aidl/generate_java.cpp
host C++: aidl <= frameworks/base/tools/aidl/generate_java_binder.cpp
host C++: aidl <= frameworks/base/tools/aidl/generate_java_rpc.cpp
host C++: aidl <= /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.cpp
/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.cpp: In function 'int yyparse()':
/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.cpp:1947:35: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_y.cpp:2091:35: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
Lex: aidl <= frameworks/base/tools/aidl/aidl_language_l.l
frameworks/base/tools/aidl/aidl_language_l.l:55: warning, rule cannot be matched
host C++: aidl <= /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl_language_l.cpp
Export includes file: frameworks/base/tools/aidl/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/export_includes
host Executable: aidl (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aidl_intermediates/aidl)
Notice file: frameworks/base/tools/aidl/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//bin/aidl.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/aidl
Aidl: framework-base <= frameworks/base/core/java/android/accessibilityservice/IAccessibilityServiceConnection.aidl
Aidl: framework-base <= frameworks/base/core/java/android/accessibilityservice/IAccessibilityServiceClient.aidl
Aidl: framework-base <= frameworks/base/core/java/android/accounts/IAccountManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/accounts/IAccountManagerResponse.aidl
Aidl: framework-base <= frameworks/base/core/java/android/accounts/IAccountAuthenticator.aidl
Aidl: framework-base <= frameworks/base/core/java/android/accounts/IAccountAuthenticatorResponse.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IActivityController.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IActivityPendingResult.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IAlarmManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IBackupAgent.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IInstrumentationWatcher.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/INotificationManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IProcessObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/ISearchManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/ISearchManagerCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IServiceConnection.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IStopUserCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IThumbnailReceiver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IThumbnailRetriever.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/ITransientNotification.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IUiAutomationConnection.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IUiModeManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IUserSwitchObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IWallpaperManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/IWallpaperManagerCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/admin/IDevicePolicyManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/backup/IBackupManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/backup/IFullBackupRestoreObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/backup/IRestoreObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/app/backup/IRestoreSession.aidl
Aidl: framework-base <= frameworks/base/core/java/android/wipower/IWipower.aidl
Aidl: framework-base <= frameworks/base/core/java/android/wipower/IWipowerManagerCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetooth.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IQBluetooth.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothA2dp.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IQBluetoothAdapterCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothHeadset.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothHeadsetPhone.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothHealth.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothHealthCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothInputDevice.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothPan.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothManagerCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IQBluetoothManagerCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothPbap.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothMap.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothStateChangeCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothHandsfreeClient.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothHidDevice.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothHidDeviceCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothGatt.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothGattCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothGattServerCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothSap.aidl
Aidl: framework-base <= frameworks/base/core/java/android/bluetooth/IBluetoothDun.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/IClipboard.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/IContentService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/IIntentReceiver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/IIntentSender.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/IOnPrimaryClipChangedListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/IAnonymousSyncAdapter.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/ISyncAdapter.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/ISyncContext.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/ISyncStatusObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/pm/IPackageDataObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/pm/IPackageDeleteObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/pm/IPackageInstallObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/pm/IPackageManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/pm/IPackageMoveObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/content/pm/IPackageStatsObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/database/IContentObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/ICameraService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/ICameraServiceListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/ICamera.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/ICameraClient.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/IConsumerIrService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/IProCameraUser.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/IProCameraCallbacks.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/camera2/ICameraDeviceUser.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/camera2/ICameraDeviceCallbacks.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/ISerialManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/display/IDisplayManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/display/IDisplayManagerCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/input/IInputManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/input/IInputDevicesChangedListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/location/IFusedLocationHardware.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/location/IFusedLocationHardwareSink.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/location/IGeofenceHardware.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/location/IGeofenceHardwareCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/location/IGeofenceHardwareMonitorCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/hardware/usb/IUsbManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/net/IConnectivityManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/net/INetworkManagementEventObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/net/INetworkPolicyListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/net/INetworkPolicyManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/net/INetworkStatsService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/net/INetworkStatsSession.aidl
Aidl: framework-base <= frameworks/base/core/java/android/net/nsd/INsdManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/nfc/IAppCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/nfc/INfcAdapter.aidl
Aidl: framework-base <= frameworks/base/core/java/android/nfc/INfcAdapterExtras.aidl
Aidl: framework-base <= frameworks/base/core/java/android/nfc/INfcTag.aidl
Aidl: framework-base <= frameworks/base/core/java/android/nfc/INfcCardEmulation.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IBatteryPropertiesListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IBatteryPropertiesRegistrar.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/ICancellationSignal.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IHardwareService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IMessenger.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/INetworkManagementService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IPermissionController.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IPowerManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IRemoteCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/ISchedulingPolicyService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IUpdateLock.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IUserManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/os/IVibratorService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/notification/INotificationListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/ILayoutResultCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IPrinterDiscoveryObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IPrintDocumentAdapter.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IPrintDocumentAdapterObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IPrintJobStateChangeListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IPrintManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IPrintSpooler.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IPrintSpoolerCallbacks.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IPrintSpoolerClient.aidl
Aidl: framework-base <= frameworks/base/core/java/android/print/IWriteResultCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/printservice/IPrintService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/printservice/IPrintServiceClient.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/dreams/IDreamManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/dreams/IDreamService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/gesture/IGestureService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/gesture/IEdgeGestureService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/gesture/IEdgeGestureActivationListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/gesture/IEdgeGestureHostCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/wallpaper/IWallpaperConnection.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/wallpaper/IWallpaperEngine.aidl
Aidl: framework-base <= frameworks/base/core/java/android/service/wallpaper/IWallpaperService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/accessibility/IAccessibilityInteractionConnection.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/accessibility/IAccessibilityInteractionConnectionCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/accessibility/IAccessibilityManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/accessibility/IAccessibilityManagerClient.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IApplicationToken.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IAssetAtlas.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IMagnificationCallbacks.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IInputFilter.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IInputFilterHost.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IOnKeyguardExitResult.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IRotationWatcher.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IWindow.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IWindowFocusObserver.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IWindowId.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IWindowManager.aidl
Aidl: framework-base <= frameworks/base/core/java/android/view/IWindowSession.aidl
Aidl: framework-base <= frameworks/base/core/java/android/speech/IRecognitionListener.aidl
Aidl: framework-base <= frameworks/base/core/java/android/speech/IRecognitionService.aidl
Aidl: framework-base <= frameworks/base/core/java/android/speech/tts/ITextToSpeechCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/android/speech/tts/ITextToSpeechService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/app/IAppOpsCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/app/IAppOpsService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/app/IBatteryStats.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/app/IProcessStats.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/app/IUsageStats.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/app/IMediaContainerService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/appwidget/IAppWidgetService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/appwidget/IAppWidgetHost.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/backup/IBackupTransport.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/backup/IObbBackupService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/policy/IFaceLockCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/policy/IFaceLockInterface.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/policy/IKeyguardShowCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/policy/IKeyguardExitCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/policy/IKeyguardService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/os/IDropBoxManagerService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/os/IResultReceiver.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/statusbar/IStatusBar.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/statusbar/IStatusBarService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/textservice/ISpellCheckerService.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/textservice/ISpellCheckerSession.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/textservice/ISpellCheckerSessionListener.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/textservice/ITextServicesManager.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/textservice/ITextServicesSessionListener.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/view/IInputContext.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/view/IInputContextCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/view/IInputMethod.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/view/IInputMethodClient.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/view/IInputMethodManager.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/view/IInputMethodSession.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/view/IInputSessionCallback.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/widget/ILockSettings.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/widget/IRemoteViewsFactory.aidl
Aidl: framework-base <= frameworks/base/core/java/com/android/internal/widget/IRemoteViewsAdapterConnection.aidl
Aidl: framework-base <= frameworks/base/keystore/java/android/security/IKeyChainAliasCallback.aidl
Aidl: framework-base <= frameworks/base/keystore/java/android/security/IKeyChainService.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/ICountryDetector.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/ICountryListener.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IFusedProvider.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IGeocodeProvider.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IGeofenceProvider.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IGeoFencer.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IGeoFenceListener.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IGpsStatusListener.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IGpsStatusProvider.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/ILocationListener.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/ILocationManager.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IFusedGeofenceHardware.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/IGpsGeofenceHardware.aidl
Aidl: framework-base <= frameworks/base/location/java/android/location/INetInitiatedListener.aidl
Aidl: framework-base <= frameworks/base/location/java/com/android/internal/location/ILocationProvider.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IAudioService.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IAudioFocusDispatcher.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IAudioRoutesObserver.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IMediaRouterClient.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IMediaRouterService.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IMediaScannerListener.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IMediaScannerService.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IRemoteControlClient.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IRemoteControlDisplay.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IRemoteDisplayCallback.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IRemoteDisplayProvider.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IRemoteVolumeObserver.aidl
Aidl: framework-base <= frameworks/base/media/java/android/media/IRingtonePlayer.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/IPhoneStateListener.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/IPhoneSubInfo.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/msim/IPhoneSubInfoMSim.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/ITelephony.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/msim/ITelephonyMSim.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/ISms.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/ITelephonyRegistry.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/ITelephonyRegistryMSim.aidl
Aidl: framework-base <= frameworks/base/telephony/java/com/android/internal/telephony/IWapPushManager.aidl
Aidl: framework-base <= frameworks/base/wifi/java/android/net/wifi/IWifiManager.aidl
Aidl: framework-base <= frameworks/base/wifi/java/android/net/wifi/p2p/IWifiP2pManager.aidl
Aidl: framework-base <= frameworks/base/packages/services/PacProcessor/com/android/net/IProxyService.aidl
Aidl: framework-base <= frameworks/base/packages/services/Proxy/com/android/net/IProxyCallback.aidl
Aidl: framework-base <= frameworks/base/packages/services/Proxy/com/android/net/IProxyPortListener.aidl
logtags: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework-base_intermediates/src/core/java/android/content/EventLogTags.java <= frameworks/base/core/java/android/content/EventLogTags.logtags
logtags: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework-base_intermediates/src/core/java/android/speech/tts/EventLogTags.java <= frameworks/base/core/java/android/speech/tts/EventLogTags.logtags
logtags: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework-base_intermediates/src/core/java/android/webkit/EventLogTags.java <= frameworks/base/core/java/android/webkit/EventLogTags.logtags
target Java: core-junit (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/core-junit_intermediates/classes)
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/core-junit_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/core-junit_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/core-junit_intermediates/classes.jar
target Java: okhttp (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/okhttp_intermediates/classes)
JarJar: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/okhttp_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/okhttp_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/okhttp_intermediates/classes.jar
Export includes file: frameworks/base/libs/androidfw/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libandroidfw_intermediates/export_includes
Export includes file: external/expat/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libexpat_intermediates/export_includes
Export includes file: external/libpng/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libpng_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aapt_intermediates/import_includes
host C++: aapt <= frameworks/base/tools/aapt/AaptAssets.cpp
host C++: aapt <= frameworks/base/tools/aapt/Command.cpp
host C++: aapt <= frameworks/base/tools/aapt/CrunchCache.cpp
host C++: aapt <= frameworks/base/tools/aapt/FileFinder.cpp
host C++: aapt <= frameworks/base/tools/aapt/Main.cpp
host C++: aapt <= frameworks/base/tools/aapt/Package.cpp
host C++: aapt <= frameworks/base/tools/aapt/StringPool.cpp
host C++: aapt <= frameworks/base/tools/aapt/XMLNode.cpp
host C++: aapt <= frameworks/base/tools/aapt/ResourceFilter.cpp
host C++: aapt <= frameworks/base/tools/aapt/ResourceIdCache.cpp
In file included from frameworks/base/tools/aapt/ResourceIdCache.cpp:10:0:
frameworks/base/tools/aapt/ResourceIdCache.h:10:16: warning: declaration 'class android::String16' does not declare anything [enabled by default]
frameworks/base/tools/aapt/ResourceIdCache.cpp: In static member function 'static void android::ResourceIdCache::dump()':
frameworks/base/tools/aapt/ResourceIdCache.cpp:101:40: warning: format '%ld' expects argument of type 'long int', but argument 2 has type 'std::map<unsigned int, CacheEntry>::size_type {aka unsigned int}' [-Wformat]
frameworks/base/tools/aapt/ResourceIdCache.cpp:102:34: warning: format '%ld' expects argument of type 'long int', but argument 2 has type 'size_t {aka unsigned int}' [-Wformat]
frameworks/base/tools/aapt/ResourceIdCache.cpp:103:36: warning: format '%ld' expects argument of type 'long int', but argument 2 has type 'size_t {aka unsigned int}' [-Wformat]
frameworks/base/tools/aapt/ResourceIdCache.cpp:104:46: warning: format '%ld' expects argument of type 'long int', but argument 2 has type 'size_t {aka unsigned int}' [-Wformat]
host C++: aapt <= frameworks/base/tools/aapt/ResourceTable.cpp
In file included from frameworks/base/tools/aapt/ResourceTable.cpp:11:0:
frameworks/base/tools/aapt/ResourceIdCache.h:10:16: warning: declaration 'class android::String16' does not declare anything [enabled by default]
host C++: aapt <= frameworks/base/tools/aapt/Images.cpp
host C++: aapt <= frameworks/base/tools/aapt/Resource.cpp
host C++: aapt <= frameworks/base/tools/aapt/pseudolocalize.cpp
host C++: aapt <= frameworks/base/tools/aapt/SourcePos.cpp
host C++: aapt <= frameworks/base/tools/aapt/WorkQueue.cpp
host C++: aapt <= frameworks/base/tools/aapt/ZipEntry.cpp
host C++: aapt <= frameworks/base/tools/aapt/ZipFile.cpp
host C: aapt <= frameworks/base/tools/aapt/qsort_r_compat.c
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libandroidfw_intermediates/import_includes
host C++: libandroidfw <= frameworks/base/libs/androidfw/Asset.cpp
host C++: libandroidfw <= frameworks/base/libs/androidfw/AssetDir.cpp
host C++: libandroidfw <= frameworks/base/libs/androidfw/AssetManager.cpp
host C++: libandroidfw <= frameworks/base/libs/androidfw/misc.cpp
host C++: libandroidfw <= frameworks/base/libs/androidfw/ObbFile.cpp
frameworks/base/libs/androidfw/ObbFile.cpp: In member function 'bool android::ObbFile::parseObbFile(int)':
frameworks/base/libs/androidfw/ObbFile.cpp:140:22: warning: deleting array 'char footer [8]' [enabled by default]
frameworks/base/libs/androidfw/ObbFile.cpp:148:22: warning: deleting array 'char footer [8]' [enabled by default]
frameworks/base/libs/androidfw/ObbFile.cpp:157:22: warning: deleting array 'char footer [8]' [enabled by default]
frameworks/base/libs/androidfw/ObbFile.cpp:164:22: warning: deleting array 'char footer [8]' [enabled by default]
frameworks/base/libs/androidfw/ObbFile.cpp:167:18: warning: deleting array 'char footer [8]' [enabled by default]
host C++: libandroidfw <= frameworks/base/libs/androidfw/ResourceTypes.cpp
frameworks/base/libs/androidfw/ResourceTypes.cpp: In member function 'void android::ResTable::print(bool) const':
frameworks/base/libs/androidfw/ResourceTypes.cpp:5737:84: warning: cast to pointer from integer of different size [-Wint-to-pointer-cast]
frameworks/base/libs/androidfw/ResourceTypes.cpp:5743:43: warning: cast to pointer from integer of different size [-Wint-to-pointer-cast]
host C++: libandroidfw <= frameworks/base/libs/androidfw/StreamingZipInflater.cpp
host C++: libandroidfw <= frameworks/base/libs/androidfw/ZipFileRO.cpp
host C++: libandroidfw <= frameworks/base/libs/androidfw/ZipUtils.cpp
host StaticLib: libandroidfw (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libandroidfw_intermediates/libandroidfw.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libexpat_intermediates/import_includes
host C: libexpat <= external/expat/lib/xmlparse.c
host C: libexpat <= external/expat/lib/xmlrole.c
host C: libexpat <= external/expat/lib/xmltok.c
host StaticLib: libexpat (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libexpat_intermediates/libexpat.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libpng_intermediates/import_includes
host C: libpng <= external/libpng/png.c
host C: libpng <= external/libpng/pngerror.c
host C: libpng <= external/libpng/pnggccrd.c
host C: libpng <= external/libpng/pngget.c
host C: libpng <= external/libpng/pngmem.c
host C: libpng <= external/libpng/pngpread.c
host C: libpng <= external/libpng/pngread.c
host C: libpng <= external/libpng/pngrio.c
host C: libpng <= external/libpng/pngrtran.c
host C: libpng <= external/libpng/pngrutil.c
host C: libpng <= external/libpng/pngset.c
host C: libpng <= external/libpng/pngtrans.c
host C: libpng <= external/libpng/pngvcrd.c
host C: libpng <= external/libpng/pngwio.c
host C: libpng <= external/libpng/pngwrite.c
host C: libpng <= external/libpng/pngwtran.c
host C: libpng <= external/libpng/pngwutil.c
host StaticLib: libpng (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libpng_intermediates/libpng.a)
Export includes file: frameworks/base/tools/aapt/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aapt_intermediates/export_includes
host Executable: aapt (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/aapt_intermediates/aapt)
Notice file: frameworks/base/tools/aapt/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//bin/aapt.txt
Notice file: frameworks/base/libs/androidfw/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libandroidfw.a.txt
Notice file: external/expat/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libexpat.a.txt
Notice file: external/libpng/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libpng.a.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/aapt
target Export Resources: framework-res (/home/hhp211/Source/AOSPA/out/target/common/obj/APPS/framework-res_intermediates/package-export.apk)
libpng warning: Ignoring attempt to set cHRM RGB triangle with zero area
libpng warning: Ignoring attempt to set cHRM RGB triangle with zero area
target R.java/Manifest.java: framework-res (/home/hhp211/Source/AOSPA/out/target/common/obj/APPS/framework-res_intermediates/src/R.stamp)
frameworks/base/core/res/AndroidManifest.xml:1679: warning: No comment for public symbol android:permission/SUBSCRIBED_FEEDS_WRITE
frameworks/base/core/res/res/values/public.xml:923: warning: No comment for public symbol android:anim/accelerate_decelerate_interpolator
frameworks/base/core/res/res/values/public.xml:1141: warning: No comment for public symbol android:anim/anticipate_interpolator
frameworks/base/core/res/res/values/public.xml:1143: warning: No comment for public symbol android:anim/anticipate_overshoot_interpolator
frameworks/base/core/res/res/values/public.xml:1144: warning: No comment for public symbol android:anim/bounce_interpolator
frameworks/base/core/res/res/values/public.xml:1243: warning: No comment for public symbol android:anim/cycle_interpolator
frameworks/base/core/res/res/values/public.xml:919: warning: No comment for public symbol android:anim/fade_in
frameworks/base/core/res/res/values/public.xml:920: warning: No comment for public symbol android:anim/fade_out
frameworks/base/core/res/res/values/public.xml:1145: warning: No comment for public symbol android:anim/linear_interpolator
frameworks/base/core/res/res/values/public.xml:1142: warning: No comment for public symbol android:anim/overshoot_interpolator
frameworks/base/core/res/res/values/public.xml:921: warning: No comment for public symbol android:anim/slide_in_left
frameworks/base/core/res/res/values/public.xml:922: warning: No comment for public symbol android:anim/slide_out_right
frameworks/base/core/res/res/values/public.xml:1322: warning: No comment for public symbol android:attr/actionBarTabBarStyle
frameworks/base/core/res/res/values/public.xml:1323: warning: No comment for public symbol android:attr/actionBarTabTextStyle
frameworks/base/core/res/res/values/public.xml:1325: warning: No comment for public symbol android:attr/actionModeCloseButtonStyle
frameworks/base/core/res/res/values/public.xml:1750: warning: No comment for public symbol android:attr/actionModeStyle
frameworks/base/core/res/res/values/public.xml:1324: warning: No comment for public symbol android:attr/actionOverflowButtonStyle
frameworks/base/core/res/res/values/public.xml:121: warning: No comment for public symbol android:attr/alertDialogStyle
frameworks/base/core/res/res/values/public.xml:233: warning: No comment for public symbol android:attr/bottomBright
frameworks/base/core/res/res/values/public.xml:229: warning: No comment for public symbol android:attr/bottomDark
frameworks/base/core/res/res/values/public.xml:234: warning: No comment for public symbol android:attr/bottomMedium
frameworks/base/core/res/res/values/public.xml:232: warning: No comment for public symbol android:attr/centerBright
frameworks/base/core/res/res/values/public.xml:228: warning: No comment for public symbol android:attr/centerDark
frameworks/base/core/res/res/values/public.xml:235: warning: No comment for public symbol android:attr/centerMedium
frameworks/base/core/res/res/values/public.xml:498: warning: No comment for public symbol android:attr/cycles
frameworks/base/core/res/res/values/public.xml:286: warning: No comment for public symbol android:attr/dial
frameworks/base/core/res/res/values/public.xml:2067: warning: No comment for public symbol android:attr/fadingMode
frameworks/base/core/res/res/values/public.xml:405: warning: No comment for public symbol android:attr/flipInterval
frameworks/base/core/res/res/values/public.xml:1309: warning: No comment for public symbol android:attr/fragmentCloseEnterAnimation
frameworks/base/core/res/res/values/public.xml:1310: warning: No comment for public symbol android:attr/fragmentCloseExitAnimation
frameworks/base/core/res/res/values/public.xml:1311: warning: No comment for public symbol android:attr/fragmentFadeEnterAnimation
frameworks/base/core/res/res/values/public.xml:1312: warning: No comment for public symbol android:attr/fragmentFadeExitAnimation
frameworks/base/core/res/res/values/public.xml:1307: warning: No comment for public symbol android:attr/fragmentOpenEnterAnimation
frameworks/base/core/res/res/values/public.xml:1308: warning: No comment for public symbol android:attr/fragmentOpenExitAnimation
frameworks/base/core/res/res/values/public.xml:488: warning: No comment for public symbol android:attr/fromAlpha
frameworks/base/core/res/res/values/public.xml:465: warning: No comment for public symbol android:attr/fromDegrees
frameworks/base/core/res/res/values/public.xml:484: warning: No comment for public symbol android:attr/fromXDelta
frameworks/base/core/res/res/values/public.xml:480: warning: No comment for public symbol android:attr/fromXScale
frameworks/base/core/res/res/values/public.xml:486: warning: No comment for public symbol android:attr/fromYDelta
frameworks/base/core/res/res/values/public.xml:482: warning: No comment for public symbol android:attr/fromYScale
frameworks/base/core/res/res/values/public.xml:230: warning: No comment for public symbol android:attr/fullBright
frameworks/base/core/res/res/values/public.xml:226: warning: No comment for public symbol android:attr/fullDark
frameworks/base/core/res/res/values/public.xml:287: warning: No comment for public symbol android:attr/hand_hour
frameworks/base/core/res/res/values/public.xml:288: warning: No comment for public symbol android:attr/hand_minute
frameworks/base/core/res/res/values/public.xml:472: warning: No comment for public symbol android:attr/insetBottom
frameworks/base/core/res/res/values/public.xml:469: warning: No comment for public symbol android:attr/insetLeft
frameworks/base/core/res/res/values/public.xml:470: warning: No comment for public symbol android:attr/insetRight
frameworks/base/core/res/res/values/public.xml:471: warning: No comment for public symbol android:attr/insetTop
frameworks/base/core/res/res/values/public.xml:349: warning: No comment for public symbol android:attr/interpolator
frameworks/base/core/res/res/values/public.xml:433: warning: No comment for public symbol android:attr/layout_scale
frameworks/base/core/res/res/values/public.xml:415: warning: No comment for public symbol android:attr/layout_weight
frameworks/base/core/res/res/values/public.xml:413: warning: No comment for public symbol android:attr/layout_x
frameworks/base/core/res/res/values/public.xml:414: warning: No comment for public symbol android:attr/layout_y
frameworks/base/core/res/res/values/public.xml:348: warning: No comment for public symbol android:attr/minHeight
frameworks/base/core/res/res/values/public.xml:347: warning: No comment for public symbol android:attr/minWidth
frameworks/base/core/res/res/values/public.xml:412: warning: No comment for public symbol android:attr/mode
frameworks/base/core/res/res/values/public.xml:467: warning: No comment for public symbol android:attr/pivotX
frameworks/base/core/res/res/values/public.xml:468: warning: No comment for public symbol android:attr/pivotY
frameworks/base/core/res/res/values/public.xml:1260: warning: No comment for public symbol android:attr/popupAnimationStyle
frameworks/base/core/res/res/values/public.xml:402: warning: No comment for public symbol android:attr/popupBackground
frameworks/base/core/res/res/values/public.xml:473: warning: No comment for public symbol android:attr/shareInterpolator
frameworks/base/core/res/res/values/public.xml:303: warning: No comment for public symbol android:attr/spacing
frameworks/base/core/res/res/values/public.xml:1165: warning: No comment for public symbol android:attr/supportsUploading
frameworks/base/core/res/res/values/public.xml:99: warning: No comment for public symbol android:attr/textCheckMarkInverse
frameworks/base/core/res/res/values/public.xml:489: warning: No comment for public symbol android:attr/toAlpha
frameworks/base/core/res/res/values/public.xml:466: warning: No comment for public symbol android:attr/toDegrees
frameworks/base/core/res/res/values/public.xml:485: warning: No comment for public symbol android:attr/toXDelta
frameworks/base/core/res/res/values/public.xml:481: warning: No comment for public symbol android:attr/toXScale
frameworks/base/core/res/res/values/public.xml:487: warning: No comment for public symbol android:attr/toYDelta
frameworks/base/core/res/res/values/public.xml:483: warning: No comment for public symbol android:attr/toYScale
frameworks/base/core/res/res/values/public.xml:231: warning: No comment for public symbol android:attr/topBright
frameworks/base/core/res/res/values/public.xml:227: warning: No comment for public symbol android:attr/topDark
frameworks/base/core/res/res/values/public.xml:2066: warning: No comment for public symbol android:attr/transitionOrdering
frameworks/base/core/res/res/values/public.xml:445: warning: No comment for public symbol android:attr/useLevel
frameworks/base/core/res/res/values/public.xml:1155: warning: No comment for public symbol android:attr/userVisible
frameworks/base/core/res/res/values/public.xml:725: warning: No comment for public symbol android:color/background_dark
frameworks/base/core/res/res/values/public.xml:726: warning: No comment for public symbol android:color/background_light
frameworks/base/core/res/res/values/public.xml:723: warning: No comment for public symbol android:color/black
frameworks/base/core/res/res/values/public.xml:711: warning: No comment for public symbol android:color/darker_gray
frameworks/base/core/res/res/values/public.xml:712: warning: No comment for public symbol android:color/primary_text_dark
frameworks/base/core/res/res/values/public.xml:713: warning: No comment for public symbol android:color/primary_text_dark_nodisable
frameworks/base/core/res/res/values/public.xml:714: warning: No comment for public symbol android:color/primary_text_light
frameworks/base/core/res/res/values/public.xml:715: warning: No comment for public symbol android:color/primary_text_light_nodisable
frameworks/base/core/res/res/values/public.xml:716: warning: No comment for public symbol android:color/secondary_text_dark
frameworks/base/core/res/res/values/public.xml:717: warning: No comment for public symbol android:color/secondary_text_dark_nodisable
frameworks/base/core/res/res/values/public.xml:718: warning: No comment for public symbol android:color/secondary_text_light
frameworks/base/core/res/res/values/public.xml:719: warning: No comment for public symbol android:color/secondary_text_light_nodisable
frameworks/base/core/res/res/values/public.xml:720: warning: No comment for public symbol android:color/tab_indicator_text
frameworks/base/core/res/res/values/public.xml:727: warning: No comment for public symbol android:color/tertiary_text_dark
frameworks/base/core/res/res/values/public.xml:728: warning: No comment for public symbol android:color/tertiary_text_light
frameworks/base/core/res/res/values/public.xml:724: warning: No comment for public symbol android:color/transparent
frameworks/base/core/res/res/values/public.xml:722: warning: No comment for public symbol android:color/white
frameworks/base/core/res/res/values/public.xml:721: warning: No comment for public symbol android:color/widget_edittext_dark
frameworks/base/core/res/res/values/public.xml:736: warning: No comment for public symbol android:drawable/alert_dark_frame
frameworks/base/core/res/res/values/public.xml:737: warning: No comment for public symbol android:drawable/alert_light_frame
frameworks/base/core/res/res/values/public.xml:738: warning: No comment for public symbol android:drawable/arrow_down_float
frameworks/base/core/res/res/values/public.xml:739: warning: No comment for public symbol android:drawable/arrow_up_float
frameworks/base/core/res/res/values/public.xml:893: warning: No comment for public symbol android:drawable/bottom_bar
frameworks/base/core/res/res/values/public.xml:740: warning: No comment for public symbol android:drawable/btn_default
frameworks/base/core/res/res/values/public.xml:741: warning: No comment for public symbol android:drawable/btn_default_small
frameworks/base/core/res/res/values/public.xml:759: warning: No comment for public symbol android:drawable/btn_dialog
frameworks/base/core/res/res/values/public.xml:742: warning: No comment for public symbol android:drawable/btn_dropdown
frameworks/base/core/res/res/values/public.xml:743: warning: No comment for public symbol android:drawable/btn_minus
frameworks/base/core/res/res/values/public.xml:744: warning: No comment for public symbol android:drawable/btn_plus
frameworks/base/core/res/res/values/public.xml:745: warning: No comment for public symbol android:drawable/btn_radio
frameworks/base/core/res/res/values/public.xml:746: warning: No comment for public symbol android:drawable/btn_star
frameworks/base/core/res/res/values/public.xml:747: warning: No comment for public symbol android:drawable/btn_star_big_off
frameworks/base/core/res/res/values/public.xml:748: warning: No comment for public symbol android:drawable/btn_star_big_on
frameworks/base/core/res/res/values/public.xml:750: warning: No comment for public symbol android:drawable/button_onoff_indicator_off
frameworks/base/core/res/res/values/public.xml:749: warning: No comment for public symbol android:drawable/button_onoff_indicator_on
frameworks/base/core/res/res/values/public.xml:751: warning: No comment for public symbol android:drawable/checkbox_off_background
frameworks/base/core/res/res/values/public.xml:752: warning: No comment for public symbol android:drawable/checkbox_on_background
frameworks/base/core/res/res/values/public.xml:753: warning: No comment for public symbol android:drawable/dialog_frame
frameworks/base/core/res/res/values/public.xml:1500: warning: No comment for public symbol android:drawable/dialog_holo_dark_frame
frameworks/base/core/res/res/values/public.xml:1501: warning: No comment for public symbol android:drawable/dialog_holo_light_frame
frameworks/base/core/res/res/values/public.xml:754: warning: No comment for public symbol android:drawable/divider_horizontal_bright
frameworks/base/core/res/res/values/public.xml:756: warning: No comment for public symbol android:drawable/divider_horizontal_dark
frameworks/base/core/res/res/values/public.xml:757: warning: No comment for public symbol android:drawable/divider_horizontal_dim_dark
frameworks/base/core/res/res/values/public.xml:755: warning: No comment for public symbol android:drawable/divider_horizontal_textfield
frameworks/base/core/res/res/values/public.xml:758: warning: No comment for public symbol android:drawable/edit_text
frameworks/base/core/res/res/values/public.xml:760: warning: No comment for public symbol android:drawable/editbox_background
frameworks/base/core/res/res/values/public.xml:761: warning: No comment for public symbol android:drawable/editbox_background_normal
frameworks/base/core/res/res/values/public.xml:762: warning: No comment for public symbol android:drawable/editbox_dropdown_dark_frame
frameworks/base/core/res/res/values/public.xml:763: warning: No comment for public symbol android:drawable/editbox_dropdown_light_frame
frameworks/base/core/res/res/values/public.xml:764: warning: No comment for public symbol android:drawable/gallery_thumb
frameworks/base/core/res/res/values/public.xml:1078: warning: No comment for public symbol android:drawable/ic_btn_speak_now
frameworks/base/core/res/res/values/public.xml:765: warning: No comment for public symbol android:drawable/ic_delete
frameworks/base/core/res/res/values/public.xml:775: warning: No comment for public symbol android:drawable/ic_dialog_alert
frameworks/base/core/res/res/values/public.xml:776: warning: No comment for public symbol android:drawable/ic_dialog_dialer
frameworks/base/core/res/res/values/public.xml:777: warning: No comment for public symbol android:drawable/ic_dialog_email
frameworks/base/core/res/res/values/public.xml:894: warning: No comment for public symbol android:drawable/ic_dialog_info
frameworks/base/core/res/res/values/public.xml:778: warning: No comment for public symbol android:drawable/ic_dialog_map
frameworks/base/core/res/res/values/public.xml:779: warning: No comment for public symbol android:drawable/ic_input_add
frameworks/base/core/res/res/values/public.xml:780: warning: No comment for public symbol android:drawable/ic_input_delete
frameworks/base/core/res/res/values/public.xml:781: warning: No comment for public symbol android:drawable/ic_input_get
frameworks/base/core/res/res/values/public.xml:782: warning: No comment for public symbol android:drawable/ic_lock_idle_alarm
frameworks/base/core/res/res/values/public.xml:766: warning: No comment for public symbol android:drawable/ic_lock_idle_charging
frameworks/base/core/res/res/values/public.xml:767: warning: No comment for public symbol android:drawable/ic_lock_idle_lock
frameworks/base/core/res/res/values/public.xml:768: warning: No comment for public symbol android:drawable/ic_lock_idle_low_battery
frameworks/base/core/res/res/values/public.xml:783: warning: No comment for public symbol android:drawable/ic_lock_lock
frameworks/base/core/res/res/values/public.xml:784: warning: No comment for public symbol android:drawable/ic_lock_power_off
frameworks/base/core/res/res/values/public.xml:785: warning: No comment for public symbol android:drawable/ic_lock_silent_mode
frameworks/base/core/res/res/values/public.xml:786: warning: No comment for public symbol android:drawable/ic_lock_silent_mode_off
frameworks/base/core/res/res/values/public.xml:769: warning: No comment for public symbol android:drawable/ic_media_ff
frameworks/base/core/res/res/values/public.xml:770: warning: No comment for public symbol android:drawable/ic_media_next
frameworks/base/core/res/res/values/public.xml:771: warning: No comment for public symbol android:drawable/ic_media_pause
frameworks/base/core/res/res/values/public.xml:772: warning: No comment for public symbol android:drawable/ic_media_play
frameworks/base/core/res/res/values/public.xml:773: warning: No comment for public symbol android:drawable/ic_media_previous
frameworks/base/core/res/res/values/public.xml:774: warning: No comment for public symbol android:drawable/ic_media_rew
frameworks/base/core/res/res/values/public.xml:787: warning: No comment for public symbol android:drawable/ic_menu_add
frameworks/base/core/res/res/values/public.xml:788: warning: No comment for public symbol android:drawable/ic_menu_agenda
frameworks/base/core/res/res/values/public.xml:789: warning: No comment for public symbol android:drawable/ic_menu_always_landscape_portrait
frameworks/base/core/res/res/values/public.xml:790: warning: No comment for public symbol android:drawable/ic_menu_call
frameworks/base/core/res/res/values/public.xml:791: warning: No comment for public symbol android:drawable/ic_menu_camera
frameworks/base/core/res/res/values/public.xml:792: warning: No comment for public symbol android:drawable/ic_menu_close_clear_cancel
frameworks/base/core/res/res/values/public.xml:793: warning: No comment for public symbol android:drawable/ic_menu_compass
frameworks/base/core/res/res/values/public.xml:794: warning: No comment for public symbol android:drawable/ic_menu_crop
frameworks/base/core/res/res/values/public.xml:795: warning: No comment for public symbol android:drawable/ic_menu_day
frameworks/base/core/res/res/values/public.xml:796: warning: No comment for public symbol android:drawable/ic_menu_delete
frameworks/base/core/res/res/values/public.xml:797: warning: No comment for public symbol android:drawable/ic_menu_directions
frameworks/base/core/res/res/values/public.xml:798: warning: No comment for public symbol android:drawable/ic_menu_edit
frameworks/base/core/res/res/values/public.xml:799: warning: No comment for public symbol android:drawable/ic_menu_gallery
frameworks/base/core/res/res/values/public.xml:800: warning: No comment for public symbol android:drawable/ic_menu_help
frameworks/base/core/res/res/values/public.xml:801: warning: No comment for public symbol android:drawable/ic_menu_info_details
frameworks/base/core/res/res/values/public.xml:802: warning: No comment for public symbol android:drawable/ic_menu_manage
frameworks/base/core/res/res/values/public.xml:803: warning: No comment for public symbol android:drawable/ic_menu_mapmode
frameworks/base/core/res/res/values/public.xml:804: warning: No comment for public symbol android:drawable/ic_menu_month
frameworks/base/core/res/res/values/public.xml:805: warning: No comment for public symbol android:drawable/ic_menu_more
frameworks/base/core/res/res/values/public.xml:806: warning: No comment for public symbol android:drawable/ic_menu_my_calendar
frameworks/base/core/res/res/values/public.xml:807: warning: No comment for public symbol android:drawable/ic_menu_mylocation
frameworks/base/core/res/res/values/public.xml:808: warning: No comment for public symbol android:drawable/ic_menu_myplaces
frameworks/base/core/res/res/values/public.xml:809: warning: No comment for public symbol android:drawable/ic_menu_preferences
frameworks/base/core/res/res/values/public.xml:810: warning: No comment for public symbol android:drawable/ic_menu_recent_history
frameworks/base/core/res/res/values/public.xml:811: warning: No comment for public symbol android:drawable/ic_menu_report_image
frameworks/base/core/res/res/values/public.xml:812: warning: No comment for public symbol android:drawable/ic_menu_revert
frameworks/base/core/res/res/values/public.xml:813: warning: No comment for public symbol android:drawable/ic_menu_rotate
frameworks/base/core/res/res/values/public.xml:814: warning: No comment for public symbol android:drawable/ic_menu_save
frameworks/base/core/res/res/values/public.xml:815: warning: No comment for public symbol android:drawable/ic_menu_search
frameworks/base/core/res/res/values/public.xml:816: warning: No comment for public symbol android:drawable/ic_menu_send
frameworks/base/core/res/res/values/public.xml:817: warning: No comment for public symbol android:drawable/ic_menu_set_as
frameworks/base/core/res/res/values/public.xml:818: warning: No comment for public symbol android:drawable/ic_menu_share
frameworks/base/core/res/res/values/public.xml:819: warning: No comment for public symbol android:drawable/ic_menu_slideshow
frameworks/base/core/res/res/values/public.xml:895: warning: No comment for public symbol android:drawable/ic_menu_sort_alphabetically
frameworks/base/core/res/res/values/public.xml:896: warning: No comment for public symbol android:drawable/ic_menu_sort_by_size
frameworks/base/core/res/res/values/public.xml:820: warning: No comment for public symbol android:drawable/ic_menu_today
frameworks/base/core/res/res/values/public.xml:821: warning: No comment for public symbol android:drawable/ic_menu_upload
frameworks/base/core/res/res/values/public.xml:822: warning: No comment for public symbol android:drawable/ic_menu_upload_you_tube
frameworks/base/core/res/res/values/public.xml:823: warning: No comment for public symbol android:drawable/ic_menu_view
frameworks/base/core/res/res/values/public.xml:824: warning: No comment for public symbol android:drawable/ic_menu_week
frameworks/base/core/res/res/values/public.xml:825: warning: No comment for public symbol android:drawable/ic_menu_zoom
frameworks/base/core/res/res/values/public.xml:826: warning: No comment for public symbol android:drawable/ic_notification_clear_all
frameworks/base/core/res/res/values/public.xml:827: warning: No comment for public symbol android:drawable/ic_notification_overlay
frameworks/base/core/res/res/values/public.xml:828: warning: No comment for public symbol android:drawable/ic_partial_secure
frameworks/base/core/res/res/values/public.xml:829: warning: No comment for public symbol android:drawable/ic_popup_disk_full
frameworks/base/core/res/res/values/public.xml:830: warning: No comment for public symbol android:drawable/ic_popup_reminder
frameworks/base/core/res/res/values/public.xml:831: warning: No comment for public symbol android:drawable/ic_popup_sync
frameworks/base/core/res/res/values/public.xml:832: warning: No comment for public symbol android:drawable/ic_search_category_default
frameworks/base/core/res/res/values/public.xml:833: warning: No comment for public symbol android:drawable/ic_secure
frameworks/base/core/res/res/values/public.xml:834: warning: No comment for public symbol android:drawable/list_selector_background
frameworks/base/core/res/res/values/public.xml:835: warning: No comment for public symbol android:drawable/menu_frame
frameworks/base/core/res/res/values/public.xml:836: warning: No comment for public symbol android:drawable/menu_full_frame
frameworks/base/core/res/res/values/public.xml:837: warning: No comment for public symbol android:drawable/menuitem_background
frameworks/base/core/res/res/values/public.xml:838: warning: No comment for public symbol android:drawable/picture_frame
frameworks/base/core/res/res/values/public.xml:1268: warning: No comment for public symbol android:drawable/presence_audio_away
frameworks/base/core/res/res/values/public.xml:1269: warning: No comment for public symbol android:drawable/presence_audio_busy
frameworks/base/core/res/res/values/public.xml:1270: warning: No comment for public symbol android:drawable/presence_audio_online
frameworks/base/core/res/res/values/public.xml:839: warning: No comment for public symbol android:drawable/presence_away
frameworks/base/core/res/res/values/public.xml:840: warning: No comment for public symbol android:drawable/presence_busy
frameworks/base/core/res/res/values/public.xml:841: warning: No comment for public symbol android:drawable/presence_invisible
frameworks/base/core/res/res/values/public.xml:842: warning: No comment for public symbol android:drawable/presence_offline
frameworks/base/core/res/res/values/public.xml:843: warning: No comment for public symbol android:drawable/presence_online
frameworks/base/core/res/res/values/public.xml:1266: warning: No comment for public symbol android:drawable/presence_video_busy
frameworks/base/core/res/res/values/public.xml:1267: warning: No comment for public symbol android:drawable/presence_video_online
frameworks/base/core/res/res/values/public.xml:844: warning: No comment for public symbol android:drawable/progress_horizontal
frameworks/base/core/res/res/values/public.xml:845: warning: No comment for public symbol android:drawable/progress_indeterminate_horizontal
frameworks/base/core/res/res/values/public.xml:846: warning: No comment for public symbol android:drawable/radiobutton_off_background
frameworks/base/core/res/res/values/public.xml:847: warning: No comment for public symbol android:drawable/radiobutton_on_background
frameworks/base/core/res/res/values/public.xml:891: warning: No comment for public symbol android:drawable/screen_background_dark
frameworks/base/core/res/res/values/public.xml:892: warning: No comment for public symbol android:drawable/screen_background_light
frameworks/base/core/res/res/values/public.xml:848: warning: No comment for public symbol android:drawable/spinner_background
frameworks/base/core/res/res/values/public.xml:849: warning: No comment for public symbol android:drawable/spinner_dropdown_background
frameworks/base/core/res/res/values/public.xml:851: warning: No comment for public symbol android:drawable/star_big_off
frameworks/base/core/res/res/values/public.xml:850: warning: No comment for public symbol android:drawable/star_big_on
frameworks/base/core/res/res/values/public.xml:853: warning: No comment for public symbol android:drawable/star_off
frameworks/base/core/res/res/values/public.xml:852: warning: No comment for public symbol android:drawable/star_on
frameworks/base/core/res/res/values/public.xml:854: warning: No comment for public symbol android:drawable/stat_notify_call_mute
frameworks/base/core/res/res/values/public.xml:855: warning: No comment for public symbol android:drawable/stat_notify_chat
frameworks/base/core/res/res/values/public.xml:856: warning: No comment for public symbol android:drawable/stat_notify_error
frameworks/base/core/res/res/values/public.xml:863: warning: No comment for public symbol android:drawable/stat_notify_missed_call
frameworks/base/core/res/res/values/public.xml:857: warning: No comment for public symbol android:drawable/stat_notify_more
frameworks/base/core/res/res/values/public.xml:858: warning: No comment for public symbol android:drawable/stat_notify_sdcard
frameworks/base/core/res/res/values/public.xml:1199: warning: No comment for public symbol android:drawable/stat_notify_sdcard_prepare
frameworks/base/core/res/res/values/public.xml:859: warning: No comment for public symbol android:drawable/stat_notify_sdcard_usb
frameworks/base/core/res/res/values/public.xml:860: warning: No comment for public symbol android:drawable/stat_notify_sync
frameworks/base/core/res/res/values/public.xml:861: warning: No comment for public symbol android:drawable/stat_notify_sync_noanim
frameworks/base/core/res/res/values/public.xml:862: warning: No comment for public symbol android:drawable/stat_notify_voicemail
frameworks/base/core/res/res/values/public.xml:864: warning: No comment for public symbol android:drawable/stat_sys_data_bluetooth
frameworks/base/core/res/res/values/public.xml:865: warning: No comment for public symbol android:drawable/stat_sys_download
frameworks/base/core/res/res/values/public.xml:866: warning: No comment for public symbol android:drawable/stat_sys_download_done
frameworks/base/core/res/res/values/public.xml:867: warning: No comment for public symbol android:drawable/stat_sys_headset
frameworks/base/core/res/res/values/public.xml:874: warning: No comment for public symbol android:drawable/stat_sys_speakerphone
frameworks/base/core/res/res/values/public.xml:875: warning: No comment for public symbol android:drawable/stat_sys_upload
frameworks/base/core/res/res/values/public.xml:876: warning: No comment for public symbol android:drawable/stat_sys_upload_done
frameworks/base/core/res/res/values/public.xml:877: warning: No comment for public symbol android:drawable/stat_sys_warning
frameworks/base/core/res/res/values/public.xml:878: warning: No comment for public symbol android:drawable/status_bar_item_app_background
frameworks/base/core/res/res/values/public.xml:879: warning: No comment for public symbol android:drawable/status_bar_item_background
frameworks/base/core/res/res/values/public.xml:880: warning: No comment for public symbol android:drawable/sym_action_call
frameworks/base/core/res/res/values/public.xml:881: warning: No comment for public symbol android:drawable/sym_action_chat
frameworks/base/core/res/res/values/public.xml:882: warning: No comment for public symbol android:drawable/sym_action_email
frameworks/base/core/res/res/values/public.xml:883: warning: No comment for public symbol android:drawable/sym_call_incoming
frameworks/base/core/res/res/values/public.xml:884: warning: No comment for public symbol android:drawable/sym_call_missed
frameworks/base/core/res/res/values/public.xml:885: warning: No comment for public symbol android:drawable/sym_call_outgoing
frameworks/base/core/res/res/values/public.xml:887: warning: No comment for public symbol android:drawable/sym_contact_card
frameworks/base/core/res/res/values/public.xml:886: warning: No comment for public symbol android:drawable/sym_def_app_icon
frameworks/base/core/res/res/values/public.xml:888: warning: No comment for public symbol android:drawable/title_bar
frameworks/base/core/res/res/values/public.xml:889: warning: No comment for public symbol android:drawable/toast_frame
frameworks/base/core/res/res/values/public.xml:890: warning: No comment for public symbol android:drawable/zoom_plate
frameworks/base/core/res/res/values/public.xml:572: warning: No comment for public symbol android:id/background
frameworks/base/core/res/res/values/public.xml:597: warning: No comment for public symbol android:id/button1
frameworks/base/core/res/res/values/public.xml:598: warning: No comment for public symbol android:id/button2
frameworks/base/core/res/res/values/public.xml:599: warning: No comment for public symbol android:id/button3
frameworks/base/core/res/res/values/public.xml:573: warning: No comment for public symbol android:id/checkbox
frameworks/base/core/res/res/values/public.xml:574: warning: No comment for public symbol android:id/content
frameworks/base/core/res/res/values/public.xml:1241: warning: No comment for public symbol android:id/custom
frameworks/base/core/res/res/values/public.xml:575: warning: No comment for public symbol android:id/edit
frameworks/base/core/res/res/values/public.xml:576: warning: No comment for public symbol android:id/empty
frameworks/base/core/res/res/values/public.xml:577: warning: No comment for public symbol android:id/hint
frameworks/base/core/res/res/values/public.xml:1470: warning: No comment for public symbol android:id/home
frameworks/base/core/res/res/values/public.xml:578: warning: No comment for public symbol android:id/icon
frameworks/base/core/res/res/values/public.xml:579: warning: No comment for public symbol android:id/icon1
frameworks/base/core/res/res/values/public.xml:580: warning: No comment for public symbol android:id/icon2
frameworks/base/core/res/res/values/public.xml:581: warning: No comment for public symbol android:id/input
frameworks/base/core/res/res/values/public.xml:582: warning: No comment for public symbol android:id/list
frameworks/base/core/res/res/values/public.xml:583: warning: No comment for public symbol android:id/message
frameworks/base/core/res/res/values/public.xml:584: warning: No comment for public symbol android:id/primary
frameworks/base/core/res/res/values/public.xml:585: warning: No comment for public symbol android:id/progress
frameworks/base/core/res/res/values/public.xml:587: warning: No comment for public symbol android:id/secondaryProgress
frameworks/base/core/res/res/values/public.xml:586: warning: No comment for public symbol android:id/selectedIcon
frameworks/base/core/res/res/values/public.xml:588: warning: No comment for public symbol android:id/summary
frameworks/base/core/res/res/values/public.xml:589: warning: No comment for public symbol android:id/tabcontent
frameworks/base/core/res/res/values/public.xml:590: warning: No comment for public symbol android:id/tabhost
frameworks/base/core/res/res/values/public.xml:591: warning: No comment for public symbol android:id/tabs
frameworks/base/core/res/res/values/public.xml:592: warning: No comment for public symbol android:id/text1
frameworks/base/core/res/res/values/public.xml:593: warning: No comment for public symbol android:id/text2
frameworks/base/core/res/res/values/public.xml:594: warning: No comment for public symbol android:id/title
frameworks/base/core/res/res/values/public.xml:595: warning: No comment for public symbol android:id/toggle
frameworks/base/core/res/res/values/public.xml:596: warning: No comment for public symbol android:id/widget_frame
frameworks/base/core/res/res/values/public.xml:898: warning: No comment for public symbol android:layout/activity_list_item
frameworks/base/core/res/res/values/public.xml:912: warning: No comment for public symbol android:layout/browser_link_context_header
frameworks/base/core/res/res/values/public.xml:899: warning: No comment for public symbol android:layout/expandable_list_content
frameworks/base/core/res/res/values/public.xml:900: warning: No comment for public symbol android:layout/preference_category
frameworks/base/core/res/res/values/public.xml:915: warning: No comment for public symbol android:layout/select_dialog_item
frameworks/base/core/res/res/values/public.xml:917: warning: No comment for public symbol android:layout/select_dialog_multichoice
frameworks/base/core/res/res/values/public.xml:916: warning: No comment for public symbol android:layout/select_dialog_singlechoice
frameworks/base/core/res/res/values/public.xml:908: warning: No comment for public symbol android:layout/simple_dropdown_item_1line
frameworks/base/core/res/res/values/public.xml:904: warning: No comment for public symbol android:layout/simple_expandable_list_item_1
frameworks/base/core/res/res/values/public.xml:905: warning: No comment for public symbol android:layout/simple_expandable_list_item_2
frameworks/base/core/res/res/values/public.xml:909: warning: No comment for public symbol android:layout/simple_gallery_item
frameworks/base/core/res/res/values/public.xml:901: warning: No comment for public symbol android:layout/simple_list_item_1
frameworks/base/core/res/res/values/public.xml:902: warning: No comment for public symbol android:layout/simple_list_item_2
frameworks/base/core/res/res/values/public.xml:903: warning: No comment for public symbol android:layout/simple_list_item_checked
frameworks/base/core/res/res/values/public.xml:914: warning: No comment for public symbol android:layout/simple_list_item_multiple_choice
frameworks/base/core/res/res/values/public.xml:913: warning: No comment for public symbol android:layout/simple_list_item_single_choice
frameworks/base/core/res/res/values/public.xml:907: warning: No comment for public symbol android:layout/simple_spinner_dropdown_item
frameworks/base/core/res/res/values/public.xml:906: warning: No comment for public symbol android:layout/simple_spinner_item
frameworks/base/core/res/res/values/public.xml:910: warning: No comment for public symbol android:layout/test_list_item
frameworks/base/core/res/res/values/public.xml:911: warning: No comment for public symbol android:layout/two_line_list_item
frameworks/base/core/res/res/values/public.xml:605: warning: No comment for public symbol android:style/Animation.Toast
frameworks/base/core/res/res/values/public.xml:1954: warning: No comment for public symbol android:style/DeviceDefault.ButtonBar.AlertDialog
frameworks/base/core/res/res/values/public.xml:1956: warning: No comment for public symbol android:style/DeviceDefault.Light.ButtonBar
frameworks/base/core/res/res/values/public.xml:1957: warning: No comment for public symbol android:style/DeviceDefault.Light.ButtonBar.AlertDialog
frameworks/base/core/res/res/values/public.xml:1958: warning: No comment for public symbol android:style/DeviceDefault.Light.SegmentedButton
frameworks/base/core/res/res/values/public.xml:1955: warning: No comment for public symbol android:style/DeviceDefault.SegmentedButton
frameworks/base/core/res/res/values/public.xml:1627: warning: No comment for public symbol android:style/Holo.ButtonBar
frameworks/base/core/res/res/values/public.xml:1629: warning: No comment for public symbol android:style/Holo.ButtonBar.AlertDialog
frameworks/base/core/res/res/values/public.xml:1628: warning: No comment for public symbol android:style/Holo.Light.ButtonBar
frameworks/base/core/res/res/values/public.xml:1630: warning: No comment for public symbol android:style/Holo.Light.ButtonBar.AlertDialog
frameworks/base/core/res/res/values/public.xml:1632: warning: No comment for public symbol android:style/Holo.Light.SegmentedButton
frameworks/base/core/res/res/values/public.xml:1631: warning: No comment for public symbol android:style/Holo.SegmentedButton
frameworks/base/core/res/res/values/public.xml:656: warning: No comment for public symbol android:style/MediaButton
frameworks/base/core/res/res/values/public.xml:660: warning: No comment for public symbol android:style/MediaButton.Ffwd
frameworks/base/core/res/res/values/public.xml:658: warning: No comment for public symbol android:style/MediaButton.Next
frameworks/base/core/res/res/values/public.xml:662: warning: No comment for public symbol android:style/MediaButton.Pause
frameworks/base/core/res/res/values/public.xml:659: warning: No comment for public symbol android:style/MediaButton.Play
frameworks/base/core/res/res/values/public.xml:657: warning: No comment for public symbol android:style/MediaButton.Previous
frameworks/base/core/res/res/values/public.xml:661: warning: No comment for public symbol android:style/MediaButton.Rew
frameworks/base/core/res/res/values/public.xml:663: warning: No comment for public symbol android:style/TextAppearance
frameworks/base/core/res/res/values/public.xml:1930: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.DialogWindowTitle
frameworks/base/core/res/res/values/public.xml:1920: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Inverse
frameworks/base/core/res/res/values/public.xml:1921: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Large
frameworks/base/core/res/res/values/public.xml:1922: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Large.Inverse
frameworks/base/core/res/res/values/public.xml:1923: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Medium
frameworks/base/core/res/res/values/public.xml:1924: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Medium.Inverse
frameworks/base/core/res/res/values/public.xml:1928: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.SearchResult.Subtitle
frameworks/base/core/res/res/values/public.xml:1927: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.SearchResult.Title
frameworks/base/core/res/res/values/public.xml:1925: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Small
frameworks/base/core/res/res/values/public.xml:1926: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Small.Inverse
frameworks/base/core/res/res/values/public.xml:1931: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget
frameworks/base/core/res/res/values/public.xml:1952: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionBar.Menu
frameworks/base/core/res/res/values/public.xml:1945: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionBar.Subtitle
frameworks/base/core/res/res/values/public.xml:1949: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionBar.Subtitle.Inverse
frameworks/base/core/res/res/values/public.xml:1944: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionBar.Title
frameworks/base/core/res/res/values/public.xml:1948: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionBar.Title.Inverse
frameworks/base/core/res/res/values/public.xml:1947: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionMode.Subtitle
frameworks/base/core/res/res/values/public.xml:1951: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionMode.Subtitle.Inverse
frameworks/base/core/res/res/values/public.xml:1946: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionMode.Title
frameworks/base/core/res/res/values/public.xml:1950: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.ActionMode.Title.Inverse
frameworks/base/core/res/res/values/public.xml:1932: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.Button
frameworks/base/core/res/res/values/public.xml:1937: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.DropDownHint
frameworks/base/core/res/res/values/public.xml:1938: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.DropDownItem
frameworks/base/core/res/res/values/public.xml:1940: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.EditText
frameworks/base/core/res/res/values/public.xml:1933: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.IconMenu.Item
frameworks/base/core/res/res/values/public.xml:1941: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.PopupMenu
frameworks/base/core/res/res/values/public.xml:1942: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.PopupMenu.Large
frameworks/base/core/res/res/values/public.xml:1943: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.PopupMenu.Small
frameworks/base/core/res/res/values/public.xml:1934: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.TabWidget
frameworks/base/core/res/res/values/public.xml:1935: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.TextView
frameworks/base/core/res/res/values/public.xml:1936: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.TextView.PopupMenu
frameworks/base/core/res/res/values/public.xml:1939: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.Widget.TextView.SpinnerItem
frameworks/base/core/res/res/values/public.xml:1929: warning: No comment for public symbol android:style/TextAppearance.DeviceDefault.WindowTitle
frameworks/base/core/res/res/values/public.xml:666: warning: No comment for public symbol android:style/TextAppearance.DialogWindowTitle
frameworks/base/core/res/res/values/public.xml:1699: warning: No comment for public symbol android:style/TextAppearance.Holo.DialogWindowTitle
frameworks/base/core/res/res/values/public.xml:1672: warning: No comment for public symbol android:style/TextAppearance.Holo.Inverse
frameworks/base/core/res/res/values/public.xml:1673: warning: No comment for public symbol android:style/TextAppearance.Holo.Large
frameworks/base/core/res/res/values/public.xml:1674: warning: No comment for public symbol android:style/TextAppearance.Holo.Large.Inverse
frameworks/base/core/res/res/values/public.xml:1675: warning: No comment for public symbol android:style/TextAppearance.Holo.Medium
frameworks/base/core/res/res/values/public.xml:1676: warning: No comment for public symbol android:style/TextAppearance.Holo.Medium.Inverse
frameworks/base/core/res/res/values/public.xml:1680: warning: No comment for public symbol android:style/TextAppearance.Holo.SearchResult.Subtitle
frameworks/base/core/res/res/values/public.xml:1679: warning: No comment for public symbol android:style/TextAppearance.Holo.SearchResult.Title
frameworks/base/core/res/res/values/public.xml:1677: warning: No comment for public symbol android:style/TextAppearance.Holo.Small
frameworks/base/core/res/res/values/public.xml:1678: warning: No comment for public symbol android:style/TextAppearance.Holo.Small.Inverse
frameworks/base/core/res/res/values/public.xml:1681: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget
frameworks/base/core/res/res/values/public.xml:1778: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionBar.Menu
frameworks/base/core/res/res/values/public.xml:1695: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionBar.Subtitle
frameworks/base/core/res/res/values/public.xml:1775: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionBar.Subtitle.Inverse
frameworks/base/core/res/res/values/public.xml:1694: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionBar.Title
frameworks/base/core/res/res/values/public.xml:1774: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionBar.Title.Inverse
frameworks/base/core/res/res/values/public.xml:1697: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionMode.Subtitle
frameworks/base/core/res/res/values/public.xml:1777: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionMode.Subtitle.Inverse
frameworks/base/core/res/res/values/public.xml:1696: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionMode.Title
frameworks/base/core/res/res/values/public.xml:1776: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.ActionMode.Title.Inverse
frameworks/base/core/res/res/values/public.xml:1682: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.Button
frameworks/base/core/res/res/values/public.xml:1687: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.DropDownHint
frameworks/base/core/res/res/values/public.xml:1688: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.DropDownItem
frameworks/base/core/res/res/values/public.xml:1690: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.EditText
frameworks/base/core/res/res/values/public.xml:1683: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.IconMenu.Item
frameworks/base/core/res/res/values/public.xml:1691: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.PopupMenu
frameworks/base/core/res/res/values/public.xml:1692: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.PopupMenu.Large
frameworks/base/core/res/res/values/public.xml:1693: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.PopupMenu.Small
frameworks/base/core/res/res/values/public.xml:1685: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.TextView
frameworks/base/core/res/res/values/public.xml:1686: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.TextView.PopupMenu
frameworks/base/core/res/res/values/public.xml:1689: warning: No comment for public symbol android:style/TextAppearance.Holo.Widget.TextView.SpinnerItem
frameworks/base/core/res/res/values/public.xml:1698: warning: No comment for public symbol android:style/TextAppearance.Holo.WindowTitle
frameworks/base/core/res/res/values/public.xml:664: warning: No comment for public symbol android:style/TextAppearance.Inverse
frameworks/base/core/res/res/values/public.xml:667: warning: No comment for public symbol android:style/TextAppearance.Large
frameworks/base/core/res/res/values/public.xml:668: warning: No comment for public symbol android:style/TextAppearance.Large.Inverse
frameworks/base/core/res/res/values/public.xml:669: warning: No comment for public symbol android:style/TextAppearance.Medium
frameworks/base/core/res/res/values/public.xml:670: warning: No comment for public symbol android:style/TextAppearance.Medium.Inverse
frameworks/base/core/res/res/values/public.xml:671: warning: No comment for public symbol android:style/TextAppearance.Small
frameworks/base/core/res/res/values/public.xml:672: warning: No comment for public symbol android:style/TextAppearance.Small.Inverse
frameworks/base/core/res/res/values/public.xml:1275: warning: No comment for public symbol android:style/TextAppearance.StatusBar.EventContent.Title
frameworks/base/core/res/res/values/public.xml:1273: warning: No comment for public symbol android:style/TextAppearance.StatusBar.Icon
frameworks/base/core/res/res/values/public.xml:1272: warning: No comment for public symbol android:style/TextAppearance.StatusBar.Title
frameworks/base/core/res/res/values/public.xml:1770: warning: No comment for public symbol android:style/TextAppearance.SuggestionHighlight
frameworks/base/core/res/res/values/public.xml:665: warning: No comment for public symbol android:style/TextAppearance.Theme
frameworks/base/core/res/res/values/public.xml:673: warning: No comment for public symbol android:style/TextAppearance.Theme.Dialog
frameworks/base/core/res/res/values/public.xml:674: warning: No comment for public symbol android:style/TextAppearance.Widget
frameworks/base/core/res/res/values/public.xml:675: warning: No comment for public symbol android:style/TextAppearance.Widget.Button
frameworks/base/core/res/res/values/public.xml:681: warning: No comment for public symbol android:style/TextAppearance.Widget.DropDownHint
frameworks/base/core/res/res/values/public.xml:682: warning: No comment for public symbol android:style/TextAppearance.Widget.DropDownItem
frameworks/base/core/res/res/values/public.xml:677: warning: No comment for public symbol android:style/TextAppearance.Widget.EditText
frameworks/base/core/res/res/values/public.xml:676: warning: No comment for public symbol android:style/TextAppearance.Widget.IconMenu.Item
frameworks/base/core/res/res/values/public.xml:1526: warning: No comment for public symbol android:style/TextAppearance.Widget.PopupMenu.Large
frameworks/base/core/res/res/values/public.xml:1527: warning: No comment for public symbol android:style/TextAppearance.Widget.PopupMenu.Small
frameworks/base/core/res/res/values/public.xml:678: warning: No comment for public symbol android:style/TextAppearance.Widget.TabWidget
frameworks/base/core/res/res/values/public.xml:679: warning: No comment for public symbol android:style/TextAppearance.Widget.TextView
frameworks/base/core/res/res/values/public.xml:680: warning: No comment for public symbol android:style/TextAppearance.Widget.TextView.PopupMenu
frameworks/base/core/res/res/values/public.xml:683: warning: No comment for public symbol android:style/TextAppearance.Widget.TextView.SpinnerItem
frameworks/base/core/res/res/values/public.xml:684: warning: No comment for public symbol android:style/TextAppearance.WindowTitle
frameworks/base/core/res/res/values/public.xml:620: warning: No comment for public symbol android:style/Widget.AbsListView
frameworks/base/core/res/res/values/public.xml:1528: warning: No comment for public symbol android:style/Widget.ActionBar
frameworks/base/core/res/res/values/public.xml:1664: warning: No comment for public symbol android:style/Widget.ActionBar.TabBar
frameworks/base/core/res/res/values/public.xml:1663: warning: No comment for public symbol android:style/Widget.ActionBar.TabText
frameworks/base/core/res/res/values/public.xml:1662: warning: No comment for public symbol android:style/Widget.ActionBar.TabView
frameworks/base/core/res/res/values/public.xml:1530: warning: No comment for public symbol android:style/Widget.ActionButton
frameworks/base/core/res/res/values/public.xml:1534: warning: No comment for public symbol android:style/Widget.ActionButton.CloseMode
frameworks/base/core/res/res/values/public.xml:1533: warning: No comment for public symbol android:style/Widget.ActionButton.Overflow
frameworks/base/core/res/res/values/public.xml:640: warning: No comment for public symbol android:style/Widget.AutoCompleteTextView
frameworks/base/core/res/res/values/public.xml:621: warning: No comment for public symbol android:style/Widget.Button
frameworks/base/core/res/res/values/public.xml:622: warning: No comment for public symbol android:style/Widget.Button.Inset
frameworks/base/core/res/res/values/public.xml:623: warning: No comment for public symbol android:style/Widget.Button.Small
frameworks/base/core/res/res/values/public.xml:624: warning: No comment for public symbol android:style/Widget.Button.Toggle
frameworks/base/core/res/res/values/public.xml:1633: warning: No comment for public symbol android:style/Widget.CalendarView
frameworks/base/core/res/res/values/public.xml:625: warning: No comment for public symbol android:style/Widget.CompoundButton
frameworks/base/core/res/res/values/public.xml:626: warning: No comment for public symbol android:style/Widget.CompoundButton.CheckBox
frameworks/base/core/res/res/values/public.xml:627: warning: No comment for public symbol android:style/Widget.CompoundButton.RadioButton
frameworks/base/core/res/res/values/public.xml:628: warning: No comment for public symbol android:style/Widget.CompoundButton.Star
frameworks/base/core/res/res/values/public.xml:1636: warning: No comment for public symbol android:style/Widget.DatePicker
frameworks/base/core/res/res/values/public.xml:1853: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionBar
frameworks/base/core/res/res/values/public.xml:1861: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionBar.Solid
frameworks/base/core/res/res/values/public.xml:1860: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionBar.TabBar
frameworks/base/core/res/res/values/public.xml:1859: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionBar.TabText
frameworks/base/core/res/res/values/public.xml:1858: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionBar.TabView
frameworks/base/core/res/res/values/public.xml:1848: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionButton
frameworks/base/core/res/res/values/public.xml:1852: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionButton.CloseMode
frameworks/base/core/res/res/values/public.xml:1849: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionButton.Overflow
frameworks/base/core/res/res/values/public.xml:1850: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionButton.TextButton
frameworks/base/core/res/res/values/public.xml:1851: warning: No comment for public symbol android:style/Widget.DeviceDefault.ActionMode
frameworks/base/core/res/res/values/public.xml:1817: warning: No comment for public symbol android:style/Widget.DeviceDefault.AutoCompleteTextView
frameworks/base/core/res/res/values/public.xml:1811: warning: No comment for public symbol android:style/Widget.DeviceDefault.Button
frameworks/base/core/res/res/values/public.xml:1854: warning: No comment for public symbol android:style/Widget.DeviceDefault.Button.Borderless
frameworks/base/core/res/res/values/public.xml:1815: warning: No comment for public symbol android:style/Widget.DeviceDefault.Button.Borderless.Small
frameworks/base/core/res/res/values/public.xml:1813: warning: No comment for public symbol android:style/Widget.DeviceDefault.Button.Inset
frameworks/base/core/res/res/values/public.xml:1812: warning: No comment for public symbol android:style/Widget.DeviceDefault.Button.Small
frameworks/base/core/res/res/values/public.xml:1814: warning: No comment for public symbol android:style/Widget.DeviceDefault.Button.Toggle
frameworks/base/core/res/res/values/public.xml:1856: warning: No comment for public symbol android:style/Widget.DeviceDefault.CalendarView
frameworks/base/core/res/res/values/public.xml:2028: warning: No comment for public symbol android:style/Widget.DeviceDefault.CheckedTextView
frameworks/base/core/res/res/values/public.xml:1818: warning: No comment for public symbol android:style/Widget.DeviceDefault.CompoundButton.CheckBox
frameworks/base/core/res/res/values/public.xml:1835: warning: No comment for public symbol android:style/Widget.DeviceDefault.CompoundButton.RadioButton
frameworks/base/core/res/res/values/public.xml:1839: warning: No comment for public symbol android:style/Widget.DeviceDefault.CompoundButton.Star
frameworks/base/core/res/res/values/public.xml:1857: warning: No comment for public symbol android:style/Widget.DeviceDefault.DatePicker
frameworks/base/core/res/res/values/public.xml:1843: warning: No comment for public symbol android:style/Widget.DeviceDefault.DropDownItem
frameworks/base/core/res/res/values/public.xml:1844: warning: No comment for public symbol android:style/Widget.DeviceDefault.DropDownItem.Spinner
frameworks/base/core/res/res/values/public.xml:1820: warning: No comment for public symbol android:style/Widget.DeviceDefault.EditText
frameworks/base/core/res/res/values/public.xml:1821: warning: No comment for public symbol android:style/Widget.DeviceDefault.ExpandableListView
frameworks/base/core/res/res/values/public.xml:1822: warning: No comment for public symbol android:style/Widget.DeviceDefault.GridView
frameworks/base/core/res/res/values/public.xml:1837: warning: No comment for public symbol android:style/Widget.DeviceDefault.HorizontalScrollView
frameworks/base/core/res/res/values/public.xml:1823: warning: No comment for public symbol android:style/Widget.DeviceDefault.ImageButton
frameworks/base/core/res/res/values/public.xml:1862: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light
frameworks/base/core/res/res/values/public.xml:1909: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar
frameworks/base/core/res/res/values/public.xml:1913: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar.Solid
frameworks/base/core/res/res/values/public.xml:1914: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar.Solid.Inverse
frameworks/base/core/res/res/values/public.xml:1912: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar.TabBar
frameworks/base/core/res/res/values/public.xml:1915: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar.TabBar.Inverse
frameworks/base/core/res/res/values/public.xml:1911: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar.TabText
frameworks/base/core/res/res/values/public.xml:1917: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar.TabText.Inverse
frameworks/base/core/res/res/values/public.xml:1910: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar.TabView
frameworks/base/core/res/res/values/public.xml:1916: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionBar.TabView.Inverse
frameworks/base/core/res/res/values/public.xml:1905: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionButton
frameworks/base/core/res/res/values/public.xml:1908: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionButton.CloseMode
frameworks/base/core/res/res/values/public.xml:1906: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionButton.Overflow
frameworks/base/core/res/res/values/public.xml:1907: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionMode
frameworks/base/core/res/res/values/public.xml:1918: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ActionMode.Inverse
frameworks/base/core/res/res/values/public.xml:1869: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.AutoCompleteTextView
frameworks/base/core/res/res/values/public.xml:1863: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.Button
frameworks/base/core/res/res/values/public.xml:1867: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.Button.Borderless.Small
frameworks/base/core/res/res/values/public.xml:1865: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.Button.Inset
frameworks/base/core/res/res/values/public.xml:1864: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.Button.Small
frameworks/base/core/res/res/values/public.xml:1866: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.Button.Toggle
frameworks/base/core/res/res/values/public.xml:1904: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.CalendarView
frameworks/base/core/res/res/values/public.xml:2029: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.CheckedTextView
frameworks/base/core/res/res/values/public.xml:1870: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.CompoundButton.CheckBox
frameworks/base/core/res/res/values/public.xml:1890: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.CompoundButton.RadioButton
frameworks/base/core/res/res/values/public.xml:1894: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.CompoundButton.Star
frameworks/base/core/res/res/values/public.xml:1898: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.DropDownItem
frameworks/base/core/res/res/values/public.xml:1899: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.DropDownItem.Spinner
frameworks/base/core/res/res/values/public.xml:1872: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.EditText
frameworks/base/core/res/res/values/public.xml:1873: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ExpandableListView
frameworks/base/core/res/res/values/public.xml:1874: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.GridView
frameworks/base/core/res/res/values/public.xml:1892: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.HorizontalScrollView
frameworks/base/core/res/res/values/public.xml:1875: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ImageButton
frameworks/base/core/res/res/values/public.xml:1901: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ListPopupWindow
frameworks/base/core/res/res/values/public.xml:1876: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ListView
frameworks/base/core/res/res/values/public.xml:1871: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ListView.DropDown
frameworks/base/core/res/res/values/public.xml:1990: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.MediaRouteButton
frameworks/base/core/res/res/values/public.xml:1902: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.PopupMenu
frameworks/base/core/res/res/values/public.xml:1877: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.PopupWindow
frameworks/base/core/res/res/values/public.xml:1878: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ProgressBar
frameworks/base/core/res/res/values/public.xml:1879: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ProgressBar.Horizontal
frameworks/base/core/res/res/values/public.xml:1883: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ProgressBar.Inverse
frameworks/base/core/res/res/values/public.xml:1882: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ProgressBar.Large
frameworks/base/core/res/res/values/public.xml:1885: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ProgressBar.Large.Inverse
frameworks/base/core/res/res/values/public.xml:1880: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ProgressBar.Small
frameworks/base/core/res/res/values/public.xml:1884: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ProgressBar.Small.Inverse
frameworks/base/core/res/res/values/public.xml:1881: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ProgressBar.Small.Title
frameworks/base/core/res/res/values/public.xml:1887: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.RatingBar
frameworks/base/core/res/res/values/public.xml:1888: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.RatingBar.Indicator
frameworks/base/core/res/res/values/public.xml:1889: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.RatingBar.Small
frameworks/base/core/res/res/values/public.xml:1891: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.ScrollView
frameworks/base/core/res/res/values/public.xml:1886: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.SeekBar
frameworks/base/core/res/res/values/public.xml:1893: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.Spinner
frameworks/base/core/res/res/values/public.xml:1903: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.Tab
frameworks/base/core/res/res/values/public.xml:1895: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.TabWidget
frameworks/base/core/res/res/values/public.xml:1868: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.TextView
frameworks/base/core/res/res/values/public.xml:1900: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.TextView.SpinnerItem
frameworks/base/core/res/res/values/public.xml:1896: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.WebTextView
frameworks/base/core/res/res/values/public.xml:1897: warning: No comment for public symbol android:style/Widget.DeviceDefault.Light.WebView
frameworks/base/core/res/res/values/public.xml:1846: warning: No comment for public symbol android:style/Widget.DeviceDefault.ListPopupWindow
frameworks/base/core/res/res/values/public.xml:1824: warning: No comment for public symbol android:style/Widget.DeviceDefault.ListView
frameworks/base/core/res/res/values/public.xml:1819: warning: No comment for public symbol android:style/Widget.DeviceDefault.ListView.DropDown
frameworks/base/core/res/res/values/public.xml:1989: warning: No comment for public symbol android:style/Widget.DeviceDefault.MediaRouteButton
frameworks/base/core/res/res/values/public.xml:1847: warning: No comment for public symbol android:style/Widget.DeviceDefault.PopupMenu
frameworks/base/core/res/res/values/public.xml:1825: warning: No comment for public symbol android:style/Widget.DeviceDefault.PopupWindow
frameworks/base/core/res/res/values/public.xml:1826: warning: No comment for public symbol android:style/Widget.DeviceDefault.ProgressBar
frameworks/base/core/res/res/values/public.xml:1827: warning: No comment for public symbol android:style/Widget.DeviceDefault.ProgressBar.Horizontal
frameworks/base/core/res/res/values/public.xml:1830: warning: No comment for public symbol android:style/Widget.DeviceDefault.ProgressBar.Large
frameworks/base/core/res/res/values/public.xml:1828: warning: No comment for public symbol android:style/Widget.DeviceDefault.ProgressBar.Small
frameworks/base/core/res/res/values/public.xml:1829: warning: No comment for public symbol android:style/Widget.DeviceDefault.ProgressBar.Small.Title
frameworks/base/core/res/res/values/public.xml:1832: warning: No comment for public symbol android:style/Widget.DeviceDefault.RatingBar
frameworks/base/core/res/res/values/public.xml:1833: warning: No comment for public symbol android:style/Widget.DeviceDefault.RatingBar.Indicator
frameworks/base/core/res/res/values/public.xml:1834: warning: No comment for public symbol android:style/Widget.DeviceDefault.RatingBar.Small
frameworks/base/core/res/res/values/public.xml:1836: warning: No comment for public symbol android:style/Widget.DeviceDefault.ScrollView
frameworks/base/core/res/res/values/public.xml:1831: warning: No comment for public symbol android:style/Widget.DeviceDefault.SeekBar
frameworks/base/core/res/res/values/public.xml:1838: warning: No comment for public symbol android:style/Widget.DeviceDefault.Spinner
frameworks/base/core/res/res/values/public.xml:1855: warning: No comment for public symbol android:style/Widget.DeviceDefault.Tab
frameworks/base/core/res/res/values/public.xml:1840: warning: No comment for public symbol android:style/Widget.DeviceDefault.TabWidget
frameworks/base/core/res/res/values/public.xml:1816: warning: No comment for public symbol android:style/Widget.DeviceDefault.TextView
frameworks/base/core/res/res/values/public.xml:1845: warning: No comment for public symbol android:style/Widget.DeviceDefault.TextView.SpinnerItem
frameworks/base/core/res/res/values/public.xml:1841: warning: No comment for public symbol android:style/Widget.DeviceDefault.WebTextView
frameworks/base/core/res/res/values/public.xml:1842: warning: No comment for public symbol android:style/Widget.DeviceDefault.WebView
frameworks/base/core/res/res/values/public.xml:644: warning: No comment for public symbol android:style/Widget.DropDownItem
frameworks/base/core/res/res/values/public.xml:645: warning: No comment for public symbol android:style/Widget.DropDownItem.Spinner
frameworks/base/core/res/res/values/public.xml:636: warning: No comment for public symbol android:style/Widget.EditText
frameworks/base/core/res/res/values/public.xml:637: warning: No comment for public symbol android:style/Widget.ExpandableListView
frameworks/base/core/res/res/values/public.xml:654: warning: No comment for public symbol android:style/Widget.Gallery
frameworks/base/core/res/res/values/public.xml:651: warning: No comment for public symbol android:style/Widget.GridView
frameworks/base/core/res/res/values/public.xml:1578: warning: No comment for public symbol android:style/Widget.Holo.ActionBar
frameworks/base/core/res/res/values/public.xml:1779: warning: No comment for public symbol android:style/Widget.Holo.ActionBar.Solid
frameworks/base/core/res/res/values/public.xml:1667: warning: No comment for public symbol android:style/Widget.Holo.ActionBar.TabBar
frameworks/base/core/res/res/values/public.xml:1666: warning: No comment for public symbol android:style/Widget.Holo.ActionBar.TabText
frameworks/base/core/res/res/values/public.xml:1665: warning: No comment for public symbol android:style/Widget.Holo.ActionBar.TabView
frameworks/base/core/res/res/values/public.xml:1573: warning: No comment for public symbol android:style/Widget.Holo.ActionButton
frameworks/base/core/res/res/values/public.xml:1577: warning: No comment for public symbol android:style/Widget.Holo.ActionButton.CloseMode
frameworks/base/core/res/res/values/public.xml:1574: warning: No comment for public symbol android:style/Widget.Holo.ActionButton.Overflow
frameworks/base/core/res/res/values/public.xml:1575: warning: No comment for public symbol android:style/Widget.Holo.ActionButton.TextButton
frameworks/base/core/res/res/values/public.xml:1576: warning: No comment for public symbol android:style/Widget.Holo.ActionMode
frameworks/base/core/res/res/values/public.xml:1542: warning: No comment for public symbol android:style/Widget.Holo.AutoCompleteTextView
frameworks/base/core/res/res/values/public.xml:1537: warning: No comment for public symbol android:style/Widget.Holo.Button
frameworks/base/core/res/res/values/public.xml:1624: warning: No comment for public symbol android:style/Widget.Holo.Button.Borderless
frameworks/base/core/res/res/values/public.xml:1772: warning: No comment for public symbol android:style/Widget.Holo.Button.Borderless.Small
frameworks/base/core/res/res/values/public.xml:1539: warning: No comment for public symbol android:style/Widget.Holo.Button.Inset
frameworks/base/core/res/res/values/public.xml:1538: warning: No comment for public symbol android:style/Widget.Holo.Button.Small
frameworks/base/core/res/res/values/public.xml:1540: warning: No comment for public symbol android:style/Widget.Holo.Button.Toggle
frameworks/base/core/res/res/values/public.xml:1634: warning: No comment for public symbol android:style/Widget.Holo.CalendarView
frameworks/base/core/res/res/values/public.xml:2026: warning: No comment for public symbol android:style/Widget.Holo.CheckedTextView
frameworks/base/core/res/res/values/public.xml:1543: warning: No comment for public symbol android:style/Widget.Holo.CompoundButton.CheckBox
frameworks/base/core/res/res/values/public.xml:1560: warning: No comment for public symbol android:style/Widget.Holo.CompoundButton.RadioButton
frameworks/base/core/res/res/values/public.xml:1564: warning: No comment for public symbol android:style/Widget.Holo.CompoundButton.Star
frameworks/base/core/res/res/values/public.xml:1637: warning: No comment for public symbol android:style/Widget.Holo.DatePicker
frameworks/base/core/res/res/values/public.xml:1568: warning: No comment for public symbol android:style/Widget.Holo.DropDownItem
frameworks/base/core/res/res/values/public.xml:1569: warning: No comment for public symbol android:style/Widget.Holo.DropDownItem.Spinner
frameworks/base/core/res/res/values/public.xml:1545: warning: No comment for public symbol android:style/Widget.Holo.EditText
frameworks/base/core/res/res/values/public.xml:1546: warning: No comment for public symbol android:style/Widget.Holo.ExpandableListView
frameworks/base/core/res/res/values/public.xml:1547: warning: No comment for public symbol android:style/Widget.Holo.GridView
frameworks/base/core/res/res/values/public.xml:1562: warning: No comment for public symbol android:style/Widget.Holo.HorizontalScrollView
frameworks/base/core/res/res/values/public.xml:1548: warning: No comment for public symbol android:style/Widget.Holo.ImageButton
frameworks/base/core/res/res/values/public.xml:1623: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar
frameworks/base/core/res/res/values/public.xml:1780: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar.Solid
frameworks/base/core/res/res/values/public.xml:1781: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar.Solid.Inverse
frameworks/base/core/res/res/values/public.xml:1670: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar.TabBar
frameworks/base/core/res/res/values/public.xml:1782: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar.TabBar.Inverse
frameworks/base/core/res/res/values/public.xml:1669: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar.TabText
frameworks/base/core/res/res/values/public.xml:1784: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar.TabText.Inverse
frameworks/base/core/res/res/values/public.xml:1668: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar.TabView
frameworks/base/core/res/res/values/public.xml:1783: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionBar.TabView.Inverse
frameworks/base/core/res/res/values/public.xml:1619: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionButton
frameworks/base/core/res/res/values/public.xml:1622: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionButton.CloseMode
frameworks/base/core/res/res/values/public.xml:1620: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionButton.Overflow
frameworks/base/core/res/res/values/public.xml:1621: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionMode
frameworks/base/core/res/res/values/public.xml:1785: warning: No comment for public symbol android:style/Widget.Holo.Light.ActionMode.Inverse
frameworks/base/core/res/res/values/public.xml:1585: warning: No comment for public symbol android:style/Widget.Holo.Light.AutoCompleteTextView
frameworks/base/core/res/res/values/public.xml:1580: warning: No comment for public symbol android:style/Widget.Holo.Light.Button
frameworks/base/core/res/res/values/public.xml:1773: warning: No comment for public symbol android:style/Widget.Holo.Light.Button.Borderless.Small
frameworks/base/core/res/res/values/public.xml:1582: warning: No comment for public symbol android:style/Widget.Holo.Light.Button.Inset
frameworks/base/core/res/res/values/public.xml:1581: warning: No comment for public symbol android:style/Widget.Holo.Light.Button.Small
frameworks/base/core/res/res/values/public.xml:1583: warning: No comment for public symbol android:style/Widget.Holo.Light.Button.Toggle
frameworks/base/core/res/res/values/public.xml:1635: warning: No comment for public symbol android:style/Widget.Holo.Light.CalendarView
frameworks/base/core/res/res/values/public.xml:2027: warning: No comment for public symbol android:style/Widget.Holo.Light.CheckedTextView
frameworks/base/core/res/res/values/public.xml:1586: warning: No comment for public symbol android:style/Widget.Holo.Light.CompoundButton.CheckBox
frameworks/base/core/res/res/values/public.xml:1606: warning: No comment for public symbol android:style/Widget.Holo.Light.CompoundButton.RadioButton
frameworks/base/core/res/res/values/public.xml:1610: warning: No comment for public symbol android:style/Widget.Holo.Light.CompoundButton.Star
frameworks/base/core/res/res/values/public.xml:1614: warning: No comment for public symbol android:style/Widget.Holo.Light.DropDownItem
frameworks/base/core/res/res/values/public.xml:1615: warning: No comment for public symbol android:style/Widget.Holo.Light.DropDownItem.Spinner
frameworks/base/core/res/res/values/public.xml:1588: warning: No comment for public symbol android:style/Widget.Holo.Light.EditText
frameworks/base/core/res/res/values/public.xml:1589: warning: No comment for public symbol android:style/Widget.Holo.Light.ExpandableListView
frameworks/base/core/res/res/values/public.xml:1590: warning: No comment for public symbol android:style/Widget.Holo.Light.GridView
frameworks/base/core/res/res/values/public.xml:1608: warning: No comment for public symbol android:style/Widget.Holo.Light.HorizontalScrollView
frameworks/base/core/res/res/values/public.xml:1591: warning: No comment for public symbol android:style/Widget.Holo.Light.ImageButton
frameworks/base/core/res/res/values/public.xml:1617: warning: No comment for public symbol android:style/Widget.Holo.Light.ListPopupWindow
frameworks/base/core/res/res/values/public.xml:1592: warning: No comment for public symbol android:style/Widget.Holo.Light.ListView
frameworks/base/core/res/res/values/public.xml:1587: warning: No comment for public symbol android:style/Widget.Holo.Light.ListView.DropDown
frameworks/base/core/res/res/values/public.xml:1988: warning: No comment for public symbol android:style/Widget.Holo.Light.MediaRouteButton
frameworks/base/core/res/res/values/public.xml:1618: warning: No comment for public symbol android:style/Widget.Holo.Light.PopupMenu
frameworks/base/core/res/res/values/public.xml:1593: warning: No comment for public symbol android:style/Widget.Holo.Light.PopupWindow
frameworks/base/core/res/res/values/public.xml:1594: warning: No comment for public symbol android:style/Widget.Holo.Light.ProgressBar
frameworks/base/core/res/res/values/public.xml:1595: warning: No comment for public symbol android:style/Widget.Holo.Light.ProgressBar.Horizontal
frameworks/base/core/res/res/values/public.xml:1599: warning: No comment for public symbol android:style/Widget.Holo.Light.ProgressBar.Inverse
frameworks/base/core/res/res/values/public.xml:1598: warning: No comment for public symbol android:style/Widget.Holo.Light.ProgressBar.Large
frameworks/base/core/res/res/values/public.xml:1601: warning: No comment for public symbol android:style/Widget.Holo.Light.ProgressBar.Large.Inverse
frameworks/base/core/res/res/values/public.xml:1596: warning: No comment for public symbol android:style/Widget.Holo.Light.ProgressBar.Small
frameworks/base/core/res/res/values/public.xml:1600: warning: No comment for public symbol android:style/Widget.Holo.Light.ProgressBar.Small.Inverse
frameworks/base/core/res/res/values/public.xml:1597: warning: No comment for public symbol android:style/Widget.Holo.Light.ProgressBar.Small.Title
frameworks/base/core/res/res/values/public.xml:1603: warning: No comment for public symbol android:style/Widget.Holo.Light.RatingBar
frameworks/base/core/res/res/values/public.xml:1604: warning: No comment for public symbol android:style/Widget.Holo.Light.RatingBar.Indicator
frameworks/base/core/res/res/values/public.xml:1605: warning: No comment for public symbol android:style/Widget.Holo.Light.RatingBar.Small
frameworks/base/core/res/res/values/public.xml:1607: warning: No comment for public symbol android:style/Widget.Holo.Light.ScrollView
frameworks/base/core/res/res/values/public.xml:1602: warning: No comment for public symbol android:style/Widget.Holo.Light.SeekBar
frameworks/base/core/res/res/values/public.xml:1609: warning: No comment for public symbol android:style/Widget.Holo.Light.Spinner
frameworks/base/core/res/res/values/public.xml:1626: warning: No comment for public symbol android:style/Widget.Holo.Light.Tab
frameworks/base/core/res/res/values/public.xml:1611: warning: No comment for public symbol android:style/Widget.Holo.Light.TabWidget
frameworks/base/core/res/res/values/public.xml:1584: warning: No comment for public symbol android:style/Widget.Holo.Light.TextView
frameworks/base/core/res/res/values/public.xml:1616: warning: No comment for public symbol android:style/Widget.Holo.Light.TextView.SpinnerItem
frameworks/base/core/res/res/values/public.xml:1612: warning: No comment for public symbol android:style/Widget.Holo.Light.WebTextView
frameworks/base/core/res/res/values/public.xml:1613: warning: No comment for public symbol android:style/Widget.Holo.Light.WebView
frameworks/base/core/res/res/values/public.xml:1571: warning: No comment for public symbol android:style/Widget.Holo.ListPopupWindow
frameworks/base/core/res/res/values/public.xml:1549: warning: No comment for public symbol android:style/Widget.Holo.ListView
frameworks/base/core/res/res/values/public.xml:1544: warning: No comment for public symbol android:style/Widget.Holo.ListView.DropDown
frameworks/base/core/res/res/values/public.xml:1987: warning: No comment for public symbol android:style/Widget.Holo.MediaRouteButton
frameworks/base/core/res/res/values/public.xml:1572: warning: No comment for public symbol android:style/Widget.Holo.PopupMenu
frameworks/base/core/res/res/values/public.xml:1550: warning: No comment for public symbol android:style/Widget.Holo.PopupWindow
frameworks/base/core/res/res/values/public.xml:1551: warning: No comment for public symbol android:style/Widget.Holo.ProgressBar
frameworks/base/core/res/res/values/public.xml:1552: warning: No comment for public symbol android:style/Widget.Holo.ProgressBar.Horizontal
frameworks/base/core/res/res/values/public.xml:1555: warning: No comment for public symbol android:style/Widget.Holo.ProgressBar.Large
frameworks/base/core/res/res/values/public.xml:1553: warning: No comment for public symbol android:style/Widget.Holo.ProgressBar.Small
frameworks/base/core/res/res/values/public.xml:1554: warning: No comment for public symbol android:style/Widget.Holo.ProgressBar.Small.Title
frameworks/base/core/res/res/values/public.xml:1557: warning: No comment for public symbol android:style/Widget.Holo.RatingBar
frameworks/base/core/res/res/values/public.xml:1558: warning: No comment for public symbol android:style/Widget.Holo.RatingBar.Indicator
frameworks/base/core/res/res/values/public.xml:1559: warning: No comment for public symbol android:style/Widget.Holo.RatingBar.Small
frameworks/base/core/res/res/values/public.xml:1561: warning: No comment for public symbol android:style/Widget.Holo.ScrollView
frameworks/base/core/res/res/values/public.xml:1556: warning: No comment for public symbol android:style/Widget.Holo.SeekBar
frameworks/base/core/res/res/values/public.xml:1563: warning: No comment for public symbol android:style/Widget.Holo.Spinner
frameworks/base/core/res/res/values/public.xml:1625: warning: No comment for public symbol android:style/Widget.Holo.Tab
frameworks/base/core/res/res/values/public.xml:1565: warning: No comment for public symbol android:style/Widget.Holo.TabWidget
frameworks/base/core/res/res/values/public.xml:1541: warning: No comment for public symbol android:style/Widget.Holo.TextView
frameworks/base/core/res/res/values/public.xml:1570: warning: No comment for public symbol android:style/Widget.Holo.TextView.SpinnerItem
frameworks/base/core/res/res/values/public.xml:1566: warning: No comment for public symbol android:style/Widget.Holo.WebTextView
frameworks/base/core/res/res/values/public.xml:1567: warning: No comment for public symbol android:style/Widget.Holo.WebView
frameworks/base/core/res/res/values/public.xml:639: warning: No comment for public symbol android:style/Widget.ImageButton
frameworks/base/core/res/res/values/public.xml:638: warning: No comment for public symbol android:style/Widget.ImageWell
frameworks/base/core/res/res/values/public.xml:1070: warning: No comment for public symbol android:style/Widget.KeyboardView
frameworks/base/core/res/res/values/public.xml:1531: warning: No comment for public symbol android:style/Widget.ListPopupWindow
frameworks/base/core/res/res/values/public.xml:647: warning: No comment for public symbol android:style/Widget.ListView
frameworks/base/core/res/res/values/public.xml:649: warning: No comment for public symbol android:style/Widget.ListView.DropDown
frameworks/base/core/res/res/values/public.xml:650: warning: No comment for public symbol android:style/Widget.ListView.Menu
frameworks/base/core/res/res/values/public.xml:648: warning: No comment for public symbol android:style/Widget.ListView.White
frameworks/base/core/res/res/values/public.xml:1532: warning: No comment for public symbol android:style/Widget.PopupMenu
frameworks/base/core/res/res/values/public.xml:655: warning: No comment for public symbol android:style/Widget.PopupWindow
frameworks/base/core/res/res/values/public.xml:629: warning: No comment for public symbol android:style/Widget.ProgressBar
frameworks/base/core/res/res/values/public.xml:632: warning: No comment for public symbol android:style/Widget.ProgressBar.Horizontal
frameworks/base/core/res/res/values/public.xml:1132: warning: No comment for public symbol android:style/Widget.ProgressBar.Inverse
frameworks/base/core/res/res/values/public.xml:630: warning: No comment for public symbol android:style/Widget.ProgressBar.Large
frameworks/base/core/res/res/values/public.xml:1133: warning: No comment for public symbol android:style/Widget.ProgressBar.Large.Inverse
frameworks/base/core/res/res/values/public.xml:631: warning: No comment for public symbol android:style/Widget.ProgressBar.Small
frameworks/base/core/res/res/values/public.xml:1134: warning: No comment for public symbol android:style/Widget.ProgressBar.Small.Inverse
frameworks/base/core/res/res/values/public.xml:634: warning: No comment for public symbol android:style/Widget.RatingBar
frameworks/base/core/res/res/values/public.xml:646: warning: No comment for public symbol android:style/Widget.ScrollView
frameworks/base/core/res/res/values/public.xml:633: warning: No comment for public symbol android:style/Widget.SeekBar
frameworks/base/core/res/res/values/public.xml:641: warning: No comment for public symbol android:style/Widget.Spinner
frameworks/base/core/res/res/values/public.xml:1529: warning: No comment for public symbol android:style/Widget.Spinner.DropDown
frameworks/base/core/res/res/values/public.xml:653: warning: No comment for public symbol android:style/Widget.TabWidget
frameworks/base/core/res/res/values/public.xml:635: warning: No comment for public symbol android:style/Widget.TextView
frameworks/base/core/res/res/values/public.xml:642: warning: No comment for public symbol android:style/Widget.TextView.PopupMenu
frameworks/base/core/res/res/values/public.xml:643: warning: No comment for public symbol android:style/Widget.TextView.SpinnerItem
frameworks/base/core/res/res/values/public.xml:652: warning: No comment for public symbol android:style/Widget.WebView
target Java: framework-base (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework-base_intermediates/classes)
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework-base_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework-base_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework-base_intermediates/classes.jar
target Static Jar: framework-base (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework-base_intermediates/javalib.jar)
target Java: framework (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework_intermediates/classes)
/bin/bash: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework_intermediates/classes/java-source-list: No such file or directory
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework_intermediates/classes.jar
target Java: framework2 (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework2_intermediates/classes)
/bin/bash: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework2_intermediates/classes/java-source-list: No such file or directory
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework2_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework2_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/framework2_intermediates/classes.jar
Aidl: telephony-common <= frameworks/opt/telephony/src/java/org/codeaurora/ims/csvt/ICsvtServiceListener.aidl
Aidl: telephony-common <= frameworks/opt/telephony/src/java/org/codeaurora/ims/csvt/ICsvtService.aidl
Aidl: telephony-common <= frameworks/opt/telephony/src/java/com/android/internal/telephony/IIccPhoneBook.aidl
Aidl: telephony-common <= frameworks/opt/telephony/src/java/com/android/internal/telephony/msim/IIccPhoneBookMSim.aidl
Aidl: telephony-common <= frameworks/opt/telephony/src/java/com/android/internal/telephony/msim/ISmsMSim.aidl
logtags: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/telephony-common_intermediates/src/src/java/com/android/internal/telephony/EventLogTags.java <= frameworks/opt/telephony/src/java/com/android/internal/telephony/EventLogTags.logtags
Aidl: voip-common <= frameworks/opt/net/voip/src/java/android/net/sip/ISipSession.aidl
Aidl: voip-common <= frameworks/opt/net/voip/src/java/android/net/sip/ISipService.aidl
Aidl: voip-common <= frameworks/opt/net/voip/src/java/android/net/sip/ISipSessionListener.aidl
target Java: voip-common (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/voip-common_intermediates/classes)
Note: frameworks/opt/net/voip/src/java/com/android/server/sip/SipService.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: frameworks/opt/net/voip/src/java/com/android/server/sip/SipService.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/voip-common_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/voip-common_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/voip-common_intermediates/classes.jar
target Java: telephony-common (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/telephony-common_intermediates/classes)
Note: Some input files use or override a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: Some input files use unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/telephony-common_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/telephony-common_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/telephony-common_intermediates/classes.jar
target Java: mms-common (/home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/mms-common_intermediates/classes)
Note: frameworks/opt/mms/src/java/com/google/android/mms/util/SqliteWrapper.java uses or overrides a deprecated API.
Note: Recompile with -Xlint:deprecation for details.
Note: frameworks/opt/mms/src/java/com/google/android/mms/pdu/PduHeaders.java uses unchecked or unsafe operations.
Note: Recompile with -Xlint:unchecked for details.
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/mms-common_intermediates/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/mms-common_intermediates/emma_out/lib/classes-jarjar.jar
Copying: /home/hhp211/Source/AOSPA/out/target/common/obj/JAVA_LIBRARIES/mms-common_intermediates/classes.jar
Aidl Preprocess: /home/hhp211/Source/AOSPA/out/target/common/obj/framework.aidl
Docs droiddoc: /home/hhp211/Source/AOSPA/out/target/common/docs/api-stubs
DroidDoc took 16 sec. to write docs to /home/hhp211/Source/AOSPA/out/target/common/docs/api-stubs
Copy: apicheck (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/apicheck_intermediates/apicheck)
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/apicheck
Checking API: checkapi-last
Checking API: checkapi-current
/home/hhp211/Source/AOSPA/out/target/common/obj/PACKAGING/public_api.txt:26068: error 3: Added class SettingConfirmationHelper to package android.util

******************************
You have tried to change the API from what has been previously approved.

To make these errors go away, you have two choices:
   1) You can add "@hide" javadoc comments to the methods, etc. listed in the
      errors above.

   2) You can update current.txt by executing the following command:
         make update-api

      To submit the revised current.txt to the main Android repository,
      you will need approval.
******************************



make: *** [/home/hhp211/Source/AOSPA/out/target/common/obj/PACKAGING/checkapi-current-timestamp] Error 38

hhp211@hhp211-Q500A:~/Source/AOSPA$ make update-api



============================================
PLATFORM_VERSION_CODENAME=REL
PLATFORM_VERSION=4.4.2
TARGET_PRODUCT=pa_fascinatemtd
TARGET_BUILD_VARIANT=userdebug
TARGET_BUILD_TYPE=release
TARGET_BUILD_APPS=
TARGET_ARCH=arm
TARGET_ARCH_VARIANT=armv7-a-neon
TARGET_CPU_VARIANT=cortex-a8
HOST_ARCH=x86
HOST_OS=linux
HOST_OS_EXTRA=Linux-3.14.0-031400rc1-generic-x86_64-with-Ubuntu-12.04-precise
HOST_BUILD_TYPE=release
BUILD_ID=KVT49L
OUT_DIR=/home/hhp211/Source/AOSPA/out
============================================
/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/APPS/SignatureTest_intermediates
build/core/base_rules.mk:529: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/fsck_msdos'
bootable/recovery/dosfstools/Android.mk:21: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/fsck_msdos'
find: `src': No such file or directory
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libril.so'
build/core/dynamic_binary.mk:117: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libril.so'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libril.so'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libril.so'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/rild'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/rild'
PRODUCT_COPY_FILES device/generic/goldfish/camera/media_profiles.xml:system/etc/media_profiles.xml ignored.
PRODUCT_COPY_FILES device/generic/goldfish/camera/media_codecs.xml:system/etc/media_codecs.xml ignored.
PRODUCT_COPY_FILES hardware/libhardware_legacy/audio/audio_policy.conf:system/etc/audio_policy.conf ignored.
PRODUCT_COPY_FILES vendor/pa/prebuilt/etc/apns-conf.xml:system/etc/apns-conf.xml ignored.
No private recovery resources for TARGET_DEVICE fascinatemtd
device/samsung/fascinatemtd/shbootimg.mk:8: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img'
device/samsung/fascinatemtd/shbootimg.mk:8: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img'
device/samsung/fascinatemtd/shbootimg.mk:12: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery.img'
device/samsung/fascinatemtd/shbootimg.mk:12: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery.img'
Copying current.txt


hhp211@hhp211-Q500A:~/Source/AOSPA$ make


============================================
PLATFORM_VERSION_CODENAME=REL
PLATFORM_VERSION=4.4.2
TARGET_PRODUCT=pa_fascinatemtd
TARGET_BUILD_VARIANT=userdebug
TARGET_BUILD_TYPE=release
TARGET_BUILD_APPS=
TARGET_ARCH=arm
TARGET_ARCH_VARIANT=armv7-a-neon
TARGET_CPU_VARIANT=cortex-a8
HOST_ARCH=x86
HOST_OS=linux
HOST_OS_EXTRA=Linux-3.14.0-031400rc1-generic-x86_64-with-Ubuntu-12.04-precise
HOST_BUILD_TYPE=release
BUILD_ID=KVT49L
OUT_DIR=/home/hhp211/Source/AOSPA/out
============================================
/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/APPS/SignatureTest_intermediates
build/core/base_rules.mk:529: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/fsck_msdos'
bootable/recovery/dosfstools/Android.mk:21: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/fsck_msdos'
find: `src': No such file or directory
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/etc/permissions/android.software.live_wallpaper.xml'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libril.so'
build/core/dynamic_binary.mk:117: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libril.so'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libril.so'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libril.so'
build/core/Makefile:66: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/rild'
build/core/base_rules.mk:529: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/rild'
PRODUCT_COPY_FILES device/generic/goldfish/camera/media_profiles.xml:system/etc/media_profiles.xml ignored.
PRODUCT_COPY_FILES device/generic/goldfish/camera/media_codecs.xml:system/etc/media_codecs.xml ignored.
PRODUCT_COPY_FILES hardware/libhardware_legacy/audio/audio_policy.conf:system/etc/audio_policy.conf ignored.
PRODUCT_COPY_FILES vendor/pa/prebuilt/etc/apns-conf.xml:system/etc/apns-conf.xml ignored.
No private recovery resources for TARGET_DEVICE fascinatemtd
device/samsung/fascinatemtd/shbootimg.mk:8: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img'
device/samsung/fascinatemtd/shbootimg.mk:8: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img'
device/samsung/fascinatemtd/shbootimg.mk:12: warning: overriding commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery.img'
device/samsung/fascinatemtd/shbootimg.mk:12: warning: ignoring old commands for target `/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery.img'
Checking API: checkapi-current
target Prebuilt:  (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/monkey)
target Prebuilt:  (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/usr/share/bmd/RFFspeed_501.bmd)
target Prebuilt:  (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/usr/share/bmd/RFFstd_501.bmd)
target Prebuilt:  (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/bmgr)
target Prebuilt:  (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/ime)
target Prebuilt:  (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/input)
target Prebuilt:  (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/pm)
target Prebuilt:  (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/bin/svc)
mkdir -p /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/KERNEL_OBJ
mkdir -p /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/modules
make  -C kernel/samsung/aries O=/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/KERNEL_OBJ ARCH=arm CROSS_COMPILE=" /home/hhp211/Source/AOSPA/prebuilts/gcc/linux-x86/arm/arm-eabi-4.7/bin/arm-eabi-" VARIANT_DEFCONFIG= SELINUX_DEFCONFIG= cyanogenmod_fascinatemtd_defconfig
make[1]: Entering directory `/home/hhp211/Source/AOSPA/kernel/samsung/aries'
  HOSTCC  scripts/basic/fixdep
  GEN     /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/KERNEL_OBJ/Makefile
  HOSTCC  scripts/kconfig/conf.o
  SHIPPED scripts/kconfig/zconf.tab.c
  SHIPPED scripts/kconfig/lex.zconf.c
  SHIPPED scripts/kconfig/zconf.hash.c
  HOSTCC  scripts/kconfig/zconf.tab.o
  HOSTLD  scripts/kconfig/conf
#
# configuration written to .config
#
make[1]: Leaving directory `/home/hhp211/Source/AOSPA/kernel/samsung/aries'
make  -C kernel/samsung/aries O=/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/KERNEL_OBJ ARCH=arm CROSS_COMPILE=" /home/hhp211/Source/AOSPA/prebuilts/gcc/linux-x86/arm/arm-eabi-4.7/bin/arm-eabi-" headers_install
make[1]: Entering directory `/home/hhp211/Source/AOSPA/kernel/samsung/aries'
  CHK     include/linux/version.h
  UPD     include/linux/version.h
  HOSTCC  scripts/unifdef
  INSTALL include/asm-generic (34 files)
  INSTALL include/drm (13 files)
  INSTALL include/linux/byteorder (2 files)
  INSTALL include/linux/caif (2 files)
  INSTALL include/linux/can (4 files)
  INSTALL include/linux/dvb (8 files)
  INSTALL include/linux/hdlc (1 file)
  INSTALL include/linux/isdn (1 file)
  INSTALL include/linux/mmc (1 file)
  INSTALL include/linux/netfilter/ipset (4 files)
  INSTALL include/linux/netfilter (69 files)
  INSTALL include/linux/netfilter_arp (2 files)
  INSTALL include/linux/netfilter_bridge (18 files)
  INSTALL include/linux/netfilter_ipv4 (14 files)
  INSTALL include/linux/netfilter_ipv6 (11 files)
  INSTALL include/linux/nfsd (6 files)
  INSTALL include/linux/raid (2 files)
  INSTALL include/linux/spi (1 file)
  INSTALL include/linux/sunrpc (1 file)
  INSTALL include/linux/tc_act (7 files)
  INSTALL include/linux/tc_ematch (4 files)
  INSTALL include/linux/usb (9 files)
  INSTALL include/linux/wimax (1 file)
  INSTALL include/linux (365 files)
  INSTALL include/mtd (5 files)
  INSTALL include/rdma (6 files)
  INSTALL include/scsi/fc (4 files)
  INSTALL include/scsi (3 files)
  INSTALL include/sound (8 files)
  INSTALL include/video (3 files)
  INSTALL include/xen (2 files)
  INSTALL include (0 file)
  INSTALL include/asm (32 files)
make[1]: Leaving directory `/home/hhp211/Source/AOSPA/kernel/samsung/aries'
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/mkbootfs_intermediates/import_includes
host C: mkbootfs <= system/core/cpio/mkbootfs.c
Export includes file: system/core/cpio/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/mkbootfs_intermediates/export_includes
host Executable: mkbootfs (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/mkbootfs_intermediates/mkbootfs)
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/mkbootfs
Export includes file: external/zlib/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libz_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/minigzip_intermediates/import_includes
host C: minigzip <= external/zlib/src/test/minigzip.c
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libz_intermediates/import_includes
host C: libz <= external/zlib/src/adler32.c
host C: libz <= external/zlib/src/compress.c
host C: libz <= external/zlib/src/crc32.c
host C: libz <= external/zlib/src/deflate.c
host C: libz <= external/zlib/src/gzclose.c
host C: libz <= external/zlib/src/gzlib.c
host C: libz <= external/zlib/src/gzread.c
host C: libz <= external/zlib/src/gzwrite.c
host C: libz <= external/zlib/src/infback.c
host C: libz <= external/zlib/src/inflate.c
host C: libz <= external/zlib/src/inftrees.c
host C: libz <= external/zlib/src/inffast.c
host C: libz <= external/zlib/src/trees.c
host C: libz <= external/zlib/src/uncompr.c
host C: libz <= external/zlib/src/zutil.c
host StaticLib: libz (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libz_intermediates/libz.a)
Export includes file: external/zlib/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/minigzip_intermediates/export_includes
host Executable: minigzip (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/minigzip_intermediates/minigzip)
Notice file: external/zlib/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//bin/minigzip.txt
Notice file: external/zlib/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libz.a.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/minigzip
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/[ -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/[[ -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/adjtimex -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/arp -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ash -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/awk -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/base64 -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/basename -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/bbconfig -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/blkid -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/blockdev -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/brctl -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/bunzip2 -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/bzcat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/bzip2 -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/cal -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/cat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/catv -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/chattr -> busybox
target Generated: toolbox_recovery <= system/core/toolbox//Android.mk
Export includes file: bionic/libc/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libc_intermediates/export_includes
Export includes file: system/core/libcutils/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libcutils_intermediates/export_includes
Export includes file: system/core/liblog/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/liblog_intermediates/export_includes
Export includes file: bionic/libm/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libm_intermediates/export_includes
Export includes file: external/libselinux/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libselinux_intermediates/export_includes
Export includes file: bionic/libstdc++/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libstdc++_intermediates/export_includes
Export includes file: external/compiler-rt/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libcompiler_rt-extras_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/toolbox_recovery_intermediates/import_includes
target thumb C: toolbox_recovery <= system/core/toolbox//toolbox.c
target thumb C: toolbox_recovery <= system/core/toolbox//start.c
target thumb C: toolbox_recovery <= system/core/toolbox//stop.c
target thumb C: toolbox_recovery <= system/core/toolbox//getprop.c
target thumb C: toolbox_recovery <= system/core/toolbox//setprop.c
target thumb C: toolbox_recovery <= system/core/toolbox//ls.c
target thumb C: toolbox_recovery <= system/core/toolbox//getenforce.c
target thumb C: toolbox_recovery <= system/core/toolbox//setenforce.c
target thumb C: toolbox_recovery <= system/core/toolbox//chcon.c
target thumb C: toolbox_recovery <= system/core/toolbox//restorecon.c
target thumb C: toolbox_recovery <= system/core/toolbox//runcon.c
target thumb C: toolbox_recovery <= system/core/toolbox//getsebool.c
target thumb C: toolbox_recovery <= system/core/toolbox//setsebool.c
system/core/toolbox//setsebool.c: In function 'do_setsebool':
system/core/toolbox//setsebool.c:19:12: warning: assignment discards 'const' qualifier from pointer target type [enabled by default]
target thumb C: toolbox_recovery <= system/core/toolbox//load_policy.c
target thumb C: toolbox_recovery <= system/core/toolbox//dynarray.c
Export includes file: bionic/libdl/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libdl_intermediates/export_includes
Export includes file: bionic/libc/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_common_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libc_intermediates/import_includes
target asm: libc <= bionic/libc/arch-arm/bionic/crtend_so.S
target arm C++: libc <= bionic/libc/bionic/pthread_create.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target arm C++: libc <= bionic/libc/bionic/pthread_key.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc <= bionic/libc/bionic/malloc_debug_common.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc <= bionic/libc/bionic/pthread_debug.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
bionic/libc/bionic/pthread_debug.cpp:545:13: warning: 'void hashmap_removeEntry(HashTable*, HashEntry*)' defined but not used [-Wunused-function]
target thumb C++: libc <= bionic/libc/bionic/libc_init_dynamic.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
bionic/libc/bionic/libc_init_dynamic.cpp:95:17: warning: unused parameter 'onexit' [-Wunused-parameter]
target arm C: libc <= bionic/libc/bionic/pthread.c
target thumb C: libc <= bionic/libc/arch-arm/bionic/crtbegin_so.c
target thumb C: libc <= bionic/libc/arch-arm/bionic/atexit_legacy.c
target thumb C: libc <= bionic/libc/arch-arm/bionic/exidx_dynamic.c
target thumb C: libc <= bionic/libc/bionic/dlmalloc.c
In file included from bionic/libc/bionic/dlmalloc.c:35:0:
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'init_bins':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:3929:5: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'prepend_alloc':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:3982:7: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:3982:7: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:3987:5: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'add_segment':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4042:5: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'dispose_chunk':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4401:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4401:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4435:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4435:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4446:5: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'tmalloc_large':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4516:11: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'tmalloc_small':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4554:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'dlmalloc':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4607:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4625:11: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4637:13: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'dlfree':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4741:17: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4741:17: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4777:15: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4777:15: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4789:13: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'try_realloc_chunk':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4891:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4891:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libdl_intermediates/import_includes
target thumb C: libdl <= bionic/libdl/libdl.c
Export includes file: external/llvm/lib/TableGen/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTableGen_intermediates/export_includes
Export includes file: external/llvm/lib/Support/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMSupport_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/clang-tblgen_intermediates/import_includes
host C++: clang-tblgen <= external/clang/utils/TableGen/ClangASTNodesEmitter.cpp
host C++: clang-tblgen <= external/clang/utils/TableGen/ClangAttrEmitter.cpp
host C++: clang-tblgen <= external/clang/utils/TableGen/ClangCommentCommandInfoEmitter.cpp
host C++: clang-tblgen <= external/clang/utils/TableGen/ClangCommentHTMLNamedCharacterReferenceEmitter.cpp
host C++: clang-tblgen <= external/clang/utils/TableGen/ClangCommentHTMLTagsEmitter.cpp
host C++: clang-tblgen <= external/clang/utils/TableGen/ClangDiagnosticsEmitter.cpp
host C++: clang-tblgen <= external/clang/utils/TableGen/ClangSACheckersEmitter.cpp
host C++: clang-tblgen <= external/clang/utils/TableGen/NeonEmitter.cpp
host C++: clang-tblgen <= external/clang/utils/TableGen/TableGen.cpp
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTableGen_intermediates/import_includes
host C++: libLLVMTableGen <= external/llvm/lib/TableGen/Error.cpp
host C++: libLLVMTableGen <= external/llvm/lib/TableGen/Main.cpp
host C++: libLLVMTableGen <= external/llvm/lib/TableGen/Record.cpp
host C++: libLLVMTableGen <= external/llvm/lib/TableGen/StringMatcher.cpp
host C++: libLLVMTableGen <= external/llvm/lib/TableGen/TableGenBackend.cpp
host C++: libLLVMTableGen <= external/llvm/lib/TableGen/TGLexer.cpp
host C++: libLLVMTableGen <= external/llvm/lib/TableGen/TGParser.cpp
host StaticLib: libLLVMTableGen (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTableGen_intermediates/libLLVMTableGen.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMSupport_intermediates/import_includes
host C++: libLLVMSupport <= external/llvm/lib/Support/Allocator.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/APFloat.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/APInt.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/APSInt.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Atomic.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/BlockFrequency.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/BranchProbability.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/CommandLine.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/ConstantRange.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/ConvertUTFWrapper.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/CrashRecoveryContext.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/DAGDeltaAlgorithm.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/DataStream.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/DataExtractor.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Debug.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/DeltaAlgorithm.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Dwarf.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/DynamicLibrary.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Errno.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/ErrorHandling.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/FileUtilities.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/FoldingSet.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/FormattedStream.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/GraphWriter.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Hashing.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Host.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/IntervalMap.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/IntEqClasses.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/IntrusiveRefCntPtr.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/IsInf.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/IsNAN.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Locale.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/LockFileManager.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/MD5.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/ManagedStatic.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Memory.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/MemoryBuffer.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/MemoryObject.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Mutex.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Path.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/PluginLoader.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/PrettyStackTrace.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Process.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Program.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Regex.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/RWMutex.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/SearchForAddressOfSpecialSymbol.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Signals.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/SmallPtrSet.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/SmallVector.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/SourceMgr.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Statistic.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/StreamableMemoryObject.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/StringExtras.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/StringMap.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/StringPool.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/StringRef.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/SystemUtils.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/TargetRegistry.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Threading.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/ThreadLocal.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Timer.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/TimeValue.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/ToolOutputFile.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Triple.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Twine.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Valgrind.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/Watchdog.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/circular_raw_ostream.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/raw_os_ostream.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/raw_ostream.cpp
host C++: libLLVMSupport <= external/llvm/lib/Support/system_error.cpp
host C: libLLVMSupport <= external/llvm/lib/Support/ConvertUTF.c
host C: libLLVMSupport <= external/llvm/lib/Support/regcomp.c
host C: libLLVMSupport <= external/llvm/lib/Support/regerror.c
host C: libLLVMSupport <= external/llvm/lib/Support/regexec.c
host C: libLLVMSupport <= external/llvm/lib/Support/regfree.c
host C: libLLVMSupport <= external/llvm/lib/Support/regstrlcpy.c
host StaticLib: libLLVMSupport (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMSupport_intermediates/libLLVMSupport.a)
Export includes file: external/clang/utils/TableGen/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/clang-tblgen_intermediates/export_includes
host Executable: clang-tblgen (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/clang-tblgen_intermediates/clang-tblgen)
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/clang-tblgen
Host Clang TableGen: clang (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: clang (gen-clang-diags-defs -clang-component=Driver) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: clang (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/tblgen_intermediates/import_includes
host C++: tblgen <= external/llvm/utils/TableGen/AsmMatcherEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/AsmWriterEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/AsmWriterInst.cpp
host C++: tblgen <= external/llvm/utils/TableGen/CallingConvEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/CodeEmitterGen.cpp
host C++: tblgen <= external/llvm/utils/TableGen/CodeGenDAGPatterns.cpp
host C++: tblgen <= external/llvm/utils/TableGen/CodeGenInstruction.cpp
host C++: tblgen <= external/llvm/utils/TableGen/CodeGenMapTable.cpp
host C++: tblgen <= external/llvm/utils/TableGen/CodeGenRegisters.cpp
In file included from external/llvm/utils/TableGen/CodeGenRegisters.h:25:0,
                 from external/llvm/utils/TableGen/CodeGenRegisters.cpp:17:
external/llvm/include/llvm/TableGen/Record.h: In member function 'bool llvm::LessRecordRegister::operator()(const llvm::Record*, const llvm::Record*) const':
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'RHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'LHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
In file included from /home/hhp211/Source/AOSPA/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.6/bin/../lib/gcc/i686-linux/4.6.x-google/../../../../i686-linux/include/c++/4.6.x-google/algorithm:63:0,
                 from external/llvm/include/llvm/ADT/SmallVector.h:21,
                 from external/llvm/include/llvm/ADT/SmallSet.h:18,
                 from external/llvm/include/llvm/ADT/SetVector.h:23,
                 from external/llvm/utils/TableGen/SetTheory.h:50,
                 from external/llvm/utils/TableGen/CodeGenRegisters.h:18,
                 from external/llvm/utils/TableGen/CodeGenRegisters.cpp:17:
external/llvm/include/llvm/TableGen/Record.h: In function 'void std::__introsort_loop(_RandomAccessIterator, _RandomAccessIterator, _Size, _Compare) [with _RandomAccessIterator = __gnu_cxx::__normal_iterator<llvm::Record**, std::vector<llvm::Record*> >, _Size = int, _Compare = llvm::LessRecordRegister]':
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'RHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:24: note: 'RHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'LHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:16: note: 'LHSVal' was declared here
host C++: tblgen <= external/llvm/utils/TableGen/CodeGenSchedule.cpp
host C++: tblgen <= external/llvm/utils/TableGen/CodeGenTarget.cpp
host C++: tblgen <= external/llvm/utils/TableGen/CTagsEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/DAGISelEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/DAGISelMatcherEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/DAGISelMatcherGen.cpp
host C++: tblgen <= external/llvm/utils/TableGen/DAGISelMatcherOpt.cpp
host C++: tblgen <= external/llvm/utils/TableGen/DAGISelMatcher.cpp
host C++: tblgen <= external/llvm/utils/TableGen/DFAPacketizerEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/DisassemblerEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/FastISelEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/FixedLenDecoderEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/InstrInfoEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/IntrinsicEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/OptParserEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/PseudoLoweringEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/RegisterInfoEmitter.cpp
In file included from external/llvm/utils/TableGen/CodeGenRegisters.h:25:0,
                 from external/llvm/utils/TableGen/RegisterInfoEmitter.cpp:16:
external/llvm/include/llvm/TableGen/Record.h: In member function 'bool llvm::LessRecordRegister::operator()(const llvm::Record*, const llvm::Record*) const':
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'RHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'LHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
In file included from /home/hhp211/Source/AOSPA/prebuilts/gcc/linux-x86/host/i686-linux-glibc2.7-4.6/bin/../lib/gcc/i686-linux/4.6.x-google/../../../../i686-linux/include/c++/4.6.x-google/set:60:0,
                 from external/llvm/include/llvm/ADT/SmallSet.h:19,
                 from external/llvm/include/llvm/ADT/SetVector.h:23,
                 from external/llvm/utils/TableGen/SetTheory.h:50,
                 from external/llvm/utils/TableGen/CodeGenRegisters.h:18,
                 from external/llvm/utils/TableGen/RegisterInfoEmitter.cpp:16:
external/llvm/include/llvm/TableGen/Record.h: In member function 'std::_Rb_tree<_Key, _Val, _KeyOfValue, _Compare, _Alloc>::const_iterator std::_Rb_tree<_Key, _Val, _KeyOfValue, _Compare, _Alloc>::find(const _Key&) const [with _Key = llvm::Record*, _Val = std::pair<llvm::Record* const, std::vector<long long int> >, _KeyOfValue = std::_Select1st<std::pair<llvm::Record* const, std::vector<long long int> > >, _Compare = llvm::LessRecordRegister, _Alloc = std::allocator<std::pair<llvm::Record* const, std::vector<long long int> > >, std::_Rb_tree<_Key, _Val, _KeyOfValue, _Compare, _Alloc>::const_iterator = std::_Rb_tree_const_iterator<std::pair<llvm::Record* const, std::vector<long long int> > >]':
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'RHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:24: note: 'RHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'LHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:16: note: 'LHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h: In function 'void (anonymous namespace)::RegisterInfoEmitter::_ZN12_GLOBAL__N_119RegisterInfoEmitter20EmitRegMappingTablesERN4llvm11raw_ostreamERKSt6vectorIPNS1_15CodeGenRegisterESaIS6_EEb.isra.565(llvm::raw_ostream&, const std::vector<llvm::CodeGenRegister*, std::allocator<llvm::CodeGenRegister*> >&, bool)':
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'RHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:24: note: 'RHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'LHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:16: note: 'LHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'RHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:24: note: 'RHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'LHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:16: note: 'LHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'RHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:24: note: 'RHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'LHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:16: note: 'LHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'RHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:24: note: 'RHSVal' was declared here
external/llvm/include/llvm/TableGen/Record.h:1807:7: warning: 'LHSVal' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/include/llvm/TableGen/Record.h:1800:16: note: 'LHSVal' was declared here
host C++: tblgen <= external/llvm/utils/TableGen/SetTheory.cpp
host C++: tblgen <= external/llvm/utils/TableGen/SubtargetEmitter.cpp
host C++: tblgen <= external/llvm/utils/TableGen/TGValueTypes.cpp
host C++: tblgen <= external/llvm/utils/TableGen/TableGen.cpp
host C++: tblgen <= external/llvm/utils/TableGen/X86DisassemblerTables.cpp
host C++: tblgen <= external/llvm/utils/TableGen/X86ModRMFilters.cpp
host C++: tblgen <= external/llvm/utils/TableGen/X86RecognizableInstr.cpp
Export includes file: external/llvm/utils/TableGen/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/tblgen_intermediates/export_includes
host Executable: tblgen (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/tblgen_intermediates/tblgen)
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/tblgen
Host TableGen: clang (gen-opt-parser-defs) <= external/clang/include/clang/Driver/Options.td
Host TableGen: clang (gen-opt-parser-defs) <= external/clang/include/clang/Driver/CC1AsOptions.td
Export includes file: external/clang/lib/FrontendTool/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangFrontendTool_intermediates/export_includes
Export includes file: external/clang/lib/Frontend/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangFrontend_intermediates/export_includes
Export includes file: external/clang/lib/ARCMigrate/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangARCMigrate_intermediates/export_includes
Export includes file: external/clang/lib/Driver/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangDriver_intermediates/export_includes
Export includes file: external/clang/lib/Serialization/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangSerialization_intermediates/export_includes
Export includes file: external/clang/lib/CodeGen/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangCodeGen_intermediates/export_includes
Export includes file: external/clang/lib/Rewrite/Frontend/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangRewriteFrontend_intermediates/export_includes
Export includes file: external/clang/lib/Rewrite/Core/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangRewriteCore_intermediates/export_includes
Export includes file: external/clang/lib/Parse/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangParse_intermediates/export_includes
Export includes file: external/clang/lib/Sema/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangSema_intermediates/export_includes
Export includes file: external/clang/lib/StaticAnalyzer/Frontend/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerFrontend_intermediates/export_includes
Export includes file: external/clang/lib/StaticAnalyzer/Checkers/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerCheckers_intermediates/export_includes
Export includes file: external/clang/lib/StaticAnalyzer/Core/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerCore_intermediates/export_includes
Export includes file: external/clang/lib/Analysis/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangAnalysis_intermediates/export_includes
Export includes file: external/clang/lib/Edit/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangEdit_intermediates/export_includes
Export includes file: external/clang/lib/AST/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangAST_intermediates/export_includes
Export includes file: external/clang/lib/Lex/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangLex_intermediates/export_includes
Export includes file: external/clang/lib/Basic/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangBasic_intermediates/export_includes
Export includes file: external/llvm/lib/Target/ARM/AsmParser/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMAsmParser_intermediates/export_includes
Export includes file: external/llvm/lib/Target/ARM/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMCodeGen_intermediates/export_includes
Export includes file: external/llvm/lib/Target/ARM/InstPrinter/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMAsmPrinter_intermediates/export_includes
Export includes file: external/llvm/lib/Target/ARM/Disassembler/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMDisassembler_intermediates/export_includes
Export includes file: external/llvm/lib/Target/ARM/MCTargetDesc/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMDesc_intermediates/export_includes
Export includes file: external/llvm/lib/Target/ARM/TargetInfo/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMInfo_intermediates/export_includes
Export includes file: external/llvm/lib/Target/Mips/AsmParser/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsAsmParser_intermediates/export_includes
Export includes file: external/llvm/lib/Target/Mips/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsCodeGen_intermediates/export_includes
Export includes file: external/llvm/lib/Target/Mips/Disassembler/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsDisassembler_intermediates/export_includes
Export includes file: external/llvm/lib/Target/Mips/InstPrinter/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsAsmPrinter_intermediates/export_includes
Export includes file: external/llvm/lib/Target/Mips/MCTargetDesc/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsDesc_intermediates/export_includes
Export includes file: external/llvm/lib/Target/Mips/TargetInfo/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsInfo_intermediates/export_includes
Export includes file: external/llvm/lib/Target/X86/TargetInfo/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Info_intermediates/export_includes
Export includes file: external/llvm/lib/Target/X86/AsmParser/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86AsmParser_intermediates/export_includes
Export includes file: external/llvm/lib/Target/X86/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86CodeGen_intermediates/export_includes
Export includes file: external/llvm/lib/Target/X86/Disassembler/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Disassembler_intermediates/export_includes
Export includes file: external/llvm/lib/Target/X86/MCTargetDesc/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Desc_intermediates/export_includes
Export includes file: external/llvm/lib/Target/X86/InstPrinter/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86AsmPrinter_intermediates/export_includes
Export includes file: external/llvm/lib/Target/X86/Utils/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Utils_intermediates/export_includes
Export includes file: external/llvm/lib/IRReader/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMIRReader_intermediates/export_includes
Export includes file: external/llvm/lib/AsmParser/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAsmParser_intermediates/export_includes
Export includes file: external/llvm/lib/CodeGen/AsmPrinter/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAsmPrinter_intermediates/export_includes
Export includes file: external/llvm/lib/Bitcode/Reader/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMBitReader_intermediates/export_includes
Export includes file: external/llvm/lib/Bitcode/Writer/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMBitWriter_intermediates/export_includes
Export includes file: external/llvm/lib/CodeGen/SelectionDAG/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMSelectionDAG_intermediates/export_includes
Export includes file: external/llvm/lib/Transforms/IPO/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMipo_intermediates/export_includes
Export includes file: external/llvm/lib/Analysis/IPA/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMipa_intermediates/export_includes
Export includes file: external/llvm/lib/Transforms/InstCombine/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMInstCombine_intermediates/export_includes
Export includes file: external/llvm/lib/Transforms/Instrumentation/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMInstrumentation_intermediates/export_includes
Export includes file: external/llvm/lib/CodeGen/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMCodeGen_intermediates/export_includes
Export includes file: external/llvm/lib/Object/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMObject_intermediates/export_includes
Export includes file: external/llvm/lib/Linker/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMLinker_intermediates/export_includes
Export includes file: external/llvm/lib/MC/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMC_intermediates/export_includes
Export includes file: external/llvm/lib/MC/MCParser/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMCParser_intermediates/export_includes
Export includes file: external/llvm/lib/Transforms/Scalar/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMScalarOpts_intermediates/export_includes
Export includes file: external/llvm/lib/Transforms/ObjCARC/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTransformObjCARC_intermediates/export_includes
Export includes file: external/llvm/lib/Transforms/Utils/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTransformUtils_intermediates/export_includes
Export includes file: external/llvm/lib/Transforms/Vectorize/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMVectorize_intermediates/export_includes
Export includes file: external/llvm/lib/Analysis/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAnalysis_intermediates/export_includes
Export includes file: external/llvm/lib/IR/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMCore_intermediates/export_includes
Export includes file: external/llvm/lib/Option/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMOption_intermediates/export_includes
Export includes file: external/llvm/lib/Target/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTarget_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/clang_intermediates/import_includes
host C++: clang <= external/clang/tools/driver/cc1_main.cpp
host C++: clang <= external/clang/tools/driver/cc1as_main.cpp
host C++: clang <= external/clang/tools/driver/driver.cpp
Host Clang TableGen: libclangFrontendTool (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangFrontendTool (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Host TableGen: libclangFrontendTool (gen-opt-parser-defs) <= external/clang/include/clang/Driver/Options.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangFrontendTool_intermediates/import_includes
host C++: libclangFrontendTool <= external/clang/lib/FrontendTool/ExecuteCompilerInvocation.cpp
host StaticLib: libclangFrontendTool (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangFrontendTool_intermediates/libclangFrontendTool.a)
Host Clang TableGen: libclangFrontend (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangFrontend (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangFrontend (gen-clang-attr-parsed-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangFrontend (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangFrontend (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangFrontend (gen-clang-diags-defs -clang-component=AST) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangFrontend (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangFrontend (gen-clang-diags-defs -clang-component=Driver) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangFrontend (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangFrontend (gen-clang-diags-defs -clang-component=Lex) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangFrontend (gen-clang-diags-defs -clang-component=Sema) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangFrontend (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangFrontend (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Host TableGen: libclangFrontend (gen-opt-parser-defs) <= external/clang/include/clang/Driver/Options.td
Updating Clang version info.
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangFrontend_intermediates/import_includes
host C++: libclangFrontend <= external/clang/lib/Frontend/ASTConsumers.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/ASTMerge.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/ASTUnit.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/CacheTokens.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/ChainedDiagnosticConsumer.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/ChainedIncludesSource.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/CompilerInstance.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/CompilerInvocation.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/CreateInvocationFromCommandLine.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/DependencyFile.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/DependencyGraph.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/DiagnosticRenderer.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/FrontendAction.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/FrontendActions.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/FrontendOptions.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/HeaderIncludeGen.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/InitHeaderSearch.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/InitPreprocessor.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/LangStandards.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/LayoutOverrideSource.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/LogDiagnosticPrinter.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/MultiplexConsumer.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/PrintPreprocessedOutput.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/SerializedDiagnosticPrinter.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/TextDiagnostic.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/TextDiagnosticBuffer.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/TextDiagnosticPrinter.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/Warnings.cpp
host C++: libclangFrontend <= external/clang/lib/Frontend/VerifyDiagnosticConsumer.cpp
host StaticLib: libclangFrontend (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangFrontend_intermediates/libclangFrontend.a)
Updating Clang version info.
Host Clang TableGen: libclangARCMigrate (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangARCMigrate (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangARCMigrate (gen-clang-attr-parsed-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangARCMigrate (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangARCMigrate (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangARCMigrate (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangARCMigrate (gen-clang-diags-defs -clang-component=Sema) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangARCMigrate (gen-clang-diag-groups) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangARCMigrate (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangARCMigrate (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangARCMigrate_intermediates/import_includes
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/ARCMT.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/ARCMTActions.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/FileRemapper.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/ObjCMT.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/PlistReporter.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransAPIUses.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransARCAssign.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransAutoreleasePool.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransBlockObjCVariable.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransEmptyStatementsAndDealloc.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransformActions.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/Transforms.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransGCAttrs.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransGCCalls.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransProperties.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransRetainReleaseDealloc.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransUnbridgedCasts.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransUnusedInitDelegate.cpp
host C++: libclangARCMigrate <= external/clang/lib/ARCMigrate/TransZeroOutPropsInDealloc.cpp
host StaticLib: libclangARCMigrate (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangARCMigrate_intermediates/libclangARCMigrate.a)
Host Clang TableGen: libclangDriver (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangDriver (gen-clang-diags-defs -clang-component=Driver) <= external/clang/include/clang/Basic/Diagnostic.td
Host TableGen: libclangDriver (gen-opt-parser-defs) <= external/clang/include/clang/Driver/Options.td
Host TableGen: libclangDriver (gen-opt-parser-defs) <= external/clang/include/clang/Driver/CC1AsOptions.td
Updating Clang version info.
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangDriver_intermediates/import_includes
host C++: libclangDriver <= external/clang/lib/Driver/Action.cpp
host C++: libclangDriver <= external/clang/lib/Driver/CC1AsOptions.cpp
host C++: libclangDriver <= external/clang/lib/Driver/Compilation.cpp
host C++: libclangDriver <= external/clang/lib/Driver/Driver.cpp
host C++: libclangDriver <= external/clang/lib/Driver/DriverOptions.cpp
host C++: libclangDriver <= external/clang/lib/Driver/Job.cpp
host C++: libclangDriver <= external/clang/lib/Driver/Phases.cpp
host C++: libclangDriver <= external/clang/lib/Driver/Tool.cpp
host C++: libclangDriver <= external/clang/lib/Driver/ToolChain.cpp
host C++: libclangDriver <= external/clang/lib/Driver/ToolChains.cpp
host C++: libclangDriver <= external/clang/lib/Driver/Tools.cpp
host C++: libclangDriver <= external/clang/lib/Driver/Types.cpp
host C++: libclangDriver <= external/clang/lib/Driver/WindowsToolChain.cpp
host StaticLib: libclangDriver (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangDriver_intermediates/libclangDriver.a)
Host Clang TableGen: libclangSerialization (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSerialization (gen-clang-attr-pch-read) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSerialization (gen-clang-attr-pch-write) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSerialization (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSerialization (gen-clang-attr-parsed-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSerialization (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangSerialization (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangSerialization (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSerialization (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSerialization (gen-clang-diags-defs -clang-component=Sema) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSerialization (gen-clang-diags-defs -clang-component=Serialization) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSerialization (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangSerialization (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Updating Clang version info.
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangSerialization_intermediates/import_includes
host C++: libclangSerialization <= external/clang/lib/Serialization/ASTCommon.cpp
host C++: libclangSerialization <= external/clang/lib/Serialization/ASTReader.cpp
host C++: libclangSerialization <= external/clang/lib/Serialization/ASTReaderDecl.cpp
host C++: libclangSerialization <= external/clang/lib/Serialization/ASTReaderStmt.cpp
external/clang/lib/Serialization/ASTReaderStmt.cpp: In member function 'clang::OMPClause* clang::OMPClauseReader::readClause()':
external/clang/lib/Serialization/ASTReaderStmt.cpp:2458:1: warning: 'C' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTReaderStmt.cpp:1683:14: note: 'C' was declared here
host C++: libclangSerialization <= external/clang/lib/Serialization/ASTWriter.cpp
external/clang/lib/Serialization/ASTWriter.cpp: In member function 'void clang::ASTWriter::WriteIdentifierTable(clang::Preprocessor&, clang::IdentifierResolver&, bool)':
external/clang/lib/Serialization/ASTWriter.cpp:3010:9: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTWriter.cpp:2987:20: note: 'isPublic' was declared here
external/clang/lib/Serialization/ASTWriter.cpp:3010:9: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTWriter.cpp:2987:20: note: 'isPublic' was declared here
external/clang/lib/Serialization/ASTWriter.cpp:3010:9: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTWriter.cpp:2987:20: note: 'isPublic' was declared here
external/clang/lib/Serialization/ASTWriter.cpp:3010:9: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTWriter.cpp:2987:20: note: 'isPublic' was declared here
external/clang/lib/Serialization/ASTWriter.cpp:3010:9: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTWriter.cpp:2987:20: note: 'isPublic' was declared here
external/clang/lib/Serialization/ASTWriter.cpp:3010:9: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTWriter.cpp:2987:20: note: 'isPublic' was declared here
external/clang/lib/Serialization/ASTWriter.cpp:3010:9: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTWriter.cpp:2987:20: note: 'isPublic' was declared here
external/clang/lib/Serialization/ASTWriter.cpp:3010:9: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Serialization/ASTWriter.cpp:2987:20: note: 'isPublic' was declared here
host C++: libclangSerialization <= external/clang/lib/Serialization/ASTWriterDecl.cpp
host C++: libclangSerialization <= external/clang/lib/Serialization/ASTWriterStmt.cpp
host C++: libclangSerialization <= external/clang/lib/Serialization/GeneratePCH.cpp
host C++: libclangSerialization <= external/clang/lib/Serialization/GlobalModuleIndex.cpp
host C++: libclangSerialization <= external/clang/lib/Serialization/Module.cpp
host C++: libclangSerialization <= external/clang/lib/Serialization/ModuleManager.cpp
host StaticLib: libclangSerialization (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangSerialization_intermediates/libclangSerialization.a)
Updating Clang version info.
Host Clang TableGen: libclangCodeGen (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangCodeGen (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangCodeGen (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangCodeGen (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangCodeGen (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangCodeGen (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangCodeGen (gen-clang-diags-defs -clang-component=Sema) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangCodeGen (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangCodeGen (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Host Clang TableGen: libclangCodeGen (gen-arm-neon-sema) <= external/clang/include/clang/Basic/arm_neon.td
Host TableGen: libclangCodeGen (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangCodeGen_intermediates/import_includes
host C++: libclangCodeGen <= external/clang/lib/CodeGen/BackendUtil.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGAtomic.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGBlocks.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGBuiltin.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGCUDANV.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGCUDARuntime.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGCXX.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGCXXABI.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGCall.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGClass.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGCleanup.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGDebugInfo.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGDecl.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGDeclCXX.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGException.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGExpr.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGExprAgg.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGExprCXX.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGExprComplex.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGExprConstant.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGExprScalar.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGObjC.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGObjCGNU.cpp
external/clang/lib/CodeGen/CGObjCGNU.cpp: In member function 'virtual clang::CodeGen::RValue (anonymous namespace)::CGObjCGNU::GenerateMessageSend(clang::CodeGen::CodeGenFunction&, clang::CodeGen::ReturnValueSlot, clang::QualType, clang::Selector, llvm::Value*, const clang::CodeGen::CallArgList&, const clang::ObjCInterfaceDecl*, const clang::ObjCMethodDecl*)':
external/clang/lib/CodeGen/CGObjCGNU.cpp:1439:53: warning: 'imp' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGObjCMac.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGObjCRuntime.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGOpenCLRuntime.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGRTTI.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGRecordLayoutBuilder.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGStmt.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGVTT.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CGVTables.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CodeGenAction.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CodeGenFunction.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CodeGenModule.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CodeGenTBAA.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/CodeGenTypes.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/ItaniumCXXABI.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/MicrosoftCXXABI.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/MicrosoftVBTables.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/ModuleBuilder.cpp
host C++: libclangCodeGen <= external/clang/lib/CodeGen/TargetInfo.cpp
external/llvm/include/llvm/IR/IRBuilder.h: In member function 'virtual llvm::Value* (anonymous namespace)::SparcV9ABIInfo::EmitVAArg(llvm::Value*, clang::QualType, clang::CodeGen::CodeGenFunction&) const':
external/llvm/include/llvm/IR/IRBuilder.h:928:66: warning: 'Stride' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/CodeGen/TargetInfo.cpp:5313:12: note: 'Stride' was declared here
external/clang/lib/CodeGen/TargetInfo.cpp:5475:1: warning: 'ArgAddr' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/CodeGen/TargetInfo.cpp:5312:16: note: 'ArgAddr' was declared here
host StaticLib: libclangCodeGen (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangCodeGen_intermediates/libclangCodeGen.a)
Host Clang TableGen: libclangRewriteFrontend (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangRewriteFrontend (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangRewriteFrontend (gen-clang-attr-parsed-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangRewriteFrontend (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangRewriteFrontend (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangRewriteFrontend (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangRewriteFrontend (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangRewriteFrontend (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangRewriteFrontend (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangRewriteFrontend_intermediates/import_includes
host C++: libclangRewriteFrontend <= external/clang/lib/Rewrite/Frontend/FixItRewriter.cpp
host C++: libclangRewriteFrontend <= external/clang/lib/Rewrite/Frontend/FrontendActions.cpp
host C++: libclangRewriteFrontend <= external/clang/lib/Rewrite/Frontend/HTMLPrint.cpp
host C++: libclangRewriteFrontend <= external/clang/lib/Rewrite/Frontend/InclusionRewriter.cpp
host C++: libclangRewriteFrontend <= external/clang/lib/Rewrite/Frontend/RewriteMacros.cpp
host C++: libclangRewriteFrontend <= external/clang/lib/Rewrite/Frontend/RewriteModernObjC.cpp
host C++: libclangRewriteFrontend <= external/clang/lib/Rewrite/Frontend/RewriteObjC.cpp
host C++: libclangRewriteFrontend <= external/clang/lib/Rewrite/Frontend/RewriteTest.cpp
host StaticLib: libclangRewriteFrontend (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangRewriteFrontend_intermediates/libclangRewriteFrontend.a)
Host Clang TableGen: libclangRewriteCore (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangRewriteCore (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangRewriteCore (gen-clang-attr-parsed-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangRewriteCore (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangRewriteCore (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangRewriteCore (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangRewriteCore (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangRewriteCore (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangRewriteCore_intermediates/import_includes
host C++: libclangRewriteCore <= external/clang/lib/Rewrite/Core/DeltaTree.cpp
host C++: libclangRewriteCore <= external/clang/lib/Rewrite/Core/HTMLRewrite.cpp
host C++: libclangRewriteCore <= external/clang/lib/Rewrite/Core/RewriteRope.cpp
host C++: libclangRewriteCore <= external/clang/lib/Rewrite/Core/Rewriter.cpp
host C++: libclangRewriteCore <= external/clang/lib/Rewrite/Core/TokenRewriter.cpp
host StaticLib: libclangRewriteCore (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangRewriteCore_intermediates/libclangRewriteCore.a)
Host Clang TableGen: libclangParse (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangParse (gen-clang-attr-expr-args-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangParse (gen-clang-attr-late-parsed-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangParse (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangParse (gen-clang-attr-parsed-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangParse (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangParse (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangParse (gen-clang-diags-defs -clang-component=Parse) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangParse (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangParse (gen-clang-diags-defs -clang-component=Sema) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangParse (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangParse (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangParse_intermediates/import_includes
host C++: libclangParse <= external/clang/lib/Parse/ParseAST.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseCXXInlineMethods.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseDecl.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseDeclCXX.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseExpr.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseExprCXX.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseInit.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseObjc.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseOpenMP.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParsePragma.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseStmt.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseTemplate.cpp
host C++: libclangParse <= external/clang/lib/Parse/ParseTentative.cpp
host C++: libclangParse <= external/clang/lib/Parse/Parser.cpp
host StaticLib: libclangParse (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangParse_intermediates/libclangParse.a)
Host Clang TableGen: libclangSema (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSema (gen-clang-attr-spelling-index) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSema (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSema (gen-clang-attr-parsed-attr-kinds) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSema (gen-clang-attr-parsed-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSema (gen-clang-attr-template-instantiate) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangSema (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangSema (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangSema (gen-clang-diags-defs -clang-component=AST) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSema (gen-clang-diags-defs -clang-component=Sema) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSema (gen-clang-diags-defs -clang-component=Parse) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSema (gen-clang-diags-defs -clang-component=Comment) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSema (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangSema (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangSema (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Host Clang TableGen: libclangSema (gen-arm-neon-sema) <= external/clang/include/clang/Basic/arm_neon.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangSema_intermediates/import_includes
host C++: libclangSema <= external/clang/lib/Sema/AnalysisBasedWarnings.cpp
host C++: libclangSema <= external/clang/lib/Sema/AttributeList.cpp
host C++: libclangSema <= external/clang/lib/Sema/CodeCompleteConsumer.cpp
host C++: libclangSema <= external/clang/lib/Sema/DeclSpec.cpp
host C++: libclangSema <= external/clang/lib/Sema/IdentifierResolver.cpp
host C++: libclangSema <= external/clang/lib/Sema/DelayedDiagnostic.cpp
host C++: libclangSema <= external/clang/lib/Sema/JumpDiagnostics.cpp
host C++: libclangSema <= external/clang/lib/Sema/MultiplexExternalSemaSource.cpp
host C++: libclangSema <= external/clang/lib/Sema/Scope.cpp
host C++: libclangSema <= external/clang/lib/Sema/ScopeInfo.cpp
host C++: libclangSema <= external/clang/lib/Sema/Sema.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaAccess.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaAttr.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaCXXScopeSpec.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaCast.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaChecking.cpp
external/clang/lib/Sema/SemaChecking.cpp: In member function 'void clang::Sema::checkCall(clang::NamedDecl*, llvm::ArrayRef<const clang::Expr*>, unsigned int, bool, clang::SourceLocation, clang::SourceRange, clang::Sema::VariadicCallType)':
external/clang/lib/Sema/SemaChecking.cpp:717:8: warning: variable 'HandledFormatString' set but not used [-Wunused-but-set-variable]
host C++: libclangSema <= external/clang/lib/Sema/SemaCodeComplete.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaConsumer.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaDecl.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaDeclAttr.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaDeclCXX.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaDeclObjC.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaExceptionSpec.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaExpr.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaExprCXX.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaExprMember.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaExprObjC.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaFixItUtils.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaInit.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaLambda.cpp
external/clang/lib/Sema/SemaLambda.cpp: In member function 'clang::ExprResult clang::Sema::ActOnLambdaExpr(clang::SourceLocation, clang::Stmt*, clang::Scope*, bool)':
external/clang/lib/Sema/SemaLambda.cpp:1059:74: warning: 'CaptureDefault' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libclangSema <= external/clang/lib/Sema/SemaLookup.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaObjCProperty.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaOpenMP.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaOverload.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaPseudoObject.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaStmt.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaStmtAsm.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaStmtAttr.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaTemplate.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaTemplateDeduction.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaTemplateInstantiate.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaTemplateInstantiateDecl.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaTemplateVariadic.cpp
host C++: libclangSema <= external/clang/lib/Sema/SemaType.cpp
host C++: libclangSema <= external/clang/lib/Sema/TargetAttributesSema.cpp
host C++: libclangSema <= external/clang/lib/Sema/TypeLocBuilder.cpp
host StaticLib: libclangSema (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangSema_intermediates/libclangSema.a)
Host Clang TableGen: libclangStaticAnalyzerFrontend (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangStaticAnalyzerFrontend (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangStaticAnalyzerFrontend (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangStaticAnalyzerFrontend (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangStaticAnalyzerFrontend (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangStaticAnalyzerFrontend (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangStaticAnalyzerFrontend (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangStaticAnalyzerFrontend (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Updating Clang version info.
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerFrontend_intermediates/import_includes
host C++: libclangStaticAnalyzerFrontend <= external/clang/lib/StaticAnalyzer/Frontend/AnalysisConsumer.cpp
host C++: libclangStaticAnalyzerFrontend <= external/clang/lib/StaticAnalyzer/Frontend/CheckerRegistration.cpp
host C++: libclangStaticAnalyzerFrontend <= external/clang/lib/StaticAnalyzer/Frontend/FrontendActions.cpp
host StaticLib: libclangStaticAnalyzerFrontend (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerFrontend_intermediates/libclangStaticAnalyzerFrontend.a)
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-attr-parsed-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-sa-checkers) <= external/clang/lib/StaticAnalyzer/Checkers/Checkers.td
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangStaticAnalyzerCheckers (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Updating Clang version info.
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerCheckers_intermediates/import_includes
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/AnalyzerStatsChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ArrayBoundChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ArrayBoundCheckerV2.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/BasicObjCFoundationChecks.cpp
external/clang/lib/StaticAnalyzer/Checkers/BasicObjCFoundationChecks.cpp: In member function 'void (anonymous namespace)::VariadicMethodTypeChecker::checkPreObjCMessage(const clang::ento::ObjCMethodCall&, clang::ento::CheckerContext&) const':
external/clang/lib/StaticAnalyzer/Checkers/BasicObjCFoundationChecks.cpp:779:69: warning: 'errorNode' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/BoolAssignmentChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/BuiltinFunctionChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CStringChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CStringSyntaxChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CallAndMessageChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CastSizeChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CastToStructChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CheckObjCDealloc.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CheckObjCInstMethSignature.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CheckSecuritySyntaxOnly.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CheckSizeofPointer.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CheckerDocumentation.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ChrootChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ClangCheckers.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/CommonBugCategories.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/DeadStoresChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/DebugCheckers.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/DereferenceChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/DirectIvarAssignment.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/DivZeroChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/DynamicTypePropagation.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ExprInspectionChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/FixedAddressChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/GenericTaintChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/IdempotentOperationChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/IvarInvalidationChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/LLVMConventionsChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/MacOSKeychainAPIChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/MacOSXAPIChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/MallocChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/MallocOverflowSecurityChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/MallocSizeofChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/NSAutoreleasePoolChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/NSErrorChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/NoReturnFunctionChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/NonNullParamChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ObjCAtSyncChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ObjCContainersASTChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ObjCContainersChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ObjCMissingSuperCallChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ObjCSelfInitChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ObjCUnusedIVarsChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/PointerArithChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/PointerSubChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/PthreadLockChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/RetainCountChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ReturnPointerRangeChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/ReturnUndefChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/SimpleStreamChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/StackAddrEscapeChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/StreamChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/TaintTesterChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/TraversalChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/UndefBranchChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/UndefCapturedBlockVarChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/UndefResultChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/UndefinedArraySubscriptChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/UndefinedAssignmentChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/UnixAPIChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/UnreachableCodeChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/VirtualCallChecker.cpp
host C++: libclangStaticAnalyzerCheckers <= external/clang/lib/StaticAnalyzer/Checkers/VLASizeChecker.cpp
host StaticLib: libclangStaticAnalyzerCheckers (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerCheckers_intermediates/libclangStaticAnalyzerCheckers.a)
Host Clang TableGen: libclangStaticAnalyzerCore (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangStaticAnalyzerCore (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangStaticAnalyzerCore (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangStaticAnalyzerCore (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangStaticAnalyzerCore (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangStaticAnalyzerCore (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangStaticAnalyzerCore (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Updating Clang version info.
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerCore_intermediates/import_includes
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/AnalysisManager.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/AnalyzerOptions.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/APSIntType.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/BasicValueFactory.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/BlockCounter.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/BugReporter.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/BugReporterVisitors.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/CallEvent.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/Checker.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/CheckerContext.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/CheckerHelpers.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/CheckerManager.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/CheckerRegistry.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/ConstraintManager.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/CoreEngine.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/Environment.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/ExplodedGraph.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/ExprEngine.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/ExprEngineC.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/ExprEngineCXX.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/ExprEngineCallAndReturn.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/ExprEngineObjC.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/FunctionSummary.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/HTMLDiagnostics.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/MemRegion.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/PathDiagnostic.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/PlistDiagnostics.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/ProgramState.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/RangeConstraintManager.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/RegionStore.cpp
external/clang/lib/StaticAnalyzer/Core/RegionStore.cpp: In member function '(anonymous namespace)::RegionBindingsRef (anonymous namespace)::RegionStoreManager::_ZN12_GLOBAL__N_118RegionStoreManager9bindArrayERKNS_17RegionBindingsRefEPKN5clang4ento16TypedValueRegionENS5_4SValE.constprop.605(RegionBindingsConstRef, const clang::ento::TypedValueRegion*, clang::ento::SVal)':
external/clang/lib/StaticAnalyzer/Core/RegionStore.cpp:2008:3: warning: 'Size' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/SValBuilder.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/SVals.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/SimpleConstraintManager.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/SimpleSValBuilder.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/Store.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/SubEngine.cpp
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/SymbolManager.cpp
external/clang/lib/StaticAnalyzer/Core/SymbolManager.cpp: In member function 'bool clang::ento::SymbolReaper::isLive(clang::ento::SymbolRef)':
external/clang/lib/StaticAnalyzer/Core/SymbolManager.cpp:484:3: warning: 'KnownLive' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libclangStaticAnalyzerCore <= external/clang/lib/StaticAnalyzer/Core/TextPathDiagnostics.cpp
host StaticLib: libclangStaticAnalyzerCore (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangStaticAnalyzerCore_intermediates/libclangStaticAnalyzerCore.a)
Host Clang TableGen: libclangAnalysis (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangAnalysis (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangAnalysis (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangAnalysis (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangAnalysis (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangAnalysis (gen-clang-diags-defs -clang-component=Analysis) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangAnalysis (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangAnalysis (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangAnalysis_intermediates/import_includes
host C++: libclangAnalysis <= external/clang/lib/Analysis/AnalysisDeclContext.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/BodyFarm.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/CallGraph.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/CFG.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/CFGReachabilityAnalysis.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/CFGStmtMap.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/CocoaConventions.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/Dominators.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/FormatString.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/LiveVariables.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/ObjCNoReturn.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/PostOrderCFGView.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/PrintfFormatString.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/ProgramPoint.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/PseudoConstantAnalysis.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/ReachableCode.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/ScanfFormatString.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/ThreadSafety.cpp
host C++: libclangAnalysis <= external/clang/lib/Analysis/UninitializedValues.cpp
host StaticLib: libclangAnalysis (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangAnalysis_intermediates/libclangAnalysis.a)
Updating Clang version info.
Host Clang TableGen: libclangEdit (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangEdit (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangEdit (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangEdit (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangEdit (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangEdit (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangEdit (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangEdit_intermediates/import_includes
host C++: libclangEdit <= external/clang/lib/Edit/Commit.cpp
host C++: libclangEdit <= external/clang/lib/Edit/EditedSource.cpp
host C++: libclangEdit <= external/clang/lib/Edit/RewriteObjCFoundationAPI.cpp
external/clang/lib/Edit/RewriteObjCFoundationAPI.cpp: In function 'bool rewriteToNumberLiteral(const clang::ObjCMessageExpr*, const clang::NSAPI&, clang::edit::Commit&)':
external/clang/lib/Edit/RewriteObjCFoundationAPI.cpp:737:31: warning: 'UpperL' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Edit/RewriteObjCFoundationAPI.cpp:696:26: note: 'UpperL' was declared here
host StaticLib: libclangEdit (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangEdit_intermediates/libclangEdit.a)
Host Clang TableGen: libclangAST (gen-clang-attr-dump) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangAST (gen-clang-attr-impl) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangAST (gen-clang-attr-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangAST (gen-clang-attr-classes) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangAST (gen-clang-comment-command-info) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangAST (gen-clang-comment-command-list) <= external/clang/include/clang/AST/CommentCommands.td
Host Clang TableGen: libclangAST (gen-clang-comment-html-named-character-references) <= external/clang/include/clang/AST/CommentHTMLNamedCharacterReferences.td
Host Clang TableGen: libclangAST (gen-clang-comment-html-tags-properties) <= external/clang/include/clang/AST/CommentHTMLTags.td
Host Clang TableGen: libclangAST (gen-clang-comment-html-tags) <= external/clang/include/clang/AST/CommentHTMLTags.td
Host Clang TableGen: libclangAST (gen-clang-comment-nodes) <= external/clang/include/clang/Basic/CommentNodes.td
Host Clang TableGen: libclangAST (gen-clang-diags-defs -clang-component=AST) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangAST (gen-clang-diags-defs -clang-component=Comment) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangAST (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangAST (gen-clang-diags-defs -clang-component=Sema) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangAST (gen-clang-decl-nodes) <= external/clang/include/clang/Basic/DeclNodes.td
Host Clang TableGen: libclangAST (gen-clang-stmt-nodes) <= external/clang/include/clang/Basic/StmtNodes.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangAST_intermediates/import_includes
host C++: libclangAST <= external/clang/lib/AST/APValue.cpp
host C++: libclangAST <= external/clang/lib/AST/ASTConsumer.cpp
host C++: libclangAST <= external/clang/lib/AST/ASTContext.cpp
host C++: libclangAST <= external/clang/lib/AST/ASTDiagnostic.cpp
host C++: libclangAST <= external/clang/lib/AST/ASTDumper.cpp
host C++: libclangAST <= external/clang/lib/AST/ASTImporter.cpp
host C++: libclangAST <= external/clang/lib/AST/ASTTypeTraits.cpp
host C++: libclangAST <= external/clang/lib/AST/AttrImpl.cpp
host C++: libclangAST <= external/clang/lib/AST/Comment.cpp
host C++: libclangAST <= external/clang/lib/AST/CommentBriefParser.cpp
host C++: libclangAST <= external/clang/lib/AST/CommentCommandTraits.cpp
host C++: libclangAST <= external/clang/lib/AST/CommentLexer.cpp
host C++: libclangAST <= external/clang/lib/AST/CommentParser.cpp
host C++: libclangAST <= external/clang/lib/AST/CommentSema.cpp
host C++: libclangAST <= external/clang/lib/AST/CXXInheritance.cpp
host C++: libclangAST <= external/clang/lib/AST/Decl.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclarationName.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclBase.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclCXX.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclFriend.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclGroup.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclObjC.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclOpenMP.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclPrinter.cpp
host C++: libclangAST <= external/clang/lib/AST/DeclTemplate.cpp
host C++: libclangAST <= external/clang/lib/AST/DumpXML.cpp
host C++: libclangAST <= external/clang/lib/AST/Expr.cpp
host C++: libclangAST <= external/clang/lib/AST/ExprClassification.cpp
host C++: libclangAST <= external/clang/lib/AST/ExprConstant.cpp
external/clang/include/clang/AST/Expr.h: In member function 'bool (anonymous namespace)::IntExprEvaluator::VisitCallExpr(const clang::CallExpr*)':
external/clang/include/clang/AST/Expr.h:2196:65: warning: 'Arg' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/AST/ExprConstant.cpp:5959:14: note: 'Arg' was declared here
host C++: libclangAST <= external/clang/lib/AST/ExprCXX.cpp
host C++: libclangAST <= external/clang/lib/AST/ExternalASTSource.cpp
host C++: libclangAST <= external/clang/lib/AST/InheritViz.cpp
host C++: libclangAST <= external/clang/lib/AST/ItaniumCXXABI.cpp
host C++: libclangAST <= external/clang/lib/AST/ItaniumMangle.cpp
host C++: libclangAST <= external/clang/lib/AST/Mangle.cpp
host C++: libclangAST <= external/clang/lib/AST/MangleNumberingContext.cpp
host C++: libclangAST <= external/clang/lib/AST/MicrosoftCXXABI.cpp
host C++: libclangAST <= external/clang/lib/AST/MicrosoftMangle.cpp
host C++: libclangAST <= external/clang/lib/AST/NestedNameSpecifier.cpp
host C++: libclangAST <= external/clang/lib/AST/NSAPI.cpp
host C++: libclangAST <= external/clang/lib/AST/ParentMap.cpp
host C++: libclangAST <= external/clang/lib/AST/RecordLayout.cpp
host C++: libclangAST <= external/clang/lib/AST/RecordLayoutBuilder.cpp
host C++: libclangAST <= external/clang/lib/AST/RawCommentList.cpp
host C++: libclangAST <= external/clang/lib/AST/SelectorLocationsKind.cpp
host C++: libclangAST <= external/clang/lib/AST/Stmt.cpp
host C++: libclangAST <= external/clang/lib/AST/StmtIterator.cpp
host C++: libclangAST <= external/clang/lib/AST/StmtPrinter.cpp
host C++: libclangAST <= external/clang/lib/AST/StmtProfile.cpp
host C++: libclangAST <= external/clang/lib/AST/StmtViz.cpp
host C++: libclangAST <= external/clang/lib/AST/TemplateBase.cpp
host C++: libclangAST <= external/clang/lib/AST/TemplateName.cpp
host C++: libclangAST <= external/clang/lib/AST/Type.cpp
host C++: libclangAST <= external/clang/lib/AST/TypeLoc.cpp
host C++: libclangAST <= external/clang/lib/AST/TypePrinter.cpp
host C++: libclangAST <= external/clang/lib/AST/VTTBuilder.cpp
host C++: libclangAST <= external/clang/lib/AST/VTableBuilder.cpp
host StaticLib: libclangAST (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangAST_intermediates/libclangAST.a)
Host Clang TableGen: libclangLex (gen-clang-attr-spelling-list) <= external/clang/include/clang/Basic/Attr.td
Host Clang TableGen: libclangLex (gen-clang-diags-defs -clang-component=Lex) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangLex (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangLex_intermediates/import_includes
host C++: libclangLex <= external/clang/lib/Lex/HeaderMap.cpp
host C++: libclangLex <= external/clang/lib/Lex/HeaderSearch.cpp
host C++: libclangLex <= external/clang/lib/Lex/Lexer.cpp
host C++: libclangLex <= external/clang/lib/Lex/LiteralSupport.cpp
host C++: libclangLex <= external/clang/lib/Lex/MacroArgs.cpp
host C++: libclangLex <= external/clang/lib/Lex/MacroInfo.cpp
external/clang/include/clang/Lex/MacroInfo.h: In member function 'clang::MacroDirective::DefInfo clang::MacroDirective::getDefinition(bool)':
external/clang/include/clang/Lex/MacroInfo.h:405:74: warning: 'isPublic' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/clang/lib/Lex/MacroInfo.cpp:131:18: note: 'isPublic' was declared here
host C++: libclangLex <= external/clang/lib/Lex/ModuleMap.cpp
host C++: libclangLex <= external/clang/lib/Lex/PPCaching.cpp
host C++: libclangLex <= external/clang/lib/Lex/PPCallbacks.cpp
host C++: libclangLex <= external/clang/lib/Lex/PPConditionalDirectiveRecord.cpp
host C++: libclangLex <= external/clang/lib/Lex/PPDirectives.cpp
host C++: libclangLex <= external/clang/lib/Lex/PPExpressions.cpp
host C++: libclangLex <= external/clang/lib/Lex/PPLexerChange.cpp
host C++: libclangLex <= external/clang/lib/Lex/PPMacroExpansion.cpp
host C++: libclangLex <= external/clang/lib/Lex/PTHLexer.cpp
host C++: libclangLex <= external/clang/lib/Lex/Pragma.cpp
host C++: libclangLex <= external/clang/lib/Lex/PreprocessingRecord.cpp
host C++: libclangLex <= external/clang/lib/Lex/Preprocessor.cpp
host C++: libclangLex <= external/clang/lib/Lex/PreprocessorLexer.cpp
host C++: libclangLex <= external/clang/lib/Lex/ScratchBuffer.cpp
host C++: libclangLex <= external/clang/lib/Lex/TokenConcatenation.cpp
host C++: libclangLex <= external/clang/lib/Lex/TokenLexer.cpp
host StaticLib: libclangLex (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangLex_intermediates/libclangLex.a)
Updating Clang version info.
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=AST) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Analysis) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Comment) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Common) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Driver) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Frontend) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Lex) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Parse) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Sema) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diags-defs -clang-component=Serialization) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diag-groups) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-clang-diag-groups) <= external/clang/include/clang/Basic/Diagnostic.td
Host Clang TableGen: libclangBasic (gen-arm-neon-sema) <= external/clang/include/clang/Basic/arm_neon.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangBasic_intermediates/import_includes
host C++: libclangBasic <= external/clang/lib/Basic/Builtins.cpp
host C++: libclangBasic <= external/clang/lib/Basic/CharInfo.cpp
host C++: libclangBasic <= external/clang/lib/Basic/Diagnostic.cpp
host C++: libclangBasic <= external/clang/lib/Basic/DiagnosticIDs.cpp
host C++: libclangBasic <= external/clang/lib/Basic/FileManager.cpp
host C++: libclangBasic <= external/clang/lib/Basic/FileSystemStatCache.cpp
host C++: libclangBasic <= external/clang/lib/Basic/IdentifierTable.cpp
host C++: libclangBasic <= external/clang/lib/Basic/LangOptions.cpp
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Address' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::InitOrder' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::UseAfterReturn' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::UseAfterScope' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Memory' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Thread' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Leak' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Alignment' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Bool' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Bounds' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Enum' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::FloatCastOverflow' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::FloatDivideByZero' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::IntegerDivideByZero' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Null' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::ObjectSize' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Return' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Shift' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::SignedIntegerOverflow' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Unreachable' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::VLABound' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::Vptr' [-Wmissing-field-initializers]
external/clang/lib/Basic/LangOptions.cpp:17:54: warning: missing initializer for member 'clang::SanitizerOptions::UnsignedIntegerOverflow' [-Wmissing-field-initializers]
host C++: libclangBasic <= external/clang/lib/Basic/Module.cpp
host C++: libclangBasic <= external/clang/lib/Basic/ObjCRuntime.cpp
host C++: libclangBasic <= external/clang/lib/Basic/OpenMPKinds.cpp
host C++: libclangBasic <= external/clang/lib/Basic/OperatorPrecedence.cpp
host C++: libclangBasic <= external/clang/lib/Basic/SourceLocation.cpp
host C++: libclangBasic <= external/clang/lib/Basic/SourceManager.cpp
host C++: libclangBasic <= external/clang/lib/Basic/TargetInfo.cpp
host C++: libclangBasic <= external/clang/lib/Basic/Targets.cpp
host C++: libclangBasic <= external/clang/lib/Basic/TokenKinds.cpp
host C++: libclangBasic <= external/clang/lib/Basic/Version.cpp
host C++: libclangBasic <= external/clang/lib/Basic/VersionTuple.cpp
host StaticLib: libclangBasic (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libclangBasic_intermediates/libclangBasic.a)
Host TableGen: libLLVMARMAsmParser (gen-instr-info) <= external/llvm/lib/Target/ARM/AsmParser/../ARM.td
Host TableGen: libLLVMARMAsmParser (gen-register-info) <= external/llvm/lib/Target/ARM/AsmParser/../ARM.td
Host TableGen: libLLVMARMAsmParser (gen-asm-matcher) <= external/llvm/lib/Target/ARM/AsmParser/../ARM.td
Host TableGen: libLLVMARMAsmParser (gen-subtarget) <= external/llvm/lib/Target/ARM/AsmParser/../ARM.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMAsmParser_intermediates/import_includes
host C++: libLLVMARMAsmParser <= external/llvm/lib/Target/ARM/AsmParser/ARMAsmParser.cpp
host StaticLib: libLLVMARMAsmParser (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMAsmParser_intermediates/libLLVMARMAsmParser.a)
Host TableGen: libLLVMARMCodeGen (gen-register-info) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-instr-info) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-emitter) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-emitter -mc-emitter) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-pseudo-lowering) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-asm-writer) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-asm-matcher) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-dag-isel) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-fast-isel) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-callingconv) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-subtarget) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-disassembler) <= external/llvm/lib/Target/ARM/ARM.td
Host TableGen: libLLVMARMCodeGen (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMCodeGen_intermediates/import_includes
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/A15SDOptimizer.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMAsmPrinter.cpp
external/llvm/lib/Target/ARM/ARMAsmPrinter.cpp: In member function 'virtual bool llvm::ARMAsmPrinter::PrintAsmOperand(const llvm::MachineInstr*, unsigned int, unsigned int, char const*, llvm::raw_ostream&)':
external/llvm/lib/Target/ARM/ARMAsmPrinter.cpp:502:7: warning: 'RC' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMBaseInstrInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMBaseRegisterInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMCodeEmitter.cpp
external/llvm/lib/Target/ARM/ARMCodeEmitter.cpp: In member function 'uint32_t (anonymous namespace)::ARMCodeEmitter::getAddrMode5OpValue(const llvm::MachineInstr&, unsigned int) const':
external/llvm/lib/Target/ARM/ARMCodeEmitter.cpp:324:16: warning: unused variable 'Reg' [-Wunused-variable]
external/llvm/lib/Target/ARM/ARMCodeEmitter.cpp:333:12: warning: variable 'isAdd' set but not used [-Wunused-but-set-variable]
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMConstantIslandPass.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMConstantPoolValue.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMExpandPseudoInsts.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMFastISel.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMFrameLowering.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMHazardRecognizer.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMISelDAGToDAG.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMISelLowering.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMInstrInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMJITInfo.cpp
external/llvm/lib/Target/ARM/ARMJITInfo.cpp: In member function 'virtual void llvm::ARMJITInfo::relocate(void*, llvm::MachineRelocation*, unsigned int, unsigned char*)':
external/llvm/lib/Target/ARM/ARMJITInfo.cpp:272:12: warning: enumeration value 'reloc_arm_so_imm_cp_entry' not handled in switch [-Wswitch]
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMLoadStoreOptimizer.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMMCInstLower.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMMachineFunctionInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMRegisterInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMSelectionDAGInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMSubtarget.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMTargetMachine.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMTargetObjectFile.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/ARMTargetTransformInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/MLxExpansionPass.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/Thumb1FrameLowering.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/Thumb1InstrInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/Thumb1RegisterInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/Thumb2ITBlockPass.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/Thumb2InstrInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/Thumb2RegisterInfo.cpp
host C++: libLLVMARMCodeGen <= external/llvm/lib/Target/ARM/Thumb2SizeReduction.cpp
host StaticLib: libLLVMARMCodeGen (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMCodeGen_intermediates/libLLVMARMCodeGen.a)
Host TableGen: libLLVMARMAsmPrinter (gen-asm-writer) <= external/llvm/lib/Target/ARM/InstPrinter/../ARM.td
Host TableGen: libLLVMARMAsmPrinter (gen-register-info) <= external/llvm/lib/Target/ARM/InstPrinter/../ARM.td
Host TableGen: libLLVMARMAsmPrinter (gen-subtarget) <= external/llvm/lib/Target/ARM/InstPrinter/../ARM.td
Host TableGen: libLLVMARMAsmPrinter (gen-instr-info) <= external/llvm/lib/Target/ARM/InstPrinter/../ARM.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMAsmPrinter_intermediates/import_includes
host C++: libLLVMARMAsmPrinter <= external/llvm/lib/Target/ARM/InstPrinter/ARMInstPrinter.cpp
host StaticLib: libLLVMARMAsmPrinter (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMAsmPrinter_intermediates/libLLVMARMAsmPrinter.a)
Host TableGen: libLLVMARMDisassembler (gen-disassembler) <= external/llvm/lib/Target/ARM/Disassembler/../ARM.td
Host TableGen: libLLVMARMDisassembler (gen-instr-info) <= external/llvm/lib/Target/ARM/Disassembler/../ARM.td
Host TableGen: libLLVMARMDisassembler (gen-subtarget) <= external/llvm/lib/Target/ARM/Disassembler/../ARM.td
Host TableGen: libLLVMARMDisassembler (gen-register-info) <= external/llvm/lib/Target/ARM/Disassembler/../ARM.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMDisassembler_intermediates/import_includes
host C++: libLLVMARMDisassembler <= external/llvm/lib/Target/ARM/Disassembler/ARMDisassembler.cpp
host StaticLib: libLLVMARMDisassembler (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMDisassembler_intermediates/libLLVMARMDisassembler.a)
Host TableGen: libLLVMARMDesc (gen-register-info) <= external/llvm/lib/Target/ARM/MCTargetDesc/../ARM.td
Host TableGen: libLLVMARMDesc (gen-instr-info) <= external/llvm/lib/Target/ARM/MCTargetDesc/../ARM.td
Host TableGen: libLLVMARMDesc (gen-emitter -mc-emitter) <= external/llvm/lib/Target/ARM/MCTargetDesc/../ARM.td
Host TableGen: libLLVMARMDesc (gen-subtarget) <= external/llvm/lib/Target/ARM/MCTargetDesc/../ARM.td
Host TableGen: libLLVMARMDesc (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMDesc_intermediates/import_includes
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMAsmBackend.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMELFObjectWriter.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMELFStreamer.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMMCAsmInfo.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMMCCodeEmitter.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMMCExpr.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMMCTargetDesc.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMMachObjectWriter.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMMachORelocationInfo.cpp
host C++: libLLVMARMDesc <= external/llvm/lib/Target/ARM/MCTargetDesc/ARMUnwindOpAsm.cpp
host StaticLib: libLLVMARMDesc (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMDesc_intermediates/libLLVMARMDesc.a)
Host TableGen: libLLVMARMInfo (gen-subtarget) <= external/llvm/lib/Target/ARM/TargetInfo/../ARM.td
Host TableGen: libLLVMARMInfo (gen-register-info) <= external/llvm/lib/Target/ARM/TargetInfo/../ARM.td
Host TableGen: libLLVMARMInfo (gen-instr-info) <= external/llvm/lib/Target/ARM/TargetInfo/../ARM.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMInfo_intermediates/import_includes
host C++: libLLVMARMInfo <= external/llvm/lib/Target/ARM/TargetInfo/ARMTargetInfo.cpp
host StaticLib: libLLVMARMInfo (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMARMInfo_intermediates/libLLVMARMInfo.a)
Host TableGen: libLLVMMipsAsmParser (gen-asm-matcher) <= external/llvm/lib/Target/Mips/AsmParser/../Mips.td
Host TableGen: libLLVMMipsAsmParser (gen-instr-info) <= external/llvm/lib/Target/Mips/AsmParser/../Mips.td
Host TableGen: libLLVMMipsAsmParser (gen-register-info) <= external/llvm/lib/Target/Mips/AsmParser/../Mips.td
Host TableGen: libLLVMMipsAsmParser (gen-subtarget) <= external/llvm/lib/Target/Mips/AsmParser/../Mips.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsAsmParser_intermediates/import_includes
host C++: libLLVMMipsAsmParser <= external/llvm/lib/Target/Mips/AsmParser/MipsAsmParser.cpp
/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsAsmParser_intermediates/MipsGenAsmMatcher.inc: In member function 'void (anonymous namespace)::MipsAsmParser::_ZN12_GLOBAL__N_113MipsAsmParser13expandMemInstERN4llvm6MCInstENS1_5SMLocERNS1_15SmallVectorImplIS2_EEbb.constprop.167(llvm::MCInst&, llvm::SMLoc, llvm::SmallVectorImpl<llvm::MCInst>&, bool, bool)':
/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsAsmParser_intermediates/MipsGenAsmMatcher.inc:2330:1: warning: 'SR' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/lib/Target/Mips/AsmParser/MipsAsmParser.cpp:647:26: note: 'SR' was declared here
external/llvm/lib/Target/Mips/AsmParser/MipsAsmParser.cpp:710:54: warning: 'LoOffset' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/lib/Target/Mips/AsmParser/MipsAsmParser.cpp:680:54: warning: 'HiOffset' may be used uninitialized in this function [-Wmaybe-uninitialized]
host StaticLib: libLLVMMipsAsmParser (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsAsmParser_intermediates/libLLVMMipsAsmParser.a)
Host TableGen: libLLVMMipsCodeGen (gen-register-info) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-instr-info) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-emitter) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-emitter -mc-emitter) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-pseudo-lowering) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-asm-writer) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-dag-isel) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-callingconv) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-subtarget) <= external/llvm/lib/Target/Mips/Mips.td
Host TableGen: libLLVMMipsCodeGen (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsCodeGen_intermediates/import_includes
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/Mips16FrameLowering.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/Mips16HardFloat.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/Mips16ISelDAGToDAG.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/Mips16ISelLowering.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/Mips16InstrInfo.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/Mips16RegisterInfo.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsAnalyzeImmediate.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsAsmPrinter.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsCodeEmitter.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsConstantIslandPass.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsDelaySlotFiller.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsFrameLowering.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsInstrInfo.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsISelDAGToDAG.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsISelLowering.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsJITInfo.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsLongBranch.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsMachineFunction.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsMCInstLower.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsModuleISelDAGToDAG.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsOptimizeMathLibCalls.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsOs16.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsRegisterInfo.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsSEFrameLowering.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsSEISelDAGToDAG.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsSEISelLowering.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsSEInstrInfo.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsSERegisterInfo.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsSelectionDAGInfo.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsSubtarget.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsTargetMachine.cpp
host C++: libLLVMMipsCodeGen <= external/llvm/lib/Target/Mips/MipsTargetObjectFile.cpp
host StaticLib: libLLVMMipsCodeGen (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsCodeGen_intermediates/libLLVMMipsCodeGen.a)
Host TableGen: libLLVMMipsDisassembler (gen-disassembler) <= external/llvm/lib/Target/Mips/Disassembler/../Mips.td
Host TableGen: libLLVMMipsDisassembler (gen-instr-info) <= external/llvm/lib/Target/Mips/Disassembler/../Mips.td
Host TableGen: libLLVMMipsDisassembler (gen-register-info) <= external/llvm/lib/Target/Mips/Disassembler/../Mips.td
Host TableGen: libLLVMMipsDisassembler (gen-subtarget) <= external/llvm/lib/Target/Mips/Disassembler/../Mips.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsDisassembler_intermediates/import_includes
host C++: libLLVMMipsDisassembler <= external/llvm/lib/Target/Mips/Disassembler/MipsDisassembler.cpp
host StaticLib: libLLVMMipsDisassembler (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsDisassembler_intermediates/libLLVMMipsDisassembler.a)
Host TableGen: libLLVMMipsAsmPrinter (gen-asm-writer) <= external/llvm/lib/Target/Mips/InstPrinter/../Mips.td
Host TableGen: libLLVMMipsAsmPrinter (gen-register-info) <= external/llvm/lib/Target/Mips/InstPrinter/../Mips.td
Host TableGen: libLLVMMipsAsmPrinter (gen-subtarget) <= external/llvm/lib/Target/Mips/InstPrinter/../Mips.td
Host TableGen: libLLVMMipsAsmPrinter (gen-instr-info) <= external/llvm/lib/Target/Mips/InstPrinter/../Mips.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsAsmPrinter_intermediates/import_includes
host C++: libLLVMMipsAsmPrinter <= external/llvm/lib/Target/Mips/InstPrinter/MipsInstPrinter.cpp
host StaticLib: libLLVMMipsAsmPrinter (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsAsmPrinter_intermediates/libLLVMMipsAsmPrinter.a)
Host TableGen: libLLVMMipsDesc (gen-register-info) <= external/llvm/lib/Target/Mips/MCTargetDesc/../Mips.td
Host TableGen: libLLVMMipsDesc (gen-instr-info) <= external/llvm/lib/Target/Mips/MCTargetDesc/../Mips.td
Host TableGen: libLLVMMipsDesc (gen-emitter -mc-emitter) <= external/llvm/lib/Target/Mips/MCTargetDesc/../Mips.td
Host TableGen: libLLVMMipsDesc (gen-subtarget) <= external/llvm/lib/Target/Mips/MCTargetDesc/../Mips.td
Host TableGen: libLLVMMipsDesc (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsDesc_intermediates/import_includes
host C++: libLLVMMipsDesc <= external/llvm/lib/Target/Mips/MCTargetDesc/MipsAsmBackend.cpp
host C++: libLLVMMipsDesc <= external/llvm/lib/Target/Mips/MCTargetDesc/MipsELFObjectWriter.cpp
host C++: libLLVMMipsDesc <= external/llvm/lib/Target/Mips/MCTargetDesc/MipsELFStreamer.cpp
host C++: libLLVMMipsDesc <= external/llvm/lib/Target/Mips/MCTargetDesc/MipsMCAsmInfo.cpp
host C++: libLLVMMipsDesc <= external/llvm/lib/Target/Mips/MCTargetDesc/MipsMCCodeEmitter.cpp
host C++: libLLVMMipsDesc <= external/llvm/lib/Target/Mips/MCTargetDesc/MipsMCTargetDesc.cpp
host C++: libLLVMMipsDesc <= external/llvm/lib/Target/Mips/MCTargetDesc/MipsReginfo.cpp
host StaticLib: libLLVMMipsDesc (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsDesc_intermediates/libLLVMMipsDesc.a)
Host TableGen: libLLVMMipsInfo (gen-instr-info) <= external/llvm/lib/Target/Mips/TargetInfo/../Mips.td
Host TableGen: libLLVMMipsInfo (gen-register-info) <= external/llvm/lib/Target/Mips/TargetInfo/../Mips.td
Host TableGen: libLLVMMipsInfo (gen-subtarget) <= external/llvm/lib/Target/Mips/TargetInfo/../Mips.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsInfo_intermediates/import_includes
host C++: libLLVMMipsInfo <= external/llvm/lib/Target/Mips/TargetInfo/MipsTargetInfo.cpp
host StaticLib: libLLVMMipsInfo (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMipsInfo_intermediates/libLLVMMipsInfo.a)
Host TableGen: libLLVMX86Info (gen-register-info) <= external/llvm/lib/Target/X86/TargetInfo/../X86.td
Host TableGen: libLLVMX86Info (gen-subtarget) <= external/llvm/lib/Target/X86/TargetInfo/../X86.td
Host TableGen: libLLVMX86Info (gen-instr-info) <= external/llvm/lib/Target/X86/TargetInfo/../X86.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Info_intermediates/import_includes
host C++: libLLVMX86Info <= external/llvm/lib/Target/X86/TargetInfo/X86TargetInfo.cpp
host StaticLib: libLLVMX86Info (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Info_intermediates/libLLVMX86Info.a)
Host TableGen: libLLVMX86AsmParser (gen-asm-matcher) <= external/llvm/lib/Target/X86/AsmParser/../X86.td
Host TableGen: libLLVMX86AsmParser (gen-instr-info) <= external/llvm/lib/Target/X86/AsmParser/../X86.td
Host TableGen: libLLVMX86AsmParser (gen-register-info) <= external/llvm/lib/Target/X86/AsmParser/../X86.td
Host TableGen: libLLVMX86AsmParser (gen-subtarget) <= external/llvm/lib/Target/X86/AsmParser/../X86.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86AsmParser_intermediates/import_includes
host C++: libLLVMX86AsmParser <= external/llvm/lib/Target/X86/AsmParser/X86AsmParser.cpp
external/llvm/lib/Target/X86/AsmParser/X86AsmParser.cpp: In member function '(anonymous namespace)::X86Operand* (anonymous namespace)::X86AsmParser::ParseIntelBracExpression(unsigned int, llvm::SMLoc, int64_t, unsigned int)':
external/llvm/lib/Target/X86/AsmParser/X86AsmParser.cpp:1391:64: warning: 'NewDisp' may be used uninitialized in this function [-Wmaybe-uninitialized]
host StaticLib: libLLVMX86AsmParser (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86AsmParser_intermediates/libLLVMX86AsmParser.a)
Host TableGen: libLLVMX86CodeGen (gen-asm-writer) <= external/llvm/lib/Target/X86/X86.td
Host TableGen: libLLVMX86CodeGen (gen-asm-writer -asmwriternum=1) <= external/llvm/lib/Target/X86/X86.td
Host TableGen: libLLVMX86CodeGen (gen-register-info) <= external/llvm/lib/Target/X86/X86.td
Host TableGen: libLLVMX86CodeGen (gen-instr-info) <= external/llvm/lib/Target/X86/X86.td
Host TableGen: libLLVMX86CodeGen (gen-dag-isel) <= external/llvm/lib/Target/X86/X86.td
Host TableGen: libLLVMX86CodeGen (gen-fast-isel) <= external/llvm/lib/Target/X86/X86.td
Host TableGen: libLLVMX86CodeGen (gen-subtarget) <= external/llvm/lib/Target/X86/X86.td
Host TableGen: libLLVMX86CodeGen (gen-callingconv) <= external/llvm/lib/Target/X86/X86.td
Host TableGen: libLLVMX86CodeGen (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86CodeGen_intermediates/import_includes
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86AsmPrinter.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86COFFMachineModuleInfo.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86CodeEmitter.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86FastISel.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86FixupLEAs.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86FloatingPoint.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86FrameLowering.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86ISelDAGToDAG.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86ISelLowering.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86InstrInfo.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86JITInfo.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86MachineFunctionInfo.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86MCInstLower.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86PadShortFunction.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86RegisterInfo.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86SelectionDAGInfo.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86Subtarget.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86TargetMachine.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86TargetObjectFile.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86TargetTransformInfo.cpp
host C++: libLLVMX86CodeGen <= external/llvm/lib/Target/X86/X86VZeroUpper.cpp
host StaticLib: libLLVMX86CodeGen (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86CodeGen_intermediates/libLLVMX86CodeGen.a)
Host TableGen: libLLVMX86Disassembler (gen-disassembler) <= external/llvm/lib/Target/X86/Disassembler/../X86.td
Host TableGen: libLLVMX86Disassembler (gen-instr-info) <= external/llvm/lib/Target/X86/Disassembler/../X86.td
Host TableGen: libLLVMX86Disassembler (gen-register-info) <= external/llvm/lib/Target/X86/Disassembler/../X86.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Disassembler_intermediates/import_includes
host C++: libLLVMX86Disassembler <= external/llvm/lib/Target/X86/Disassembler/X86Disassembler.cpp
host C: libLLVMX86Disassembler <= external/llvm/lib/Target/X86/Disassembler/X86DisassemblerDecoder.c
host StaticLib: libLLVMX86Disassembler (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Disassembler_intermediates/libLLVMX86Disassembler.a)
Host TableGen: libLLVMX86Desc (gen-register-info) <= external/llvm/lib/Target/X86/MCTargetDesc/../X86.td
Host TableGen: libLLVMX86Desc (gen-instr-info) <= external/llvm/lib/Target/X86/MCTargetDesc/../X86.td
Host TableGen: libLLVMX86Desc (gen-subtarget) <= external/llvm/lib/Target/X86/MCTargetDesc/../X86.td
Host TableGen: libLLVMX86Desc (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Desc_intermediates/import_includes
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86AsmBackend.cpp
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86ELFObjectWriter.cpp
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86ELFRelocationInfo.cpp
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86MCTargetDesc.cpp
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86MCAsmInfo.cpp
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86MCCodeEmitter.cpp
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86MachORelocationInfo.cpp
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86MachObjectWriter.cpp
host C++: libLLVMX86Desc <= external/llvm/lib/Target/X86/MCTargetDesc/X86WinCOFFObjectWriter.cpp
host StaticLib: libLLVMX86Desc (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Desc_intermediates/libLLVMX86Desc.a)
Host TableGen: libLLVMX86AsmPrinter (gen-asm-writer) <= external/llvm/lib/Target/X86/InstPrinter/../X86.td
Host TableGen: libLLVMX86AsmPrinter (gen-asm-writer -asmwriternum=1) <= external/llvm/lib/Target/X86/InstPrinter/../X86.td
Host TableGen: libLLVMX86AsmPrinter (gen-instr-info) <= external/llvm/lib/Target/X86/InstPrinter/../X86.td
Host TableGen: libLLVMX86AsmPrinter (gen-register-info) <= external/llvm/lib/Target/X86/InstPrinter/../X86.td
Host TableGen: libLLVMX86AsmPrinter (gen-subtarget) <= external/llvm/lib/Target/X86/InstPrinter/../X86.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86AsmPrinter_intermediates/import_includes
host C++: libLLVMX86AsmPrinter <= external/llvm/lib/Target/X86/InstPrinter/X86ATTInstPrinter.cpp
host C++: libLLVMX86AsmPrinter <= external/llvm/lib/Target/X86/InstPrinter/X86IntelInstPrinter.cpp
host C++: libLLVMX86AsmPrinter <= external/llvm/lib/Target/X86/InstPrinter/X86InstComments.cpp
host StaticLib: libLLVMX86AsmPrinter (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86AsmPrinter_intermediates/libLLVMX86AsmPrinter.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Utils_intermediates/import_includes
host C++: libLLVMX86Utils <= external/llvm/lib/Target/X86/Utils/X86ShuffleDecode.cpp
host StaticLib: libLLVMX86Utils (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMX86Utils_intermediates/libLLVMX86Utils.a)
Host TableGen: libLLVMIRReader (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMIRReader_intermediates/import_includes
host C++: libLLVMIRReader <= external/llvm/lib/IRReader/IRReader.cpp
host StaticLib: libLLVMIRReader (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMIRReader_intermediates/libLLVMIRReader.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAsmParser_intermediates/import_includes
host C++: libLLVMAsmParser <= external/llvm/lib/AsmParser/LLLexer.cpp
host C++: libLLVMAsmParser <= external/llvm/lib/AsmParser/LLParser.cpp
host C++: libLLVMAsmParser <= external/llvm/lib/AsmParser/Parser.cpp
host StaticLib: libLLVMAsmParser (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAsmParser_intermediates/libLLVMAsmParser.a)
Host TableGen: libLLVMAsmPrinter (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAsmPrinter_intermediates/import_includes
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/AsmPrinter.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/AsmPrinterDwarf.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/AsmPrinterInlineAsm.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/ARMException.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/DIE.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/DwarfAccelTable.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/DwarfCFIException.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/DwarfCompileUnit.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/DwarfDebug.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/DwarfException.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/ErlangGCPrinter.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/OcamlGCPrinter.cpp
host C++: libLLVMAsmPrinter <= external/llvm/lib/CodeGen/AsmPrinter/Win64Exception.cpp
host StaticLib: libLLVMAsmPrinter (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAsmPrinter_intermediates/libLLVMAsmPrinter.a)
Host TableGen: libLLVMBitReader (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMBitReader_intermediates/import_includes
host C++: libLLVMBitReader <= external/llvm/lib/Bitcode/Reader/BitReader.cpp
host C++: libLLVMBitReader <= external/llvm/lib/Bitcode/Reader/BitcodeReader.cpp
host C++: libLLVMBitReader <= external/llvm/lib/Bitcode/Reader/BitstreamReader.cpp
host StaticLib: libLLVMBitReader (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMBitReader_intermediates/libLLVMBitReader.a)
Host TableGen: libLLVMBitWriter (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMBitWriter_intermediates/import_includes
host C++: libLLVMBitWriter <= external/llvm/lib/Bitcode/Writer/BitWriter.cpp
host C++: libLLVMBitWriter <= external/llvm/lib/Bitcode/Writer/BitcodeWriter.cpp
host C++: libLLVMBitWriter <= external/llvm/lib/Bitcode/Writer/BitcodeWriterPass.cpp
host C++: libLLVMBitWriter <= external/llvm/lib/Bitcode/Writer/ValueEnumerator.cpp
host StaticLib: libLLVMBitWriter (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMBitWriter_intermediates/libLLVMBitWriter.a)
Host TableGen: libLLVMSelectionDAG (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMSelectionDAG_intermediates/import_includes
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/DAGCombiner.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/FastISel.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/FunctionLoweringInfo.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/InstrEmitter.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/LegalizeDAG.cpp
external/llvm/lib/CodeGen/SelectionDAG/LegalizeDAG.cpp: In member function 'void (anonymous namespace)::SelectionDAGLegalize::ExpandNode(llvm::SDNode*)':
external/llvm/lib/CodeGen/SelectionDAG/LegalizeDAG.cpp:3636:53: warning: 'TrueValue' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/LegalizeFloatTypes.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/LegalizeIntegerTypes.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/LegalizeTypes.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/LegalizeTypesGeneric.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/LegalizeVectorOps.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/LegalizeVectorTypes.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/ResourcePriorityQueue.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/ScheduleDAGFast.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/ScheduleDAGRRList.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/ScheduleDAGSDNodes.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/ScheduleDAGVLIW.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/SelectionDAG.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/SelectionDAGBuilder.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/SelectionDAGDumper.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/SelectionDAGISel.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/SelectionDAGPrinter.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/TargetLowering.cpp
host C++: libLLVMSelectionDAG <= external/llvm/lib/CodeGen/SelectionDAG/TargetSelectionDAGInfo.cpp
host StaticLib: libLLVMSelectionDAG (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMSelectionDAG_intermediates/libLLVMSelectionDAG.a)
Host TableGen: libLLVMipo (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMipo_intermediates/import_includes
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/ArgumentPromotion.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/BarrierNoopPass.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/ConstantMerge.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/DeadArgumentElimination.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/ExtractGV.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/FunctionAttrs.cpp
external/llvm/lib/Transforms/IPO/FunctionAttrs.cpp: In member function 'virtual bool (anonymous namespace)::ArgumentUsesTracker::captured(llvm::Use*)':
external/llvm/lib/Transforms/IPO/FunctionAttrs.cpp:353:12: warning: variable 'Found' set but not used [-Wunused-but-set-variable]
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/GlobalDCE.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/GlobalOpt.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/IPConstantPropagation.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/IPO.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/InlineAlways.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/InlineSimple.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/Inliner.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/Internalize.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/LoopExtractor.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/MergeFunctions.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/PartialInlining.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/PassManagerBuilder.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/PruneEH.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/StripDeadPrototypes.cpp
host C++: libLLVMipo <= external/llvm/lib/Transforms/IPO/StripSymbols.cpp
host StaticLib: libLLVMipo (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMipo_intermediates/libLLVMipo.a)
Host TableGen: libLLVMipa (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMipa_intermediates/import_includes
host C++: libLLVMipa <= external/llvm/lib/Analysis/IPA/CallGraph.cpp
host C++: libLLVMipa <= external/llvm/lib/Analysis/IPA/CallGraphSCCPass.cpp
host C++: libLLVMipa <= external/llvm/lib/Analysis/IPA/CallPrinter.cpp
host C++: libLLVMipa <= external/llvm/lib/Analysis/IPA/FindUsedTypes.cpp
host C++: libLLVMipa <= external/llvm/lib/Analysis/IPA/GlobalsModRef.cpp
host C++: libLLVMipa <= external/llvm/lib/Analysis/IPA/IPA.cpp
host C++: libLLVMipa <= external/llvm/lib/Analysis/IPA/InlineCost.cpp
host StaticLib: libLLVMipa (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMipa_intermediates/libLLVMipa.a)
Host TableGen: libLLVMInstCombine (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMInstCombine_intermediates/import_includes
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineAddSub.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineAndOrXor.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineCalls.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineCasts.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineCompares.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineLoadStoreAlloca.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineMulDivRem.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombinePHI.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineSelect.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineShifts.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineSimplifyDemanded.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstCombineVectorOps.cpp
host C++: libLLVMInstCombine <= external/llvm/lib/Transforms/InstCombine/InstructionCombining.cpp
host StaticLib: libLLVMInstCombine (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMInstCombine_intermediates/libLLVMInstCombine.a)
Host TableGen: libLLVMInstrumentation (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMInstrumentation_intermediates/import_includes
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/AddressSanitizer.cpp
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/BoundsChecking.cpp
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/EdgeProfiling.cpp
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/GCOVProfiling.cpp
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/Instrumentation.cpp
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/MemorySanitizer.cpp
external/llvm/include/llvm/IR/IRBuilder.h: In member function 'virtual void (anonymous namespace)::VarArgAMD64Helper::visitCallSite(llvm::CallSite&, llvm::IRBuilder<>&)':
external/llvm/include/llvm/IR/IRBuilder.h:847:54: warning: 'Base' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/lib/Transforms/Instrumentation/MemorySanitizer.cpp:1878:14: note: 'Base' was declared here
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/OptimalEdgeProfiling.cpp
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/PathProfiling.cpp
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/ProfilingUtils.cpp
host C++: libLLVMInstrumentation <= external/llvm/lib/Transforms/Instrumentation/ThreadSanitizer.cpp
host StaticLib: libLLVMInstrumentation (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMInstrumentation_intermediates/libLLVMInstrumentation.a)
Host TableGen: libLLVMCodeGen (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMCodeGen_intermediates/import_includes
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/AggressiveAntiDepBreaker.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/AllocationOrder.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/Analysis.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/BasicTargetTransformInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/BranchFolding.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/CalcSpillWeights.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/CallingConvLower.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/CodeGen.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/CriticalAntiDepBreaker.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/DeadMachineInstructionElim.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/DFAPacketizer.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/DwarfEHPrepare.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/EarlyIfConversion.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/EdgeBundles.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ErlangGC.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ExecutionDepsFix.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ExpandISelPseudos.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ExpandPostRAPseudos.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/GCMetadata.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/GCMetadataPrinter.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/GCStrategy.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/IfConversion.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/InlineSpiller.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/InterferenceCache.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/IntrinsicLowering.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/JITCodeEmitter.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LatencyPriorityQueue.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LexicalScopes.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveDebugVariables.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveIntervalAnalysis.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveInterval.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveIntervalUnion.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveRangeCalc.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveRangeEdit.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveRegMatrix.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveStackAnalysis.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LiveVariables.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LLVMTargetMachine.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/LocalStackSlotAllocation.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineBasicBlock.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineBlockFrequencyInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineBlockPlacement.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineBranchProbabilityInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineCodeEmitter.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineCopyPropagation.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineCSE.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineDominators.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineFunctionAnalysis.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineFunction.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineFunctionPass.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineFunctionPrinterPass.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineInstrBundle.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineInstr.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineLICM.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineLoopInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineModuleInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineModuleInfoImpls.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachinePassRegistry.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachinePostDominators.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineRegisterInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineScheduler.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineSink.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineSSAUpdater.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineTraceMetrics.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/MachineVerifier.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/OcamlGC.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/OptimizePHIs.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/Passes.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/PeepholeOptimizer.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/PHIElimination.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/PHIEliminationUtils.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/PostRASchedulerList.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ProcessImplicitDefs.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/PrologEpilogInserter.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/PseudoSourceValue.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegAllocBase.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegAllocBasic.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegAllocFast.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegAllocGreedy.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegAllocPBQP.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegisterClassInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegisterCoalescer.cpp
external/llvm/lib/CodeGen/RegisterCoalescer.cpp: In member function 'bool (anonymous namespace)::RegisterCoalescer::_ZN12_GLOBAL__N_117RegisterCoalescer23reMaterializeTrivialDefERN4llvm13CoalescerPairEPNS1_12MachineInstrERb.constprop.392(llvm::CoalescerPair&, llvm::MachineInstr*, bool&)':
external/llvm/lib/CodeGen/RegisterCoalescer.cpp:832:12: warning: 'RCForInst' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegisterPressure.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/RegisterScavenging.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ScheduleDAG.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ScheduleDAGInstrs.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ScheduleDAGPrinter.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ScoreboardHazardRecognizer.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ShadowStackGC.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/ShrinkWrapping.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/SjLjEHPrepare.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/SlotIndexes.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/Spiller.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/SpillPlacement.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/SplitKit.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/StackColoring.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/StackProtector.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/StackSlotColoring.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/StrongPHIElimination.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TailDuplication.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TargetFrameLoweringImpl.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TargetInstrInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TargetLoweringBase.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TargetLoweringObjectFileImpl.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TargetOptionsImpl.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TargetRegisterInfo.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TargetSchedule.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/TwoAddressInstructionPass.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/UnreachableBlockElim.cpp
host C++: libLLVMCodeGen <= external/llvm/lib/CodeGen/VirtRegMap.cpp
host StaticLib: libLLVMCodeGen (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMCodeGen_intermediates/libLLVMCodeGen.a)
Host TableGen: libLLVMObject (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMObject_intermediates/import_includes
host C++: libLLVMObject <= external/llvm/lib/Object/Archive.cpp
host C++: libLLVMObject <= external/llvm/lib/Object/Binary.cpp
host C++: libLLVMObject <= external/llvm/lib/Object/COFFObjectFile.cpp
external/llvm/include/llvm/Support/Endian.h: In constructor 'llvm::object::COFFObjectFile::COFFObjectFile(llvm::MemoryBuffer*, llvm::error_code&)':
external/llvm/include/llvm/Support/Endian.h:51:3: warning: 'StringTableSizePtr' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/lib/Object/COFFObjectFile.cpp:504:24: note: 'StringTableSizePtr' was declared here
host C++: libLLVMObject <= external/llvm/lib/Object/ELFObjectFile.cpp
host C++: libLLVMObject <= external/llvm/lib/Object/Error.cpp
host C++: libLLVMObject <= external/llvm/lib/Object/MachOObjectFile.cpp
host C++: libLLVMObject <= external/llvm/lib/Object/MachOUniversal.cpp
host C++: libLLVMObject <= external/llvm/lib/Object/Object.cpp
host C++: libLLVMObject <= external/llvm/lib/Object/ObjectFile.cpp
host StaticLib: libLLVMObject (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMObject_intermediates/libLLVMObject.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMLinker_intermediates/import_includes
host C++: libLLVMLinker <= external/llvm/lib/Linker/LinkModules.cpp
host StaticLib: libLLVMLinker (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMLinker_intermediates/libLLVMLinker.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMC_intermediates/import_includes
host C++: libLLVMMC <= external/llvm/lib/MC/ELFObjectWriter.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MachObjectWriter.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCAsmBackend.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCAsmInfo.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCAsmInfoCOFF.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCAsmInfoDarwin.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCAsmStreamer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCAssembler.cpp
external/llvm/lib/MC/MCAssembler.cpp: In member function 'uint64_t llvm::MCAssembler::computeFragmentSize(const llvm::MCAsmLayout&, const llvm::MCFragment&) const':
external/llvm/lib/MC/MCAssembler.cpp:433:10: warning: enumeration value 'FT_Region' not handled in switch [-Wswitch]
external/llvm/lib/MC/MCAssembler.cpp:433:10: warning: enumeration value 'FT_Reloc' not handled in switch [-Wswitch]
external/llvm/lib/MC/MCAssembler.cpp:433:10: warning: enumeration value 'FT_Target' not handled in switch [-Wswitch]
external/llvm/lib/MC/MCAssembler.cpp: In function 'void writeFragment(const llvm::MCAssembler&, const llvm::MCAsmLayout&, const llvm::MCFragment&)':
external/llvm/lib/MC/MCAssembler.cpp:585:10: warning: enumeration value 'FT_Region' not handled in switch [-Wswitch]
external/llvm/lib/MC/MCAssembler.cpp:585:10: warning: enumeration value 'FT_Reloc' not handled in switch [-Wswitch]
external/llvm/lib/MC/MCAssembler.cpp:585:10: warning: enumeration value 'FT_Target' not handled in switch [-Wswitch]
host C++: libLLVMMC <= external/llvm/lib/MC/MCCodeEmitter.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCCodeGenInfo.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCContext.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCDisassembler.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCDwarf.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCELF.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCELFObjectTargetWriter.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCELFStreamer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCExpr.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCExternalSymbolizer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCInst.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCInstPrinter.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCInstrAnalysis.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCLabel.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCMachObjectTargetWriter.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCMachOStreamer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCNullStreamer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCObjectFileInfo.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCObjectStreamer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCObjectWriter.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCRegisterInfo.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCRelocationInfo.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCSection.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCSectionCOFF.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCSectionELF.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCSectionMachO.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCStreamer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCSubtargetInfo.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCSymbol.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCSymbolizer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCValue.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/MCWin64EH.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/WinCOFFObjectWriter.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/WinCOFFStreamer.cpp
host C++: libLLVMMC <= external/llvm/lib/MC/SubtargetFeature.cpp
host StaticLib: libLLVMMC (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMC_intermediates/libLLVMMC.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMCParser_intermediates/import_includes
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/AsmLexer.cpp
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/AsmParser.cpp
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/COFFAsmParser.cpp
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/DarwinAsmParser.cpp
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/ELFAsmParser.cpp
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/MCAsmLexer.cpp
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/MCAsmParser.cpp
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/MCAsmParserExtension.cpp
host C++: libLLVMMCParser <= external/llvm/lib/MC/MCParser/MCTargetAsmParser.cpp
host StaticLib: libLLVMMCParser (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMMCParser_intermediates/libLLVMMCParser.a)
Host TableGen: libLLVMScalarOpts (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMScalarOpts_intermediates/import_includes
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/ADCE.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/BasicBlockPlacement.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/CodeGenPrepare.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/ConstantProp.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/CorrelatedValuePropagation.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/DCE.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/DeadStoreElimination.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/EarlyCSE.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/GlobalMerge.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/GVN.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/IndVarSimplify.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/JumpThreading.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LICM.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LoopDeletion.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LoopIdiomRecognize.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LoopInstSimplify.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LoopRotation.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LoopStrengthReduce.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LoopUnrollPass.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LoopUnswitch.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/LowerAtomic.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/MemCpyOptimizer.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/Reassociate.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/Reg2Mem.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/SCCP.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/SROA.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/Scalar.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/ScalarReplAggregates.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/SimplifyCFGPass.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/Sink.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/StructurizeCFG.cpp
host C++: libLLVMScalarOpts <= external/llvm/lib/Transforms/Scalar/TailRecursionElimination.cpp
host StaticLib: libLLVMScalarOpts (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMScalarOpts_intermediates/libLLVMScalarOpts.a)
Host TableGen: libLLVMTransformObjCARC (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTransformObjCARC_intermediates/import_includes
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/DependencyAnalysis.cpp
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/ObjCARCAliasAnalysis.cpp
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/ObjCARCAPElim.cpp
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/ObjCARCContract.cpp
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/ObjCARC.cpp
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/ObjCARCExpand.cpp
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/ObjCARCOpts.cpp
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/ObjCARCUtil.cpp
host C++: libLLVMTransformObjCARC <= external/llvm/lib/Transforms/ObjCARC/ProvenanceAnalysis.cpp
host StaticLib: libLLVMTransformObjCARC (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTransformObjCARC_intermediates/libLLVMTransformObjCARC.a)
Host TableGen: libLLVMTransformUtils (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTransformUtils_intermediates/import_includes
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/BasicBlockUtils.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/BreakCriticalEdges.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/BuildLibCalls.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/BypassSlowDivision.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/CloneFunction.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/CloneModule.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/CmpInstAnalysis.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/CodeExtractor.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/DemoteRegToStack.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/InlineFunction.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/InstructionNamer.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/LCSSA.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/Local.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/LoopSimplify.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/LoopUnroll.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/LoopUnrollRuntime.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/LowerExpectIntrinsic.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/LowerInvoke.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/LowerSwitch.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/Mem2Reg.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/MetaRenamer.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/ModuleUtils.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/PromoteMemoryToRegister.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/SSAUpdater.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/SimplifyCFG.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/SimplifyIndVar.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/SimplifyInstructions.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/SimplifyLibCalls.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/SpecialCaseList.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/UnifyFunctionExitNodes.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/Utils.cpp
host C++: libLLVMTransformUtils <= external/llvm/lib/Transforms/Utils/ValueMapper.cpp
host StaticLib: libLLVMTransformUtils (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTransformUtils_intermediates/libLLVMTransformUtils.a)
Host TableGen: libLLVMVectorize (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMVectorize_intermediates/import_includes
host C++: libLLVMVectorize <= external/llvm/lib/Transforms/Vectorize/BBVectorize.cpp
host C++: libLLVMVectorize <= external/llvm/lib/Transforms/Vectorize/LoopVectorize.cpp
host C++: libLLVMVectorize <= external/llvm/lib/Transforms/Vectorize/SLPVectorizer.cpp
host C++: libLLVMVectorize <= external/llvm/lib/Transforms/Vectorize/Vectorize.cpp
host StaticLib: libLLVMVectorize (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMVectorize_intermediates/libLLVMVectorize.a)
Host TableGen: libLLVMAnalysis (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAnalysis_intermediates/import_includes
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/AliasAnalysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/AliasAnalysisCounter.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/AliasAnalysisEvaluator.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/AliasDebugger.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/AliasSetTracker.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/Analysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/BasicAliasAnalysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/BlockFrequencyInfo.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/BranchProbabilityInfo.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/CFG.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/CFGPrinter.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/CaptureTracking.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/CodeMetrics.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ConstantFolding.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/CostModel.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/DependenceAnalysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/DomPrinter.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/DominanceFrontier.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/IVUsers.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/InstCount.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/InstructionSimplify.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/Interval.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/IntervalPartition.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/LazyValueInfo.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/LibCallAliasAnalysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/LibCallSemantics.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/Lint.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/Loads.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/LoopInfo.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/LoopPass.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/MemDepPrinter.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/MemoryBuiltins.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/MemoryDependenceAnalysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ModuleDebugInfoPrinter.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/NoAliasAnalysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/PHITransAddr.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/PathNumbering.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/PathProfileInfo.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/PathProfileVerifier.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/PostDominators.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ProfileDataLoader.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ProfileDataLoaderPass.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ProfileEstimatorPass.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ProfileInfo.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ProfileInfoLoader.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ProfileInfoLoaderPass.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ProfileVerifierPass.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/PtrUseVisitor.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/RegionInfo.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/RegionPass.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/RegionPrinter.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ScalarEvolution.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ScalarEvolutionAliasAnalysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ScalarEvolutionExpander.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ScalarEvolutionNormalization.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/SparsePropagation.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/TargetTransformInfo.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/Trace.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/TypeBasedAliasAnalysis.cpp
host C++: libLLVMAnalysis <= external/llvm/lib/Analysis/ValueTracking.cpp
host StaticLib: libLLVMAnalysis (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMAnalysis_intermediates/libLLVMAnalysis.a)
Host TableGen: libLLVMCore (gen-intrinsic) <= external/llvm/include/llvm/IR/Intrinsics.td
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMCore_intermediates/import_includes
host C++: libLLVMCore <= external/llvm/lib/IR/AsmWriter.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Attributes.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/AutoUpgrade.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/BasicBlock.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/ConstantFold.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Constants.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Core.cpp
external/llvm/include/llvm/IR/IRBuilder.h: In function 'LLVMOpaqueValue* LLVMBuildAtomicRMW(LLVMBuilderRef, LLVMAtomicRMWBinOp, LLVMValueRef, LLVMValueRef, LLVMAtomicOrdering, LLVMBool)':
external/llvm/include/llvm/IR/IRBuilder.h:887:72: warning: 'intordering' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/lib/IR/Core.cpp:2417:18: note: 'intordering' was declared here
external/llvm/include/llvm/IR/IRBuilder.h:887:72: warning: 'intop' may be used uninitialized in this function [-Wmaybe-uninitialized]
external/llvm/lib/IR/Core.cpp:2403:24: note: 'intop' was declared here
host C++: libLLVMCore <= external/llvm/lib/IR/DataLayout.cpp
external/llvm/lib/IR/DataLayout.cpp: In function 'unsigned int getInt(llvm::StringRef)':
external/llvm/lib/IR/DataLayout.cpp:193:10: warning: 'Result' may be used uninitialized in this function [-Wmaybe-uninitialized]
host C++: libLLVMCore <= external/llvm/lib/IR/DebugInfo.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/DebugLoc.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/DIBuilder.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Dominators.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Function.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/GVMaterializer.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Globals.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/IRBuilder.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/InlineAsm.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Instruction.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Instructions.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/IntrinsicInst.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/LLVMContext.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/LLVMContextImpl.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/LeakDetector.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Metadata.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Module.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Pass.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/PassManager.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/PassRegistry.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/PrintModulePass.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Type.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/TypeFinder.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Use.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/User.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Value.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/ValueSymbolTable.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/ValueTypes.cpp
host C++: libLLVMCore <= external/llvm/lib/IR/Verifier.cpp
host StaticLib: libLLVMCore (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMCore_intermediates/libLLVMCore.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMOption_intermediates/import_includes
host C++: libLLVMOption <= external/llvm/lib/Option/Arg.cpp
host C++: libLLVMOption <= external/llvm/lib/Option/ArgList.cpp
host C++: libLLVMOption <= external/llvm/lib/Option/Option.cpp
host C++: libLLVMOption <= external/llvm/lib/Option/OptTable.cpp
host StaticLib: libLLVMOption (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMOption_intermediates/libLLVMOption.a)
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTarget_intermediates/import_includes
host C++: libLLVMTarget <= external/llvm/lib/Target/Mangler.cpp
host C++: libLLVMTarget <= external/llvm/lib/Target/Target.cpp
host C++: libLLVMTarget <= external/llvm/lib/Target/TargetIntrinsicInfo.cpp
host C++: libLLVMTarget <= external/llvm/lib/Target/TargetJITInfo.cpp
host C++: libLLVMTarget <= external/llvm/lib/Target/TargetLibraryInfo.cpp
host C++: libLLVMTarget <= external/llvm/lib/Target/TargetLoweringObjectFile.cpp
host C++: libLLVMTarget <= external/llvm/lib/Target/TargetMachineC.cpp
host C++: libLLVMTarget <= external/llvm/lib/Target/TargetMachine.cpp
host C++: libLLVMTarget <= external/llvm/lib/Target/TargetSubtargetInfo.cpp
host StaticLib: libLLVMTarget (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libLLVMTarget_intermediates/libLLVMTarget.a)
Export includes file: external/clang/tools/driver/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/clang_intermediates/export_includes
host Executable: clang (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/clang_intermediates/clang)
Host Clang TableGen: arm_neon.h (gen-arm-neon) <= external/clang/include/clang/Basic/arm_neon.td
Notice file: external/clang/lib/Analysis/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libclangAnalysis.a.txt
Notice file: external/llvm/lib/Analysis/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libLLVMAnalysis.a.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/clang
Symlink /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/clang++ -> /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/clang
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libcompiler_rt-extras_intermediates/import_includes
target thumb C: libcompiler_rt-extras <= external/compiler-rt/lib/mulodi4.c
target StaticLib: libcompiler_rt-extras (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libcompiler_rt-extras_intermediates/libcompiler_rt-extras.a)
target SharedLib: libdl (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libdl_intermediates/LINKED/libdl.so)
target Symbolic: libdl (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/system/lib/libdl.so)
target Strip: libdl (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libdl.so)
Export includes file: bionic/libc/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbionic_ssp_intermediates/export_includes
Export includes file: bionic/libc/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_bionic_intermediates/export_includes
Export includes file: bionic/libc/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_freebsd_intermediates/export_includes
Export includes file: bionic/libc/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_netbsd_intermediates/export_includes
Export includes file: bionic/libc/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_tzcode_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_common_intermediates/import_includes
target asm: libc_common <= bionic/libc/arch-arm/syscalls/_exit.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/_exit_thread.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__fork.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__waitid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/wait4.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__sys_clone.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/execve.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__setuid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getuid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getgid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/geteuid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getegid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getresuid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getresgid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/gettid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/readahead.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getgroups.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getpgid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getppid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getsid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setsid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setgid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__setreuid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__setresuid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setresgid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__brk.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__ptrace.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__getpriority.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setpriority.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setrlimit.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getrlimit.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getrusage.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setgroups.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setpgid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/vfork.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setregid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/chroot.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/prctl.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/capget.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/capset.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sigaltstack.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/acct.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/read.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/write.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/pread64.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/pwrite64.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__open.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__openat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/close.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/lseek.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__llseek.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getpid.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__mmap2.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/munmap.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mremap.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/msync.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mprotect.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/madvise.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mlock.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/munlock.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mlockall.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/munlockall.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mincore.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__ioctl.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/readv.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/writev.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__fcntl.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/flock.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fchmod.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/dup.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/pipe.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/pipe2.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/dup2.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/select.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/ftruncate.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/ftruncate64.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getdents.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fsync.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fdatasync.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fchown.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sync.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__fcntl64.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__fstatfs64.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sendfile.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fstatat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mkdirat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fchownat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fchmodat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/renameat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fsetxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fgetxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/flistxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fremovexattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/link.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/unlink.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/unlinkat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/chdir.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mknod.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/chmod.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/chown.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/lchown.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mount.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/umount2.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fstat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/stat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/lstat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/mkdir.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/readlink.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/rmdir.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/rename.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__getcwd.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/access.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/faccessat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/symlink.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/fchdir.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/truncate.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/lsetxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/lgetxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/listxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/llistxattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/removexattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/lremovexattr.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__statfs64.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/unshare.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/swapon.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/swapoff.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/pause.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/gettimeofday.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/settimeofday.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/times.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/nanosleep.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/clock_gettime.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/clock_settime.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/clock_getres.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/clock_nanosleep.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getitimer.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setitimer.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__timer_create.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__timer_settime.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__timer_gettime.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__timer_getoverrun.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__timer_delete.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/utimes.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/utimensat.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/timerfd_create.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/timerfd_settime.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/timerfd_gettime.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sigaction.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sigprocmask.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__sigsuspend.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__rt_sigaction.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__rt_sigprocmask.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__rt_sigtimedwait.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sigpending.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/signalfd4.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/socket.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/socketpair.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/bind.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/connect.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/listen.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/accept.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getsockname.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getpeername.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sendto.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/recvfrom.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/shutdown.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/setsockopt.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/getsockopt.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sendmsg.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/recvmsg.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_setscheduler.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_getscheduler.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_yield.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_setparam.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_getparam.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_get_priority_max.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_get_priority_min.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_rr_get_interval.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sched_setaffinity.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__sched_getaffinity.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__getcpu.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/ioprio_set.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/ioprio_get.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/uname.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/umask.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__reboot.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__syslog.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/init_module.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/delete_module.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/klogctl.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/sysinfo.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/personality.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/perf_event_open.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/futex.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/epoll_create.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/epoll_ctl.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/epoll_wait.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/inotify_init.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/inotify_add_watch.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/inotify_rm_watch.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/poll.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/eventfd.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/__set_tls.S
target asm: libc_common <= bionic/libc/arch-arm/syscalls/cacheflush.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/abort_arm.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/clone.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/_exit_with_stack_teardown.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/ffs.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/futex_arm.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/__get_sp.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/kill.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/memcmp16.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/memcmp.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/_setjmp.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/setjmp.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/sigsetjmp.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/syscall.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/tgkill.S
target asm: libc_common <= bionic/libc/arch-arm/bionic/tkill.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/memcpy.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/memset.S
target asm: libc_common <= bionic/libc/arch-arm/krait/bionic/memmove.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/strcat.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/strcmp.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/strcpy.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/strlen.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/__strcat_chk.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/__strcpy_chk.S
target asm: libc_common <= bionic/libc/arch-arm/cortex-a15/bionic/memchr.S
target thumb C++: libc_common <= bionic/libc/bionic/__fgets_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__memmove_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__strchr_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__strlcat_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__strlcpy_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__strlen_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__strncat_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__strncpy_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__strrchr_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__umask_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__vsnprintf_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/__vsprintf_chk.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc_common <= bionic/libc/bionic/strchr.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target arm C: libc_common <= bionic/libc/bionic/pthread-atfork.c
target arm C: libc_common <= bionic/libc/bionic/pthread-rwlocks.c
target arm C: libc_common <= bionic/libc/bionic/pthread-timers.c
target arm C: libc_common <= bionic/libc/bionic/ptrace.c
bionic/libc/bionic/ptrace.c: In function '_thread_created_hook':
bionic/libc/bionic/ptrace.c:66:44: warning: unused parameter 'thread_id' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/unistd/alarm.c
target thumb C: libc_common <= bionic/libc/unistd/exec.c
target thumb C: libc_common <= bionic/libc/unistd/fnmatch.c
target thumb C: libc_common <= bionic/libc/unistd/syslog.c
target thumb C: libc_common <= bionic/libc/unistd/system.c
target thumb C: libc_common <= bionic/libc/unistd/time.c
target thumb C: libc_common <= bionic/libc/stdio/asprintf.c
target thumb C: libc_common <= bionic/libc/stdio/fflush.c
target thumb C: libc_common <= bionic/libc/stdio/fgetc.c
target thumb C: libc_common <= bionic/libc/stdio/findfp.c
target thumb C: libc_common <= bionic/libc/stdio/fprintf.c
target thumb C: libc_common <= bionic/libc/stdio/fputc.c
target thumb C: libc_common <= bionic/libc/stdio/fread.c
target thumb C: libc_common <= bionic/libc/stdio/freopen.c
target thumb C: libc_common <= bionic/libc/stdio/fscanf.c
target thumb C: libc_common <= bionic/libc/stdio/fseek.c
target thumb C: libc_common <= bionic/libc/stdio/ftell.c
target thumb C: libc_common <= bionic/libc/stdio/fvwrite.c
target thumb C: libc_common <= bionic/libc/stdio/gets.c
target thumb C: libc_common <= bionic/libc/stdio/printf.c
target thumb C: libc_common <= bionic/libc/stdio/refill.c
target thumb C: libc_common <= bionic/libc/stdio/rewind.c
target thumb C: libc_common <= bionic/libc/stdio/scanf.c
target thumb C: libc_common <= bionic/libc/stdio/snprintf.c
target thumb C: libc_common <= bionic/libc/stdio/sprintf.c
target thumb C: libc_common <= bionic/libc/stdio/sscanf.c
bionic/libc/stdio/sscanf.c: In function 'eofread':
bionic/libc/stdio/sscanf.c:41:15: warning: unused parameter 'cookie' [-Wunused-parameter]
bionic/libc/stdio/sscanf.c:41:29: warning: unused parameter 'buf' [-Wunused-parameter]
bionic/libc/stdio/sscanf.c:41:38: warning: unused parameter 'len' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/stdio/stdio.c
target thumb C: libc_common <= bionic/libc/stdio/ungetc.c
target thumb C: libc_common <= bionic/libc/stdio/vasprintf.c
target thumb C: libc_common <= bionic/libc/stdio/vfprintf.c
bionic/libc/stdio/vfprintf.c: In function '__vfprintf':
bionic/libc/stdio/vfprintf.c:782:6: warning: 'ndig' may be used uninitialized in this function [-Wmaybe-uninitialized]
target thumb C: libc_common <= bionic/libc/stdio/vfscanf.c
target thumb C: libc_common <= bionic/libc/stdio/vprintf.c
target thumb C: libc_common <= bionic/libc/stdio/vsnprintf.c
target thumb C: libc_common <= bionic/libc/stdio/vsprintf.c
target thumb C: libc_common <= bionic/libc/stdio/vscanf.c
target thumb C: libc_common <= bionic/libc/stdio/vsscanf.c
bionic/libc/stdio/vsscanf.c: In function 'eofread':
bionic/libc/stdio/vsscanf.c:40:15: warning: unused parameter 'cookie' [-Wunused-parameter]
bionic/libc/stdio/vsscanf.c:40:29: warning: unused parameter 'buf' [-Wunused-parameter]
bionic/libc/stdio/vsscanf.c:40:38: warning: unused parameter 'len' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/stdio/wbuf.c
target thumb C: libc_common <= bionic/libc/stdlib/atexit.c
target thumb C: libc_common <= bionic/libc/stdlib/ctype_.c
target thumb C: libc_common <= bionic/libc/stdlib/getenv.c
target thumb C: libc_common <= bionic/libc/stdlib/putenv.c
target thumb C: libc_common <= bionic/libc/stdlib/setenv.c
target thumb C: libc_common <= bionic/libc/stdlib/strtod.c
target thumb C: libc_common <= bionic/libc/stdlib/strtoimax.c
target thumb C: libc_common <= bionic/libc/stdlib/strtol.c
target thumb C: libc_common <= bionic/libc/stdlib/strtoll.c
target thumb C: libc_common <= bionic/libc/stdlib/strtoul.c
target thumb C: libc_common <= bionic/libc/stdlib/strtoull.c
target thumb C: libc_common <= bionic/libc/stdlib/strtoumax.c
target thumb C: libc_common <= bionic/libc/stdlib/tolower_.c
target thumb C: libc_common <= bionic/libc/stdlib/toupper_.c
target thumb C: libc_common <= bionic/libc/string/strcasecmp.c
target thumb C: libc_common <= bionic/libc/string/strcspn.c
target thumb C: libc_common <= bionic/libc/string/strdup.c
target thumb C: libc_common <= bionic/libc/string/strpbrk.c
target thumb C: libc_common <= bionic/libc/string/strsep.c
target thumb C: libc_common <= bionic/libc/string/strspn.c
target thumb C: libc_common <= bionic/libc/string/strstr.c
target thumb C: libc_common <= bionic/libc/string/strtok.c
target thumb C: libc_common <= bionic/libc/wchar/wcswidth.c
target thumb C: libc_common <= bionic/libc/wchar/wcsxfrm.c
bionic/libc/wchar/wcsxfrm.c: In function 'wcsxfrm':
bionic/libc/wchar/wcsxfrm.c:39:23: warning: unused variable 'ss' [-Wunused-variable]
bionic/libc/wchar/wcsxfrm.c:39:19: warning: unused variable 's' [-Wunused-variable]
bionic/libc/wchar/wcsxfrm.c:39:11: warning: unused variable 'mbsrc' [-Wunused-variable]
bionic/libc/wchar/wcsxfrm.c:37:20: warning: unused variable 'l' [-Wunused-variable]
bionic/libc/wchar/wcsxfrm.c:37:15: warning: unused variable 'sec' [-Wunused-variable]
bionic/libc/wchar/wcsxfrm.c:37:9: warning: unused variable 'prim' [-Wunused-variable]
target thumb C: libc_common <= bionic/libc/bionic/arc4random.c
bionic/libc/bionic/arc4random.c: In function 'arc4_stir':
bionic/libc/bionic/arc4random.c:109:6: warning: unused variable 'n' [-Wunused-variable]
target thumb C: libc_common <= bionic/libc/bionic/atoi.c
target thumb C: libc_common <= bionic/libc/bionic/atol.c
target thumb C: libc_common <= bionic/libc/bionic/atoll.c
target thumb C: libc_common <= bionic/libc/bionic/bindresvport.c
target thumb C: libc_common <= bionic/libc/bionic/bionic_clone.c
target thumb C: libc_common <= bionic/libc/bionic/clearenv.c
target thumb C: libc_common <= bionic/libc/bionic/cpuacct.c
target thumb C: libc_common <= bionic/libc/bionic/daemon.c
target thumb C: libc_common <= bionic/libc/bionic/err.c
target thumb C: libc_common <= bionic/libc/bionic/ether_aton.c
target thumb C: libc_common <= bionic/libc/bionic/ether_ntoa.c
target thumb C: libc_common <= bionic/libc/bionic/fcntl.c
target thumb C: libc_common <= bionic/libc/bionic/fdprintf.c
target thumb C: libc_common <= bionic/libc/bionic/flockfile.c
target thumb C: libc_common <= bionic/libc/bionic/fork.c
target thumb C: libc_common <= bionic/libc/bionic/fstatfs.c
target thumb C: libc_common <= bionic/libc/bionic/ftime.c
target thumb C: libc_common <= bionic/libc/bionic/ftok.c
target thumb C: libc_common <= bionic/libc/bionic/fts.c
bionic/libc/bionic/fts.c: In function 'fts_set':
bionic/libc/bionic/fts.c:449:14: warning: unused parameter 'sp' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/bionic/getdtablesize.c
target thumb C: libc_common <= bionic/libc/bionic/gethostname.c
target thumb C: libc_common <= bionic/libc/bionic/getpgrp.c
target thumb C: libc_common <= bionic/libc/bionic/getpriority.c
target thumb C: libc_common <= bionic/libc/bionic/getpt.c
target thumb C: libc_common <= bionic/libc/bionic/if_indextoname.c
bionic/libc/bionic/if_indextoname.c: In function 'if_indextoname':
bionic/libc/bionic/if_indextoname.c:44:9: warning: unused variable 'index' [-Wunused-variable]
target thumb C: libc_common <= bionic/libc/bionic/if_nametoindex.c
target thumb C: libc_common <= bionic/libc/bionic/initgroups.c
target thumb C: libc_common <= bionic/libc/bionic/ioctl.c
target thumb C: libc_common <= bionic/libc/bionic/isatty.c
target thumb C: libc_common <= bionic/libc/bionic/issetugid.c
target thumb C: libc_common <= bionic/libc/bionic/ldexp.c
target thumb C: libc_common <= bionic/libc/bionic/lseek64.c
target thumb C: libc_common <= bionic/libc/bionic/md5.c
bionic/libc/bionic/md5.c: In function 'MD5_Update':
bionic/libc/bionic/md5.c:234:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
target thumb C: libc_common <= bionic/libc/bionic/memmem.c
target thumb C: libc_common <= bionic/libc/bionic/memswap.c
target thumb C: libc_common <= bionic/libc/bionic/name_mem.c
bionic/libc/bionic/name_mem.c: In function '__bionic_name_mem':
bionic/libc/bionic/name_mem.c:51:5: warning: implicit declaration of function 'prctl' [-Wimplicit-function-declaration]
target thumb C: libc_common <= bionic/libc/bionic/openat.c
target thumb C: libc_common <= bionic/libc/bionic/open.c
target thumb C: libc_common <= bionic/libc/bionic/pathconf.c
target thumb C: libc_common <= bionic/libc/bionic/perror.c
target thumb C: libc_common <= bionic/libc/bionic/pread.c
target thumb C: libc_common <= bionic/libc/bionic/pselect.c
target thumb C: libc_common <= bionic/libc/bionic/ptsname.c
target thumb C: libc_common <= bionic/libc/bionic/ptsname_r.c
target thumb C: libc_common <= bionic/libc/bionic/pututline.c
target thumb C: libc_common <= bionic/libc/bionic/pwrite.c
target thumb C: libc_common <= bionic/libc/bionic/reboot.c
target thumb C: libc_common <= bionic/libc/bionic/recv.c
target thumb C: libc_common <= bionic/libc/bionic/sched_cpualloc.c
target thumb C: libc_common <= bionic/libc/bionic/sched_cpucount.c
target thumb C: libc_common <= bionic/libc/bionic/sched_getcpu.c
target thumb C: libc_common <= bionic/libc/bionic/semaphore.c
bionic/libc/bionic/semaphore.c: In function 'sem_unlink':
bionic/libc/bionic/semaphore.c:150:29: warning: unused parameter 'name' [-Wunused-parameter]
bionic/libc/bionic/semaphore.c: In function 'sem_timedwait':
bionic/libc/bionic/semaphore.c:269:10: warning: unused variable 'ret' [-Wunused-variable]
target thumb C: libc_common <= bionic/libc/bionic/send.c
target thumb C: libc_common <= bionic/libc/bionic/setegid.c
target thumb C: libc_common <= bionic/libc/bionic/seteuid.c
target thumb C: libc_common <= bionic/libc/bionic/setpgrp.c
target thumb C: libc_common <= bionic/libc/bionic/setresuid.c
target thumb C: libc_common <= bionic/libc/bionic/setreuid.c
target thumb C: libc_common <= bionic/libc/bionic/setuid.c
target thumb C: libc_common <= bionic/libc/bionic/sigblock.c
target thumb C: libc_common <= bionic/libc/bionic/siginterrupt.c
target thumb C: libc_common <= bionic/libc/bionic/siglist.c
target thumb C: libc_common <= bionic/libc/bionic/signal.c
target thumb C: libc_common <= bionic/libc/bionic/signame.c
target thumb C: libc_common <= bionic/libc/bionic/sigsetmask.c
target thumb C: libc_common <= bionic/libc/bionic/sigsuspend.c
target thumb C: libc_common <= bionic/libc/bionic/sleep.c
target thumb C: libc_common <= bionic/libc/bionic/statfs.c
target thumb C: libc_common <= bionic/libc/bionic/strndup.c
target thumb C: libc_common <= bionic/libc/bionic/strntoimax.c
target thumb C: libc_common <= bionic/libc/bionic/strntoumax.c
target thumb C: libc_common <= bionic/libc/bionic/strtotimeval.c
bionic/libc/bionic/strtotimeval.c: In function 'strtotimeval':
bionic/libc/bionic/strtotimeval.c:35:9: warning: unused variable 'n' [-Wunused-variable]
target thumb C: libc_common <= bionic/libc/bionic/system_properties.c
bionic/libc/bionic/system_properties.c: In function 'send_prop_msg':
bionic/libc/bionic/system_properties.c:501:8: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/system_properties.c:501:8: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
target thumb C: libc_common <= bionic/libc/bionic/system_properties_compat.c
target thumb C: libc_common <= bionic/libc/bionic/tcgetpgrp.c
target thumb C: libc_common <= bionic/libc/bionic/tcsetpgrp.c
target thumb C: libc_common <= bionic/libc/bionic/thread_atexit.c
target thumb C: libc_common <= bionic/libc/bionic/time64.c
bionic/libc/bionic/time64.c: In function 'check_tm':
bionic/libc/bionic/time64.c:251:32: warning: unused parameter 'tm' [-Wunused-parameter]
bionic/libc/bionic/time64.c: At top level:
bionic/libc/bionic/time64.c:251:12: warning: 'check_tm' defined but not used [-Wunused-function]
target thumb C: libc_common <= bionic/libc/bionic/umount.c
target thumb C: libc_common <= bionic/libc/bionic/unlockpt.c
target thumb C: libc_common <= bionic/libc/bionic/usleep.c
target thumb C: libc_common <= bionic/libc/bionic/utmp.c
target thumb C: libc_common <= bionic/libc/bionic/wcscoll.c
target thumb C: libc_common <= bionic/libc/netbsd/gethnamaddr.c
bionic/libc/netbsd/gethnamaddr.c: In function 'getanswer':
bionic/libc/netbsd/gethnamaddr.c:400:5: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:400:5: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:400:5: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c: In function 'gethostbyname_r':
bionic/libc/netbsd/gethnamaddr.c:471:61: warning: unused parameter 'buf' [-Wunused-parameter]
bionic/libc/netbsd/gethnamaddr.c:471:73: warning: unused parameter 'buflen' [-Wunused-parameter]
bionic/libc/netbsd/gethnamaddr.c: In function 'android_open_proxy':
bionic/libc/netbsd/gethnamaddr.c:546:6: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:546:6: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c: In function 'android_gethostbyaddrforiface_proxy':
bionic/libc/netbsd/gethnamaddr.c:784:51: warning: unused parameter 'mark' [-Wunused-parameter]
bionic/libc/netbsd/gethnamaddr.c: In function 'android_gethostbyaddrforiface_real':
bionic/libc/netbsd/gethnamaddr.c:834:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:834:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:834:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:835:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:835:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:835:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:835:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:835:7: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/gethnamaddr.c:837:8: warning: pointer of type 'void *' used in arithmetic [-Wpointer-arith]
bionic/libc/netbsd/gethnamaddr.c: In function '_gethtbyname':
bionic/libc/netbsd/gethnamaddr.c:989:30: warning: unused parameter 'cb_data' [-Wunused-parameter]
bionic/libc/netbsd/gethnamaddr.c: In function '_gethtbyaddr':
bionic/libc/netbsd/gethnamaddr.c:1116:30: warning: unused parameter 'cb_data' [-Wunused-parameter]
bionic/libc/netbsd/gethnamaddr.c: In function '_dns_gethtbyname':
bionic/libc/netbsd/gethnamaddr.c:1249:34: warning: unused parameter 'cb_data' [-Wunused-parameter]
bionic/libc/netbsd/gethnamaddr.c: In function '_dns_gethtbyaddr':
bionic/libc/netbsd/gethnamaddr.c:1309:34: warning: unused parameter 'cb_data' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/netbsd/inet/nsap_addr.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/__dn_comp.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/__res_close.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/__res_send.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/herror.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_comp.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_data.c
bionic/libc/netbsd/resolv/res_data.c: In function '__hostalias':
bionic/libc/netbsd/resolv/res_data.c:306:23: warning: unused parameter 'name' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_debug.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_init.c
bionic/libc/netbsd/resolv/res_init.c: In function '__res_vinit':
bionic/libc/netbsd/resolv/res_init.c:178:8: warning: unused variable 'net' [-Wunused-variable]
bionic/libc/netbsd/resolv/res_init.c:177:6: warning: unused variable 'nsort' [-Wunused-variable]
bionic/libc/netbsd/resolv/res_init.c:175:6: warning: unused variable 'haveenv' [-Wunused-variable]
bionic/libc/netbsd/resolv/res_init.c:172:15: warning: unused variable 'n' [-Wunused-variable]
bionic/libc/netbsd/resolv/res_init.c:170:17: warning: unused variable 'fp' [-Wunused-variable]
bionic/libc/netbsd/resolv/res_init.c: In function 'real_randomid':
bionic/libc/netbsd/resolv/res_init.c:618:2: warning: statement with no effect [-Wunused-value]
bionic/libc/netbsd/resolv/res_init.c: At top level:
bionic/libc/netbsd/resolv/res_init.c:595:1: warning: 'net_mask' defined but not used [-Wunused-function]
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_mkquery.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_query.c
bionic/libc/netbsd/resolv/res_query.c: In function '__res_nsearch':
bionic/libc/netbsd/resolv/res_query.c:282:3: warning: implicit declaration of function '_resolv_populate_res_for_iface' [-Wimplicit-function-declaration]
bionic/libc/netbsd/resolv/res_query.c: In function '__res_hostalias':
bionic/libc/netbsd/resolv/res_query.c:422:31: warning: unused parameter 'statp' [-Wunused-parameter]
bionic/libc/netbsd/resolv/res_query.c:422:50: warning: unused parameter 'name' [-Wunused-parameter]
bionic/libc/netbsd/resolv/res_query.c:422:62: warning: unused parameter 'dst' [-Wunused-parameter]
bionic/libc/netbsd/resolv/res_query.c:422:74: warning: unused parameter 'siz' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_send.c
bionic/libc/netbsd/resolv/res_send.c: In function '__res_ourserver_p':
bionic/libc/netbsd/resolv/res_send.c:263:8: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:263:8: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:263:8: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:263:8: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c: In function '__res_nsend':
bionic/libc/netbsd/resolv/res_send.c:428:26: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:429:19: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:438:17: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:442:26: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c: In function 'get_nsaddr':
bionic/libc/netbsd/resolv/res_send.c:708:18: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:715:18: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c: In function 'send_vc':
bionic/libc/netbsd/resolv/res_send.c:768:13: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:769:24: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c: In function 'send_dg':
bionic/libc/netbsd/resolv/res_send.c:1160:15: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/resolv/res_send.c:1194:38: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_state.c
target thumb C: libc_common <= bionic/libc/netbsd/resolv/res_cache.c
bionic/libc/netbsd/resolv/res_cache.c: In function '_resolv_populate_res_for_iface':
bionic/libc/netbsd/resolv/res_cache.c:2683:19: warning: assignment from incompatible pointer type [enabled by default]
target thumb C: libc_common <= bionic/libc/netbsd/net/nsdispatch.c
bionic/libc/netbsd/net/nsdispatch.c: In function '_nsmethod':
bionic/libc/netbsd/net/nsdispatch.c:91:43: warning: unused parameter 'database' [-Wunused-parameter]
bionic/libc/netbsd/net/nsdispatch.c:91:65: warning: unused parameter 'method' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/netbsd/net/getaddrinfo.c
bionic/libc/netbsd/net/getaddrinfo.c: In function 'android_getaddrinfo_proxy':
bionic/libc/netbsd/net/getaddrinfo.c:441:6: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:441:6: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c: In function 'getanswer':
bionic/libc/netbsd/net/getaddrinfo.c:1439:5: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1439:5: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1439:5: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c: In function '_get_scope':
bionic/libc/netbsd/net/getaddrinfo.c:1501:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1501:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1501:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1501:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c: In function '_get_label':
bionic/libc/netbsd/net/getaddrinfo.c:1563:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1563:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1563:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1563:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1565:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1565:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1565:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1569:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1573:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1573:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1573:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1573:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1573:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c: In function '_get_precedence':
bionic/libc/netbsd/net/getaddrinfo.c:1605:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1605:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1605:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1605:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1607:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1607:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1607:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1611:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1615:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1615:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1615:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1615:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c:1615:3: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getaddrinfo.c: In function '_using_default_dns':
bionic/libc/netbsd/net/getaddrinfo.c:1876:2: warning: implicit declaration of function '_resolv_get_default_iface' [-Wimplicit-function-declaration]
bionic/libc/netbsd/net/getaddrinfo.c: In function '_dns_getaddrinfo':
bionic/libc/netbsd/net/getaddrinfo.c:1885:34: warning: unused parameter 'cb_data' [-Wunused-parameter]
bionic/libc/netbsd/net/getaddrinfo.c: In function '_files_getaddrinfo':
bionic/libc/netbsd/net/getaddrinfo.c:2116:36: warning: unused parameter 'cb_data' [-Wunused-parameter]
bionic/libc/netbsd/net/getaddrinfo.c: In function 'res_searchN':
bionic/libc/netbsd/net/getaddrinfo.c:2323:3: warning: implicit declaration of function '_resolv_populate_res_for_iface' [-Wimplicit-function-declaration]
target thumb C: libc_common <= bionic/libc/netbsd/net/getnameinfo.c
bionic/libc/netbsd/net/getnameinfo.c: In function 'android_gethostbyaddr_proxy':
bionic/libc/netbsd/net/getnameinfo.c:164:4: warning: implicit declaration of function 'android_gethostbyaddrforiface_proxy' [-Wimplicit-function-declaration]
bionic/libc/netbsd/net/getnameinfo.c:164:4: warning: initialization makes pointer from integer without a cast [enabled by default]
bionic/libc/netbsd/net/getnameinfo.c: In function 'getnameinfo_inet':
bionic/libc/netbsd/net/getnameinfo.c:264:4: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getnameinfo.c:264:4: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getnameinfo.c:264:4: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getnameinfo.c:266:4: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getnameinfo.c:266:4: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getnameinfo.c:266:4: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getnameinfo.c:266:4: warning: dereferencing type-punned pointer will break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/netbsd/net/getnameinfo.c: In function 'ip6_sa2str':
bionic/libc/netbsd/net/getnameinfo.c:422:74: warning: unused parameter 'flags' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/netbsd/net/getservbyname.c
bionic/libc/netbsd/net/getservbyname.c: In function 'getservbyname':
bionic/libc/netbsd/net/getservbyname.c:37:22: warning: unused variable 's' [-Wunused-variable]
target thumb C: libc_common <= bionic/libc/netbsd/net/getservent.c
bionic/libc/netbsd/net/getservent.c: In function 'setservent':
bionic/libc/netbsd/net/getservent.c:36:16: warning: unused parameter 'f' [-Wunused-parameter]
target thumb C: libc_common <= bionic/libc/netbsd/net/base64.c
target thumb C: libc_common <= bionic/libc/netbsd/net/getservbyport.c
bionic/libc/netbsd/net/getservbyport.c: In function 'getservbyport':
bionic/libc/netbsd/net/getservbyport.c:36:22: warning: unused variable 's' [-Wunused-variable]
target thumb C: libc_common <= bionic/libc/netbsd/nameser/ns_name.c
target thumb C: libc_common <= bionic/libc/netbsd/nameser/ns_parse.c
target thumb C: libc_common <= bionic/libc/netbsd/nameser/ns_ttl.c
target thumb C: libc_common <= bionic/libc/netbsd/nameser/ns_netint.c
target thumb C: libc_common <= bionic/libc/netbsd/nameser/ns_print.c
target thumb C: libc_common <= bionic/libc/netbsd/nameser/ns_samedomain.c
target thumb C: libc_common <= bionic/libc/string/strncmp.c
target thumb C: libc_common <= bionic/libc/string/strncat.c
target thumb C: libc_common <= bionic/libc/string/strncpy.c
target thumb C: libc_common <= bionic/libc/string/strrchr.c
target thumb C: libc_common <= bionic/libc/bionic/memrchr.c
target thumb C: libc_common <= bionic/libc/string/index.c
target thumb C: libc_common <= bionic/libc/bionic/strnlen.c
target thumb C: libc_common <= bionic/libc/string/strlcat.c
target thumb C: libc_common <= bionic/libc/string/strlcpy.c
target thumb C: libc_common <= bionic/libc/upstream-freebsd/lib/libc/string/wcschr.c
target thumb C: libc_common <= bionic/libc/upstream-freebsd/lib/libc/string/wcsrchr.c
target thumb C: libc_common <= bionic/libc/upstream-freebsd/lib/libc/string/wcscmp.c
target thumb C: libc_common <= bionic/libc/upstream-freebsd/lib/libc/string/wcscpy.c
target thumb C: libc_common <= bionic/libc/upstream-freebsd/lib/libc/string/wmemcmp.c
target thumb C: libc_common <= bionic/libc/upstream-freebsd/lib/libc/string/wcslen.c
target thumb C: libc_common <= bionic/libc/upstream-freebsd/lib/libc/string/wcscat.c
target thumb C: libc_common <= bionic/libc/arch-arm/bionic/atomics_arm.c
target thumb C: libc_common <= bionic/libc/arch-arm/bionic/eabi.c
target thumb C: libc_common <= bionic/libc/arch-arm/bionic/libgcc_compat.c
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbionic_ssp_intermediates/import_includes
target thumb C++: libbionic_ssp <= bionic/libc/bionic/__stack_chk_fail.cpp
target StaticLib: libbionic_ssp (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbionic_ssp_intermediates/libbionic_ssp.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_bionic_intermediates/import_includes
target thumb C++: libc_bionic <= bionic/libc/bionic/abort.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/assert.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/brk.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/dirent.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/eventfd_read.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/eventfd_write.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/futimens.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/getauxval.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/getcwd.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/libc_init_common.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/libc_logging.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/libgen.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/mmap.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_attr.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_detach.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_equal.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_getcpuclockid.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_getschedparam.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_internals.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_join.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_kill.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_self.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_setname_np.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_setschedparam.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/pthread_sigmask.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/raise.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/sbrk.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/scandir.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/sched_getaffinity.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/__set_errno.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/setlocale.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/signalfd.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/sigwait.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/statvfs.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/strerror.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/strerror_r.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/strsignal.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/stubs.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/sysconf.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/tdestroy.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/tmpfile.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/wait.cpp
target thumb C++: libc_bionic <= bionic/libc/bionic/wchar.cpp
target thumb C: libc_bionic <= bionic/libc/bionic/__errno.c
target StaticLib: libc_bionic (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_bionic_intermediates/libc_bionic.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_freebsd_intermediates/import_includes
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/clrerr.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fclose.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fdopen.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/feof.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/ferror.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fgetln.c
bionic/libc/upstream-freebsd/lib/libc/stdio/fgetln.c: In function '__slbexpand':
bionic/libc/upstream-freebsd/lib/libc/stdio/fgetln.c:62:20: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fgetpos.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fgets.c
bionic/libc/upstream-freebsd/lib/libc/stdio/fgets.c: In function 'fgets':
bionic/libc/upstream-freebsd/lib/libc/stdio/fgets.c:88:11: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fileno.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/flags.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fopen.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fpurge.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fputs.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fsetpos.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/funopen.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fwalk.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/fwrite.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/getc.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/getchar.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/makebuf.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/mktemp.c
bionic/libc/upstream-freebsd/lib/libc/stdio/mktemp.c: In function '_gettemp':
bionic/libc/upstream-freebsd/lib/libc/stdio/mktemp.c:123:3: warning: implicit declaration of function 'arc4random_uniform' [-Wimplicit-function-declaration]
bionic/libc/upstream-freebsd/lib/libc/stdio/mktemp.c:171:4: warning: pointer targets in passing argument 1 of 'strchr' differ in signedness [-Wpointer-sign]
In file included from bionic/libc/include/signal.h:34:0,
                 from bionic/libc/include/sys/select.h:34,
                 from bionic/libc/include/unistd.h:34,
                 from bionic/libc/include/fcntl.h:34,
                 from bionic/libc/upstream-freebsd/lib/libc/stdio/mktemp.c:39:
bionic/libc/include/string.h:232:7: note: expected 'const char *' but argument is of type 'const unsigned char *'
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/putc.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/putchar.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/puts.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/putw.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/remove.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/rget.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/setbuf.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/setbuffer.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/setvbuf.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/tempnam.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/tmpnam.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdio/wsetup.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdlib/abs.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdlib/getopt_long.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdlib/imaxabs.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdlib/imaxdiv.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdlib/labs.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdlib/llabs.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdlib/qsort.c
bionic/libc/upstream-freebsd/lib/libc/stdlib/qsort.c: In function 'qsort':
bionic/libc/upstream-freebsd/lib/libc/stdlib/qsort.c:180:6: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
bionic/libc/upstream-freebsd/lib/libc/stdlib/qsort.c:180:6: warning: signed and unsigned type in conditional expression [-Wsign-compare]
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/stdlib/realpath.c
bionic/libc/upstream-freebsd/lib/libc/stdlib/realpath.c: In function 'realpath':
bionic/libc/upstream-freebsd/lib/libc/stdlib/realpath.c:113:16: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
bionic/libc/upstream-freebsd/lib/libc/stdlib/realpath.c:220:19: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcpcpy.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcpncpy.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcscasecmp.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcscspn.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcsdup.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcslcat.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcslcpy.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcsncasecmp.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcsncat.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcsncmp.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcsncpy.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcsnlen.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcspbrk.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcsspn.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcsstr.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wcstok.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wmemchr.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wmemcpy.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wmemmove.c
target thumb C: libc_freebsd <= bionic/libc/upstream-freebsd/lib/libc/string/wmemset.c
target StaticLib: libc_freebsd (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_freebsd_intermediates/libc_freebsd.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_netbsd_intermediates/import_includes
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/common/lib/libc/hash/sha1/sha1.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/common/lib/libc/inet/inet_addr.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/compat-43/creat.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/gen/ftw.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/gen/nftw.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/gen/nice.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/gen/popen.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/gen/psignal.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/gen/setjmperr.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/gen/utime.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/inet/inet_ntoa.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/inet/inet_ntop.c
bionic/libc/upstream-netbsd/libc/inet/inet_ntop.c: In function 'inet_ntop6':
bionic/libc/upstream-netbsd/libc/inet/inet_ntop.c:224:25: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/inet/inet_pton.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/isc/ev_streams.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/isc/ev_timers.c
bionic/libc/upstream-netbsd/libc/isc/ev_timers.c: In function '__evNowTime':
bionic/libc/upstream-netbsd/libc/isc/ev_timers.c:136:2: warning: implicit declaration of function 'clock_gettime' [-Wimplicit-function-declaration]
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/regex/regcomp.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/regex/regerror.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/regex/regexec.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/regex/regfree.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdio/getdelim.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdio/getline.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/bsearch.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/div.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/drand48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/erand48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/exit.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/jrand48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/ldiv.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/lldiv.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/lrand48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/mrand48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/nrand48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/_rand48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/seed48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/srand48.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/tdelete.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/tfind.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/stdlib/tsearch.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/string/memccpy.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/string/strcasestr.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/string/strcoll.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/string/strxfrm.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/thread-stub/__isthreaded.c
target thumb C: libc_netbsd <= bionic/libc/upstream-netbsd/libc/unistd/killpg.c
target StaticLib: libc_netbsd (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_netbsd_intermediates/libc_netbsd.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_tzcode_intermediates/import_includes
target thumb C: libc_tzcode <= bionic/libc/tzcode/asctime.c
target thumb C: libc_tzcode <= bionic/libc/tzcode/difftime.c
target thumb C: libc_tzcode <= bionic/libc/tzcode/localtime.c
bionic/libc/tzcode/localtime.c: In function 'differ_by_repeat':
bionic/libc/tzcode/localtime.c:340:2: warning: comparison is always false due to limited range of data type [-Wtype-limits]
bionic/libc/tzcode/localtime.c: In function 'localsub':
bionic/libc/tzcode/localtime.c:1352:27: warning: assignment discards 'const' qualifier from pointer target type [enabled by default]
target thumb C: libc_tzcode <= bionic/libc/tzcode/strftime.c
bionic/libc/tzcode/strftime.c:3:13: warning: 'elsieid' defined but not used [-Wunused-variable]
target thumb C: libc_tzcode <= bionic/libc/tzcode/strptime.c
target StaticLib: libc_tzcode (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_tzcode_intermediates/libc_tzcode.a)
preparing StaticLib: libc_common [including  /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbionic_ssp_intermediates/libbionic_ssp.a]
preparing StaticLib: libc_common [including  /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_bionic_intermediates/libc_bionic.a]
preparing StaticLib: libc_common [including  /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_freebsd_intermediates/libc_freebsd.a]
preparing StaticLib: libc_common [including  /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_netbsd_intermediates/libc_netbsd.a]
preparing StaticLib: libc_common [including  /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_tzcode_intermediates/libc_tzcode.a]
target StaticLib: libc_common (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_common_intermediates/libc_common.a)
target SharedLib: libc (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libc_intermediates/LINKED/libc.so)
target Symbolic: libc (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/system/lib/libc.so)
target Strip: libc (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libc.so)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libstdc++_intermediates/import_includes
target thumb C++: libstdc++ <= bionic/libstdc++/src/one_time_construction.cpp
target thumb C++: libstdc++ <= bionic/libstdc++/src/new.cpp
target thumb C++: libstdc++ <= bionic/libstdc++/src/pure_virtual.cpp
target thumb C++: libstdc++ <= bionic/libstdc++/src/typeinfo.cpp
target SharedLib: libstdc++ (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libstdc++_intermediates/LINKED/libstdc++.so)
target Symbolic: libstdc++ (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/system/lib/libstdc++.so)
target Strip: libstdc++ (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libstdc++.so)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libm_intermediates/import_includes
target arm C: libm <= bionic/libm/digittoint.c
target arm C: libm <= bionic/libm/fpclassify.c
target arm C: libm <= bionic/libm/isinf.c
target arm C: libm <= bionic/libm/sincos.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/bsdsrc/b_exp.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/bsdsrc/b_log.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/bsdsrc/b_tgamma.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_acos.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_acosf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_acosh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_acoshf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_asin.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_asinf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_atan2.c
bionic/libm/upstream-freebsd/lib/msun/src/e_atan2.c: In function 'atan2':
bionic/libm/upstream-freebsd/lib/msun/src/e_atan2.c:74:2: warning: suggest parentheses around arithmetic in operand of '|' [-Wparentheses]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_atan2f.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_atanh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_atanhf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_cosh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_coshf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_exp.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_expf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_fmod.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_fmodf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_gamma.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_gammaf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_gammaf_r.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_gamma_r.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_hypot.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_hypotf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_j0.c
bionic/libm/upstream-freebsd/lib/msun/src/e_j0.c: In function 'pzero':
bionic/libm/upstream-freebsd/lib/msun/src/e_j0.c:284:22: warning: 'q' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j0.c:283:15: warning: 'p' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j0.c: In function 'qzero':
bionic/libm/upstream-freebsd/lib/msun/src/e_j0.c:379:22: warning: 'q' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j0.c:378:15: warning: 'p' may be used uninitialized in this function [-Wmaybe-uninitialized]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c: In function 'j0f':
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c:65:8: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c: In function 'y0f':
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c:139:22: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c: In function 'pzerof':
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c:240:22: warning: 'q' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c:239:15: warning: 'p' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c: In function 'qzerof':
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c:335:22: warning: 'q' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j0f.c:334:15: warning: 'p' may be used uninitialized in this function [-Wmaybe-uninitialized]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_j1.c
bionic/libm/upstream-freebsd/lib/msun/src/e_j1.c: In function 'pone':
bionic/libm/upstream-freebsd/lib/msun/src/e_j1.c:278:29: warning: 'q' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j1.c:277:22: warning: 'p' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j1.c: In function 'qone':
bionic/libm/upstream-freebsd/lib/msun/src/e_j1.c:374:22: warning: 'q' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j1.c:373:15: warning: 'p' may be used uninitialized in this function [-Wmaybe-uninitialized]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c
bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c: In function 'j1f':
bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c:66:8: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c: In function 'ponef':
bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c:235:29: warning: 'q' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c:234:22: warning: 'p' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c: In function 'qonef':
bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c:331:22: warning: 'q' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_j1f.c:330:15: warning: 'p' may be used uninitialized in this function [-Wmaybe-uninitialized]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_jn.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_jnf.c
bionic/libm/upstream-freebsd/lib/msun/src/e_jnf.c: In function 'ynf':
bionic/libm/upstream-freebsd/lib/msun/src/e_jnf.c:192:17: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_lgamma.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_lgammaf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_lgammaf_r.c
bionic/libm/include/math.h: In function 'lgammaf_r':
bionic/libm/upstream-freebsd/lib/msun/src/e_lgammaf_r.c:228:13: warning: 'nadj' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_lgammaf_r.c:140:14: note: 'nadj' was declared here
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_lgamma_r.c
bionic/libm/include/math.h: In function 'lgamma_r':
bionic/libm/upstream-freebsd/lib/msun/src/e_lgamma_r.c:295:13: warning: 'nadj' may be used uninitialized in this function [-Wmaybe-uninitialized]
bionic/libm/upstream-freebsd/lib/msun/src/e_lgamma_r.c:207:15: note: 'nadj' was declared here
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_log10.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_log10f.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_log2.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_log2f.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_log.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_logf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_pow.c
bionic/libm/upstream-freebsd/lib/msun/src/e_pow.c: In function 'pow':
bionic/libm/upstream-freebsd/lib/msun/src/e_pow.c:116:16: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
bionic/libm/upstream-freebsd/lib/msun/src/e_pow.c:153:21: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_powf.c
bionic/libm/upstream-freebsd/lib/msun/src/e_powf.c: In function 'powf':
bionic/libm/upstream-freebsd/lib/msun/src/e_powf.c:216:12: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_remainder.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_remainderf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_rem_pio2.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_rem_pio2f.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_scalb.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_scalbf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_sinh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_sinhf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_cos.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_cosf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_exp.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_expf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_rem_pio2.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_sin.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_sinf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_tan.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/k_tanf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_asinh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_asinhf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_atan.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_atanf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_carg.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cargf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cbrt.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cbrtf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_ccosh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_ccoshf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_ceil.c
bionic/libm/upstream-freebsd/lib/msun/src/s_ceil.c: In function 'ceil':
bionic/libm/upstream-freebsd/lib/msun/src/s_ceil.c:64:8: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_ceilf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cexp.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cexpf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cimag.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cimagf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_conj.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_conjf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_copysign.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_copysignf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cosf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cproj.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cprojf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_creal.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_crealf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_csinh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_csinhf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_csqrt.c
bionic/libm/upstream-freebsd/lib/msun/src/s_csqrt.c:43:0: warning: ignoring #pragma STDC CX_LIMITED_RANGE [-Wunknown-pragmas]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_csqrtf.c
bionic/libm/upstream-freebsd/lib/msun/src/s_csqrtf.c:42:0: warning: ignoring #pragma STDC CX_LIMITED_RANGE [-Wunknown-pragmas]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_ctanh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_ctanhf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_erf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_erff.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_exp2.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_exp2f.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_expm1.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_expm1f.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fabs.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fabsf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fdim.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_finite.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_finitef.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_floor.c
bionic/libm/upstream-freebsd/lib/msun/src/s_floor.c: In function 'floor':
bionic/libm/upstream-freebsd/lib/msun/src/s_floor.c:65:8: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_floorf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fma.c
bionic/libm/upstream-freebsd/lib/msun/src/s_fma.c: In function 'add_and_denormalize':
bionic/libm/upstream-freebsd/lib/msun/src/s_fma.c:120:3: warning: suggest parentheses around comparison in operand of '^' [-Wparentheses]
bionic/libm/upstream-freebsd/lib/msun/src/s_fma.c: In function 'fma':
bionic/libm/upstream-freebsd/lib/msun/src/s_fma.c:219:4: warning: suggest parentheses around comparison in operand of '^' [-Wparentheses]
bionic/libm/upstream-freebsd/lib/msun/src/s_fma.c:219:4: warning: suggest parentheses around comparison in operand of '^' [-Wparentheses]
bionic/libm/upstream-freebsd/lib/msun/src/s_fma.c:224:4: warning: suggest parentheses around comparison in operand of '^' [-Wparentheses]
bionic/libm/upstream-freebsd/lib/msun/src/s_fma.c:229:4: warning: suggest parentheses around comparison in operand of '^' [-Wparentheses]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fmaf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fmax.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fmaxf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fmin.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_fminf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_frexp.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_frexpf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_ilogb.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_ilogbf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_isfinite.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_isnan.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_isnormal.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_llrint.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_llrintf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_llround.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_llroundf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_log1p.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_log1pf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_logb.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_logbf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_lrint.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_lrintf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_lround.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_lroundf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_modf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_modff.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_nan.c
bionic/libm/upstream-freebsd/lib/msun/src/s_nan.c: In function '_scan_nan':
bionic/libm/upstream-freebsd/lib/msun/src/s_nan.c:74:3: warning: implicit declaration of function 'digittoint' [-Wimplicit-function-declaration]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_nearbyint.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_nextafter.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_nextafterf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_nexttowardf.c
bionic/libm/upstream-freebsd/lib/msun/src/s_nexttowardf.c: In function 'nexttowardf':
bionic/libm/upstream-freebsd/lib/msun/src/s_nexttowardf.c:44:2: warning: suggest parentheses around comparison in operand of '^' [-Wparentheses]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_remquo.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_remquof.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_rint.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_rintf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_round.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_roundf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_scalbln.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_scalbn.c
bionic/libm/upstream-freebsd/lib/msun/src/s_scalbn.c: In function 'scalbn':
bionic/libm/upstream-freebsd/lib/msun/src/s_scalbn.c:54:12: warning: suggest explicit braces to avoid ambiguous 'else' [-Wparentheses]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_scalbnf.c
bionic/libm/upstream-freebsd/lib/msun/src/s_scalbnf.c: In function 'scalbnf':
bionic/libm/upstream-freebsd/lib/msun/src/s_scalbnf.c:49:12: warning: suggest explicit braces to avoid ambiguous 'else' [-Wparentheses]
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_signbit.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_signgam.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_significand.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_significandf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_sinf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_tan.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_tanf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_tanh.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_tanhf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_tgammaf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_trunc.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_truncf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/w_cabs.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/w_cabsf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/w_drem.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/w_dremf.c
target arm C: libm <= bionic/libm/fake_long_double.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_cos.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/s_sin.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_sqrtf.c
target arm C: libm <= bionic/libm/upstream-freebsd/lib/msun/src/e_sqrt.c
bionic/libm/upstream-freebsd/lib/msun/src/e_sqrt.c: In function 'sqrt':
bionic/libm/upstream-freebsd/lib/msun/src/e_sqrt.c:159:16: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target arm C: libm <= bionic/libm/arm/fenv.c
Export includes file: bionic/libm/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libm_intermediates/export_includes
target StaticLib: libm (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libm_intermediates/libm.a)
target SharedLib: libm (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libm_intermediates/LINKED/libm.so)
target Symbolic: libm (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/system/lib/libm.so)
target Strip: libm (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libm.so)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/liblog_intermediates/import_includes
target thumb C: liblog <= system/core/liblog/logd_write.c
target thumb C: liblog <= system/core/liblog/logprint.c
target thumb C: liblog <= system/core/liblog/event_tag_map.c
Export includes file: system/core/liblog/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/liblog_intermediates/export_includes
target StaticLib: liblog (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/liblog_intermediates/liblog.a)
target SharedLib: liblog (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/liblog_intermediates/LINKED/liblog.so)
target Symbolic: liblog (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/system/lib/liblog.so)
target Strip: liblog (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/liblog.so)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libcutils_intermediates/import_includes
target asm: libcutils <= system/core/libcutils/arch-arm/memset32.S
target arm C: libcutils <= system/core/libcutils/atomic.c
target thumb C: libcutils <= system/core/libcutils/hashmap.c
target thumb C: libcutils <= system/core/libcutils/native_handle.c
target thumb C: libcutils <= system/core/libcutils/socket_inaddr_any_server.c
target thumb C: libcutils <= system/core/libcutils/socket_local_client.c
target thumb C: libcutils <= system/core/libcutils/socket_local_server.c
target thumb C: libcutils <= system/core/libcutils/socket_loopback_client.c
target thumb C: libcutils <= system/core/libcutils/socket_loopback_server.c
target thumb C: libcutils <= system/core/libcutils/socket_network_client.c
target thumb C: libcutils <= system/core/libcutils/sockets.c
target thumb C: libcutils <= system/core/libcutils/config_utils.c
target thumb C: libcutils <= system/core/libcutils/cpu_info.c
target thumb C: libcutils <= system/core/libcutils/load_file.c
target thumb C: libcutils <= system/core/libcutils/list.c
target thumb C: libcutils <= system/core/libcutils/open_memstream.c
target thumb C: libcutils <= system/core/libcutils/strdup16to8.c
target thumb C: libcutils <= system/core/libcutils/strdup8to16.c
target thumb C: libcutils <= system/core/libcutils/record_stream.c
target thumb C: libcutils <= system/core/libcutils/process_name.c
target thumb C: libcutils <= system/core/libcutils/threads.c
target thumb C: libcutils <= system/core/libcutils/sched_policy.c
target thumb C: libcutils <= system/core/libcutils/iosched_policy.c
system/core/libcutils/iosched_policy.c: In function 'android_get_ioprio':
system/core/libcutils/iosched_policy.c:54:5: warning: implicit declaration of function 'ioprio_get' [-Wimplicit-function-declaration]
target thumb C: libcutils <= system/core/libcutils/str_parms.c
target thumb C: libcutils <= system/core/libcutils/fs.c
target thumb C: libcutils <= system/core/libcutils/multiuser.c
target thumb C: libcutils <= system/core/libcutils/android_reboot.c
target thumb C: libcutils <= system/core/libcutils/ashmem-dev.c
target thumb C: libcutils <= system/core/libcutils/debugger.c
target thumb C: libcutils <= system/core/libcutils/klog.c
target thumb C: libcutils <= system/core/libcutils/partition_utils.c
target thumb C: libcutils <= system/core/libcutils/properties.c
target thumb C: libcutils <= system/core/libcutils/qtaguid.c
target thumb C: libcutils <= system/core/libcutils/trace.c
target thumb C: libcutils <= system/core/libcutils/uevent.c
Export includes file: system/core/libcutils/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libcutils_intermediates/export_includes
target StaticLib: libcutils (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libcutils_intermediates/libcutils.a)
target SharedLib: libcutils (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libcutils_intermediates/LINKED/libcutils.so)
target Symbolic: libcutils (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/system/lib/libcutils.so)
target Strip: libcutils (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libcutils.so)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libselinux_intermediates/import_includes
target thumb C: libselinux <= external/libselinux/src/booleans.c
target thumb C: libselinux <= external/libselinux/src/canonicalize_context.c
target thumb C: libselinux <= external/libselinux/src/disable.c
target thumb C: libselinux <= external/libselinux/src/enabled.c
target thumb C: libselinux <= external/libselinux/src/fgetfilecon.c
target thumb C: libselinux <= external/libselinux/src/fsetfilecon.c
target thumb C: libselinux <= external/libselinux/src/getenforce.c
target thumb C: libselinux <= external/libselinux/src/getfilecon.c
target thumb C: libselinux <= external/libselinux/src/getpeercon.c
target thumb C: libselinux <= external/libselinux/src/lgetfilecon.c
target thumb C: libselinux <= external/libselinux/src/load_policy.c
target thumb C: libselinux <= external/libselinux/src/lsetfilecon.c
target thumb C: libselinux <= external/libselinux/src/policyvers.c
target thumb C: libselinux <= external/libselinux/src/procattr.c
target thumb C: libselinux <= external/libselinux/src/setenforce.c
target thumb C: libselinux <= external/libselinux/src/setfilecon.c
target thumb C: libselinux <= external/libselinux/src/context.c
target thumb C: libselinux <= external/libselinux/src/mapping.c
target thumb C: libselinux <= external/libselinux/src/stringrep.c
target thumb C: libselinux <= external/libselinux/src/compute_create.c
target thumb C: libselinux <= external/libselinux/src/compute_av.c
target thumb C: libselinux <= external/libselinux/src/avc.c
target thumb C: libselinux <= external/libselinux/src/avc_internal.c
target thumb C: libselinux <= external/libselinux/src/avc_sidtab.c
target thumb C: libselinux <= external/libselinux/src/get_initial_context.c
target thumb C: libselinux <= external/libselinux/src/checkAccess.c
target thumb C: libselinux <= external/libselinux/src/sestatus.c
target thumb C: libselinux <= external/libselinux/src/deny_unknown.c
target thumb C: libselinux <= external/libselinux/src/callbacks.c
target thumb C: libselinux <= external/libselinux/src/check_context.c
target thumb C: libselinux <= external/libselinux/src/freecon.c
target thumb C: libselinux <= external/libselinux/src/init.c
target thumb C: libselinux <= external/libselinux/src/label.c
target thumb C: libselinux <= external/libselinux/src/label_file.c
target thumb C: libselinux <= external/libselinux/src/label_android_property.c
target thumb C: libselinux <= external/libselinux/src/android.c
target SharedLib: libselinux (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libselinux_intermediates/LINKED/libselinux.so)
target Symbolic: libselinux (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/system/lib/libselinux.so)
target Strip: libselinux (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libselinux.so)
target Executable: toolbox_recovery (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/toolbox_recovery_intermediates/LINKED/toolbox)
target Symbolic: toolbox_recovery (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/recovery/root/sbin/toolbox)
Export includes file: bootable/recovery/openaes/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/toolbox_recovery_intermediates/export_includes
target Strip: toolbox_recovery (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/toolbox_recovery_intermediates/toolbox)
Notice file: system/core/toolbox//NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//recovery/root/sbin/toolbox.txt
Notice file: bionic/libc/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libc.so.txt
Notice file: bionic/libc/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libc_common.a.txt
target Prebuilt: tzdata (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/tzdata_intermediates/tzdata)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/usr/share/zoneinfo/tzdata
Notice file: bionic/libdl/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libdl.so.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libdl.so
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libc.so
Notice file: system/core/libcutils/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libcutils.so.txt
Notice file: system/core/libcutils/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libcutils.a.txt
Notice file: system/core/liblog/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/liblog.a.txt
Notice file: system/core/liblog/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/liblog.so.txt
Notice file: bionic/libm/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libm.so.txt
Notice file: bionic/libm/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libm.a.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libm.so
Notice file: bionic/libstdc++/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libstdc++.so.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libstdc++.so
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/liblog.so
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libcutils.so
Notice file: external/libselinux/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libselinux.so.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libselinux.so
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/chcon -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/chgrp -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/chmod -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/chown -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/chroot -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/clear -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/cmp -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/comm -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/cp -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/cpio -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/crond -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/crontab -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/cut -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/date -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/dc -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/dd -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/depmod -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/devmem -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/df -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/diff -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/dirname -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/dmesg -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/dnsd -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/dos2unix -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/du -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/echo -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ed -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/egrep -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/env -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/expand -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/expr -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/false -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/fbsplash -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/fdisk -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/fgrep -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/find -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/flash_lock -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/flash_unlock -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/flashcp -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/flock -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/fold -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/free -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/freeramdisk -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/fstrim -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/fsync -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ftpget -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ftpput -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/fuser -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/getenforce -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/getopt -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/getprop -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/getsebool -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/grep -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/groups -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/halt -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/head -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/hexdump -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/id -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ifconfig -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/inetd -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/insmod -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/install -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ionice -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/iostat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ip -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/kill -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/killall -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/killall5 -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/less -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ln -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/load_policy -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/losetup -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ls -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/lsattr -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/lsmod -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/lsusb -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/lzcat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/lzma -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/lzop -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/lzopcat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/man -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/md5sum -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mesg -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mkdir -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mkfifo -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mkfs.ext2 -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mkfs.vfat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mknod -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mkswap -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mktemp -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/modinfo -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/modprobe -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/more -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mount -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mountpoint -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mpstat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/mv -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/nanddump -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/nandwrite -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/nbd-client -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/nc -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/netstat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/nice -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/nohup -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/nslookup -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ntpd -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/od -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/patch -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pgrep -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pidof -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ping -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pipe_progress -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pkill -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pmap -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/poweroff -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/printenv -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/printf -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ps -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pstree -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pwd -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pwdx -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/rdev -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/readlink -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/realpath -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/renice -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/reset -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/resize -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/restorecon -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/rev -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/rm -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/rmdir -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/rmmod -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/route -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/run-parts -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/runcon -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/rx -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sed -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/seq -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/setconsole -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/setenforce -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/setprop -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/setsebool -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/setserial -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/setsid -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sh -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sha1sum -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sha256sum -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sha3sum -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sha512sum -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sleep -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sort -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/split -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/start -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/stat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/stop -> toolbox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/strings -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/stty -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sum -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/swapoff -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/swapon -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sync -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/sysctl -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/tac -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/tail -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/tar -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/taskset -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/tee -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/telnet -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/telnetd -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/test -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/tftp -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/tftpd -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/time -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/timeout -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/top -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/touch -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/tr -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/traceroute -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/true -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/ttysize -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/umount -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/uname -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/uncompress -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/unexpand -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/uniq -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/unix2dos -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/unlzma -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/unlzop -> busybox
Export includes file: external/zlib/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libz_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/RECOVERY_EXECUTABLES/pigz_intermediates/import_includes
target thumb C: pigz <= bootable/recovery/pigz/pigz.c
bootable/recovery/pigz/pigz.c: In function 'process':
bootable/recovery/pigz/pigz.c:2994:47: warning: signed and unsigned type in conditional expression [-Wsign-compare]
target thumb C: pigz <= bootable/recovery/pigz/yarn.c
bootable/recovery/pigz/yarn.c: In function 'destruct':
bootable/recovery/pigz/yarn.c:372:5: warning: implicit declaration of function 'pthread_cancel' [-Wimplicit-function-declaration]
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libz_intermediates/import_includes
target asm: libz <= external/zlib/src/contrib/inflateneon/inflate_fast_copy_neon.s
target arm C: libz <= external/zlib/src/adler32.c
target arm C: libz <= external/zlib/src/compress.c
target arm C: libz <= external/zlib/src/crc32.c
target arm C: libz <= external/zlib/src/deflate.c
target arm C: libz <= external/zlib/src/gzclose.c
target arm C: libz <= external/zlib/src/gzlib.c
target arm C: libz <= external/zlib/src/gzread.c
target arm C: libz <= external/zlib/src/gzwrite.c
target arm C: libz <= external/zlib/src/infback.c
target arm C: libz <= external/zlib/src/inflate.c
target arm C: libz <= external/zlib/src/inftrees.c
target arm C: libz <= external/zlib/src/inffast.c
target arm C: libz <= external/zlib/src/trees.c
target arm C: libz <= external/zlib/src/uncompr.c
target arm C: libz <= external/zlib/src/zutil.c
target SharedLib: libz (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libz_intermediates/LINKED/libz.so)
target Symbolic: libz (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/system/lib/libz.so)
target Strip: libz (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/lib/libz.so)
target Executable: pigz (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/RECOVERY_EXECUTABLES/pigz_intermediates/LINKED/pigz)
target Symbolic: pigz (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/recovery/root/sbin/pigz)
Export includes file: bootable/recovery/pigz/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/RECOVERY_EXECUTABLES/pigz_intermediates/export_includes
target Strip: pigz (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/RECOVERY_EXECUTABLES/pigz_intermediates/pigz)
Notice file: external/zlib/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libz.so.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/system/lib/libz.so
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/pigz
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/unpigz -> pigz
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/unxz -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/unzip -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/uptime -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/usleep -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/uudecode -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/uuencode -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/vi -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/watch -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/wc -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/wget -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/which -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/whoami -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/xargs -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/xz -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/xzcat -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/yes -> busybox
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/sbin/zcat -> busybox
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/usb.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/recovery/root/etc/twrp.fstab
Export includes file: bootable/recovery/minui/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libminui_intermediates/export_includes
Export includes file: system/core/libpixelflinger/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libpixelflinger_static_intermediates/export_includes
Export includes file: external/libpng/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libpng_intermediates/export_includes
Export includes file: system/core/libsuspend/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libsuspend_intermediates/export_includes
Export includes file: external/zlib/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libz_intermediates/export_includes
Export includes file: bionic/libstdc++/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libstdc++_intermediates/export_includes
Export includes file: bionic/libc/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/charger_intermediates/import_includes
target thumb C: charger <= system/core/charger/charger.c
system/core/charger/charger.c: In function 'alarm_set_reboot_time':
system/core/charger/charger.c:1111:3: warning: format '%d' expects argument of type 'int', but argument 3 has type 'time_t' [-Wformat]
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libminui_intermediates/import_includes
target thumb C: libminui <= bootable/recovery/minui/events.c
target thumb C: libminui <= bootable/recovery/minui/resources.c
bootable/recovery/minui/resources.c: In function 'res_create_surface':
bootable/recovery/minui/resources.c:99:13: warning: passing argument 3 of 'png_get_IHDR' from incompatible pointer type [enabled by default]
In file included from bootable/recovery/minui/resources.c:32:0:
external/libpng/png.h:2470:8: note: expected 'png_uint_32 *' but argument is of type 'size_t *'
bootable/recovery/minui/resources.c:99:13: warning: passing argument 4 of 'png_get_IHDR' from incompatible pointer type [enabled by default]
In file included from bootable/recovery/minui/resources.c:32:0:
external/libpng/png.h:2470:8: note: expected 'png_uint_32 *' but argument is of type 'size_t *'
bootable/recovery/minui/resources.c: In function 'res_create_localized_surface':
bootable/recovery/minui/resources.c:254:13: warning: passing argument 3 of 'png_get_IHDR' from incompatible pointer type [enabled by default]
In file included from bootable/recovery/minui/resources.c:32:0:
external/libpng/png.h:2470:8: note: expected 'png_uint_32 *' but argument is of type 'size_t *'
bootable/recovery/minui/resources.c:254:13: warning: passing argument 4 of 'png_get_IHDR' from incompatible pointer type [enabled by default]
In file included from bootable/recovery/minui/resources.c:32:0:
external/libpng/png.h:2470:8: note: expected 'png_uint_32 *' but argument is of type 'size_t *'
bootable/recovery/minui/resources.c:265:19: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
bootable/recovery/minui/resources.c:270:21: warning: pointer targets in initialization differ in signedness [-Wpointer-sign]
bootable/recovery/minui/resources.c:272:19: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
target thumb C: libminui <= bootable/recovery/minui/../../../device/samsung/fascinatemtd/recovery/graphics.c
target StaticLib: libminui (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libminui_intermediates/libminui.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libpixelflinger_static_intermediates/import_includes
target asm: libpixelflinger_static <= system/core/libpixelflinger/t32cb16blend.S
target asm: libpixelflinger_static <= system/core/libpixelflinger/col32cb16blend.S
target arm C++: libpixelflinger_static <= system/core/libpixelflinger/fixed.cpp
target arm C++: libpixelflinger_static <= system/core/libpixelflinger/picker.cpp
target arm C++: libpixelflinger_static <= system/core/libpixelflinger/pixelflinger.cpp
target arm C++: libpixelflinger_static <= system/core/libpixelflinger/trap.cpp
target arm C++: libpixelflinger_static <= system/core/libpixelflinger/scanline.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/ARMAssemblerInterface.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/ARMAssemblerProxy.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/ARMAssembler.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/CodeCache.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/GGLAssembler.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/load_store.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/blending.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/texturing.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/tinyutils/SharedBuffer.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/tinyutils/VectorImpl.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/format.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/clear.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/raster.cpp
target thumb C++: libpixelflinger_static <= system/core/libpixelflinger/buffer.cpp
target thumb C: libpixelflinger_static <= system/core/libpixelflinger/codeflinger/disassem.c
system/core/libpixelflinger/codeflinger/disassem.c:710:1: warning: initialization from incompatible pointer type [enabled by default]
system/core/libpixelflinger/codeflinger/disassem.c:710:1: warning: (near initialization for 'disassemble_di.di_printf') [enabled by default]
target StaticLib: libpixelflinger_static (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libpixelflinger_static_intermediates/libpixelflinger_static.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libpng_intermediates/import_includes
target thumb C: libpng <= external/libpng/png.c
external/libpng/png.c:722:12: warning: explicitly assigning a variable of type 'png_structp' (aka 'struct png_struct_def *') to itself [-Wself-assign]
   png_ptr = png_ptr;  /* Silence compiler warning about unused png_ptr */
   ~~~~~~~ ^ ~~~~~~~
external/libpng/png.c:754:12: warning: explicitly assigning a variable of type 'png_structp' (aka 'struct png_struct_def *') to itself [-Wself-assign]
   png_ptr = png_ptr;  /* Silence compiler warning about unused png_ptr */
   ~~~~~~~ ^ ~~~~~~~
external/libpng/png.c:762:12: warning: explicitly assigning a variable of type 'png_structp' (aka 'struct png_struct_def *') to itself [-Wself-assign]
   png_ptr = png_ptr;  /* Silence compiler warning about unused png_ptr */
   ~~~~~~~ ^ ~~~~~~~
external/libpng/png.c:770:12: warning: explicitly assigning a variable of type 'png_structp' (aka 'struct png_struct_def *') to itself [-Wself-assign]
   png_ptr = png_ptr;  /* Silence compiler warning about unused png_ptr */
   ~~~~~~~ ^ ~~~~~~~
4 warnings generated.
target thumb C: libpng <= external/libpng/pngerror.c
external/libpng/pngerror.c:351:12: warning: explicitly assigning a variable of type 'png_structp' (aka 'struct png_struct_def *') to itself [-Wself-assign]
   png_ptr = png_ptr; /* Make compiler happy */
   ~~~~~~~ ^ ~~~~~~~
1 warning generated.
target thumb C: libpng <= external/libpng/pnggccrd.c
target thumb C: libpng <= external/libpng/pngget.c
external/libpng/pngget.c:896:16: warning: explicitly assigning a variable of type 'int' to itself [-Wself-assign]
    flag_select=flag_select;
    ~~~~~~~~~~~^~~~~~~~~~~~
external/libpng/pngget.c:906:16: warning: explicitly assigning a variable of type 'int' to itself [-Wself-assign]
    flag_select=flag_select;
    ~~~~~~~~~~~^~~~~~~~~~~~
2 warnings generated.
target thumb C: libpng <= external/libpng/pngmem.c
target thumb C: libpng <= external/libpng/pngpread.c
external/libpng/pngpread.c:1212:19: warning: explicitly assigning a variable of type 'png_infop' (aka 'struct png_info_struct *') to itself [-Wself-assign]
         info_ptr = info_ptr; /* To quiet some compiler warnings */
         ~~~~~~~~ ^ ~~~~~~~~
external/libpng/pngpread.c:1310:19: warning: explicitly assigning a variable of type 'png_infop' (aka 'struct png_info_struct *') to itself [-Wself-assign]
         info_ptr = info_ptr; /* To quiet some compiler warnings */
         ~~~~~~~~ ^ ~~~~~~~~
external/libpng/pngpread.c:1646:16: warning: explicitly assigning a variable of type 'png_infop' (aka 'struct png_info_struct *') to itself [-Wself-assign]
      info_ptr = info_ptr; /* To quiet some compiler warnings */
      ~~~~~~~~ ^ ~~~~~~~~
3 warnings generated.
target thumb C: libpng <= external/libpng/pngread.c
external/libpng/pngread.c:1707:15: warning: explicitly assigning a variable of type 'int' to itself [-Wself-assign]
   transforms = transforms; /* Quiet compiler warnings */
   ~~~~~~~~~~ ^ ~~~~~~~~~~
external/libpng/pngread.c:1708:11: warning: explicitly assigning a variable of type 'voidp' (aka 'void *') to itself [-Wself-assign]
   params = params;
   ~~~~~~ ^ ~~~~~~
2 warnings generated.
target thumb C: libpng <= external/libpng/pngrio.c
target thumb C: libpng <= external/libpng/pngrtran.c
target thumb C: libpng <= external/libpng/pngrutil.c
external/libpng/pngrutil.c:695:13: warning: explicitly assigning a variable of type 'png_infop' (aka 'struct png_info_struct *') to itself [-Wself-assign]
   info_ptr = info_ptr; /* Quiet compiler warnings about unused info_ptr */
   ~~~~~~~~ ^ ~~~~~~~~
1 warning generated.
target thumb C: libpng <= external/libpng/pngset.c
external/libpng/pngset.c:1187:15: warning: explicitly assigning a variable of type 'png_uint_32' (aka 'unsigned long') to itself [-Wself-assign]
    asm_flags = asm_flags; /* Quiet the compiler */
    ~~~~~~~~~ ^ ~~~~~~~~~
external/libpng/pngset.c:1200:28: warning: explicitly assigning a variable of type 'png_byte' (aka 'unsigned char') to itself [-Wself-assign]
    mmx_bitdepth_threshold = mmx_bitdepth_threshold;
    ~~~~~~~~~~~~~~~~~~~~~~ ^ ~~~~~~~~~~~~~~~~~~~~~~
external/libpng/pngset.c:1201:28: warning: explicitly assigning a variable of type 'png_uint_32' (aka 'unsigned long') to itself [-Wself-assign]
    mmx_rowbytes_threshold = mmx_rowbytes_threshold;
    ~~~~~~~~~~~~~~~~~~~~~~ ^ ~~~~~~~~~~~~~~~~~~~~~~
3 warnings generated.
target thumb C: libpng <= external/libpng/pngtrans.c
target thumb C: libpng <= external/libpng/pngvcrd.c
target thumb C: libpng <= external/libpng/pngwio.c
target thumb C: libpng <= external/libpng/pngwrite.c
external/libpng/pngwrite.c:1589:15: warning: explicitly assigning a variable of type 'int' to itself [-Wself-assign]
   transforms = transforms; /* Quiet compiler warnings */
   ~~~~~~~~~~ ^ ~~~~~~~~~~
external/libpng/pngwrite.c:1590:11: warning: explicitly assigning a variable of type 'voidp' (aka 'void *') to itself [-Wself-assign]
   params = params;
   ~~~~~~ ^ ~~~~~~
2 warnings generated.
target thumb C: libpng <= external/libpng/pngwtran.c
target thumb C: libpng <= external/libpng/pngwutil.c
target StaticLib: libpng (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libpng_intermediates/libpng.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libsuspend_intermediates/import_includes
target thumb C: libsuspend <= system/core/libsuspend/autosuspend.c
target thumb C: libsuspend <= system/core/libsuspend/autosuspend_autosleep.c
target thumb C: libsuspend <= system/core/libsuspend/autosuspend_earlysuspend.c
target thumb C: libsuspend <= system/core/libsuspend/autosuspend_wakeup_count.c
target StaticLib: libsuspend (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libsuspend_intermediates/libsuspend.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libz_intermediates/import_includes
target asm: libz <= external/zlib/src/contrib/inflateneon/inflate_fast_copy_neon.s
target arm C: libz <= external/zlib/src/adler32.c
target arm C: libz <= external/zlib/src/compress.c
target arm C: libz <= external/zlib/src/crc32.c
target arm C: libz <= external/zlib/src/deflate.c
target arm C: libz <= external/zlib/src/gzclose.c
target arm C: libz <= external/zlib/src/gzlib.c
target arm C: libz <= external/zlib/src/gzread.c
target arm C: libz <= external/zlib/src/gzwrite.c
target arm C: libz <= external/zlib/src/infback.c
target arm C: libz <= external/zlib/src/inflate.c
target arm C: libz <= external/zlib/src/inftrees.c
target arm C: libz <= external/zlib/src/inffast.c
target arm C: libz <= external/zlib/src/trees.c
target arm C: libz <= external/zlib/src/uncompr.c
target arm C: libz <= external/zlib/src/zutil.c
target StaticLib: libz (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libz_intermediates/libz.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libstdc++_intermediates/import_includes
target thumb C++: libstdc++ <= bionic/libstdc++/src/one_time_construction.cpp
target thumb C++: libstdc++ <= bionic/libstdc++/src/new.cpp
target thumb C++: libstdc++ <= bionic/libstdc++/src/pure_virtual.cpp
target thumb C++: libstdc++ <= bionic/libstdc++/src/typeinfo.cpp
target StaticLib: libstdc++ (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libstdc++_intermediates/libstdc++.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_intermediates/import_includes
target arm C++: libc <= bionic/libc/bionic/pthread_create.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target arm C++: libc <= bionic/libc/bionic/pthread_key.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc <= bionic/libc/bionic/malloc_debug_common.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
target thumb C++: libc <= bionic/libc/bionic/libc_init_static.cpp
cc1plus: warning: command line option '-std=gnu99' is valid for C/ObjC but not for C++ [enabled by default]
bionic/libc/bionic/libc_init_static.cpp:86:17: warning: unused parameter 'onexit' [-Wunused-parameter]
target arm C: libc <= bionic/libc/bionic/pthread.c
target thumb C: libc <= bionic/libc/arch-arm/bionic/exidx_static.c
target thumb C: libc <= bionic/libc/bionic/dlmalloc.c
In file included from bionic/libc/bionic/dlmalloc.c:35:0:
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'init_bins':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:3929:5: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'prepend_alloc':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:3982:7: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:3982:7: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:3987:5: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'add_segment':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4042:5: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'dispose_chunk':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4401:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4401:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4435:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4435:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4446:5: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'tmalloc_large':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4516:11: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'tmalloc_small':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4554:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'dlmalloc':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4607:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4625:11: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4637:13: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'dlfree':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4741:17: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4741:17: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4777:15: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4777:15: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4789:13: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c: In function 'try_realloc_chunk':
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4891:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
bionic/libc/bionic/../upstream-dlmalloc/malloc.c:4891:9: warning: dereferencing type-punned pointer might break strict-aliasing rules [-Wstrict-aliasing]
preparing StaticLib: libc [including  /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_common_intermediates/libc_common.a]
target StaticLib: libc (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libc_intermediates/libc.a)
target StaticExecutable: charger (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/charger_intermediates/LINKED/charger)
target Symbolic: charger (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/charger)
Export includes file: system/core/charger/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/charger_intermediates/export_includes
target Strip: charger (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/charger_intermediates/charger)
Notice file: system/core/libpixelflinger/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libpixelflinger_static.a.txt
Notice file: external/libpng/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libpng.a.txt
Notice file: external/zlib/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libz.a.txt
Notice file: bionic/libstdc++/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libstdc++.a.txt
Notice file: bionic/libc/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libc.a.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/charger
Yacc: checkpolicy <= external/checkpolicy/policy_parse.y
prebuilts/misc/linux-x86/bison/bison -d -v -o /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.cpp external/checkpolicy/policy_parse.y
touch /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.hpp
echo '#ifndef 'policy_parse_h > /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.h
echo '#define 'policy_parse_h >> /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.h
cat /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.hpp >> /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.h
echo '#endif' >> /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.h
rm -f /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.hpp
Export includes file: external/libsepol/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libsepol_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/import_includes
host C: checkpolicy <= external/checkpolicy/queue.c
host C: checkpolicy <= external/checkpolicy/module_compiler.c
external/checkpolicy/module_compiler.c: In function 'add_perm_to_class':
external/checkpolicy/module_compiler.c:710:38: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
external/checkpolicy/module_compiler.c: In function 'is_scope_in_stack':
external/checkpolicy/module_compiler.c:1233:17: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
external/checkpolicy/module_compiler.c: In function 'end_optional':
external/checkpolicy/module_compiler.c:1448:22: warning: unused parameter 'pass' [-Wunused-parameter]
external/checkpolicy/module_compiler.c: In function 'copy_requirements':
external/checkpolicy/module_compiler.c:1511:11: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
external/checkpolicy/module_compiler.c:1517:17: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
host C: checkpolicy <= external/checkpolicy/parse_util.c
host C: checkpolicy <= external/checkpolicy/policy_define.c
external/checkpolicy/policy_define.c: In function 'define_dominance':
external/checkpolicy/policy_define.c:833:12: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
external/checkpolicy/policy_define.c: In function 'clone_level':
external/checkpolicy/policy_define.c:963:38: warning: unused parameter 'key' [-Wunused-parameter]
external/checkpolicy/policy_define.c: In function 'define_compute_type_helper':
external/checkpolicy/policy_define.c:1529:2: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
external/checkpolicy/policy_define.c: In function 'dominate_role_recheck':
external/checkpolicy/policy_define.c:2099:3: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
external/checkpolicy/policy_define.c:2105:3: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
external/checkpolicy/policy_define.c:2078:48: warning: unused parameter 'key' [-Wunused-parameter]
external/checkpolicy/policy_define.c: In function 'parse_semantic_categories':
external/checkpolicy/policy_define.c:3399:64: warning: unused parameter 'levdatum' [-Wunused-parameter]
host C: checkpolicy <= external/checkpolicy/checkpolicy.c
external/checkpolicy/checkpolicy.c: In function 'display_bools':
external/checkpolicy/checkpolicy.c:296:16: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
external/checkpolicy/checkpolicy.c: In function 'check_level':
external/checkpolicy/checkpolicy.c:364:72: warning: unused parameter 'arg' [-Wunused-parameter]
external/checkpolicy/checkpolicy.c: In function 'main':
external/checkpolicy/checkpolicy.c:472:20: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
host C++: checkpolicy <= /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_parse.cpp
cc1: warning: command line option '-Wsign-promo' is valid for C++/ObjC++ but not for C [enabled by default]
Lex: checkpolicy <= external/checkpolicy/policy_scan.l
host C++: checkpolicy <= /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/policy_scan.cpp
cc1: warning: command line option '-Wsign-promo' is valid for C++/ObjC++ but not for C [enabled by default]
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libsepol_intermediates/import_includes
host C: libsepol <= external/libsepol/src/assertion.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/avrule_block.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/avtab.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/boolean_record.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/booleans.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/conditional.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/constraint.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/context.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/context_record.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/debug.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/ebitmap.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/expand.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/genbools.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
external/libsepol/src/genbools.c: In function 'load_booleans':
external/libsepol/src/genbools.c:90:2: warning: implicit declaration of function 'getline' [-Wimplicit-function-declaration]
host C: libsepol <= external/libsepol/src/genusers.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
external/libsepol/src/genusers.c: In function 'load_users':
external/libsepol/src/genusers.c:74:2: warning: implicit declaration of function 'getline' [-Wimplicit-function-declaration]
host C: libsepol <= external/libsepol/src/handle.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/hashtab.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/hierarchy.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/iface_record.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/interfaces.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/link.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
external/libsepol/src/link.c: In function 'is_decl_requires_met':
external/libsepol/src/link.c:2024:8: warning: variable 'rc' set but not used [-Wunused-but-set-variable]
host C: libsepol <= external/libsepol/src/mls.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/module.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/node_record.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/nodes.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/polcaps.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/policydb.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/policydb_convert.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/policydb_public.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/port_record.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/ports.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/roles.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/services.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/sidtab.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/symtab.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/user_record.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/users.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/util.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host C: libsepol <= external/libsepol/src/write.c
In file included from <command-line>:0:0:
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:5: warning: "__GLIBC__" is not defined [-Wundef]
./build/core/combo/include/arch/linux-x86/AndroidConfig.h:337:23: warning: "__GLIBC__" is not defined [-Wundef]
host StaticLib: libsepol (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libsepol_intermediates/libsepol.a)
Export includes file: external/checkpolicy/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/export_includes
host Executable: checkpolicy (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkpolicy_intermediates/checkpolicy)
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkpolicy
/home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkpolicy:  loading policy configuration from /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/sepolicy_intermediates/policy.conf
/home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkpolicy:  policy configuration loaded
/home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkpolicy:  writing binary representation (version 26) to /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/sepolicy_intermediates/sepolicy
/home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkpolicy:  loading policy configuration from /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/sepolicy_intermediates/policy.conf.dontaudit
/home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkpolicy:  policy configuration loaded
/home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkpolicy:  writing binary representation (version 26) to /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/sepolicy_intermediates//sepolicy.dontaudit
Export includes file: external/libselinux/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libselinux_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkfc_intermediates/import_includes
host C: checkfc <= external/sepolicy/tools/checkfc.c
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libselinux_intermediates/import_includes
host C: libselinux <= external/libselinux/src/callbacks.c
host C: libselinux <= external/libselinux/src/check_context.c
host C: libselinux <= external/libselinux/src/freecon.c
host C: libselinux <= external/libselinux/src/init.c
host C: libselinux <= external/libselinux/src/label.c
host C: libselinux <= external/libselinux/src/label_file.c
host C: libselinux <= external/libselinux/src/label_android_property.c
host StaticLib: libselinux (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/STATIC_LIBRARIES/libselinux_intermediates/libselinux.a)
Export includes file: external/sepolicy/tools/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkfc_intermediates/export_includes
host Executable: checkfc (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkfc_intermediates/checkfc)
Notice file: external/libselinux/NOTICE -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/NOTICE_FILES/src//lib/libselinux.a.txt
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkfc
Notice file: external/sepolicy/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//root/file_contexts.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/file_contexts
Export includes file: system/core/fs_mgr/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libfs_mgr_intermediates/export_includes
Export includes file: system/core/logwrapper/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/liblogwrap_intermediates/export_includes
Export includes file: external/libselinux/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libselinux_intermediates/export_includes
Export includes file: system/core/libmincrypt/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libmincrypt_intermediates/export_includes
Export includes file: system/extras/ext4_utils/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libext4_utils_static_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/init_intermediates/import_includes
target thumb C: init <= system/core/init/builtins.c
system/core/init/builtins.c: In function 'do_exec':
system/core/init/builtins.c:269:34: warning: comparison between signed and unsigned integer expressions [-Wsign-compare]
system/core/init/builtins.c: In function 'do_setsebool':
system/core/init/builtins.c:927:12: warning: assignment discards 'const' qualifier from pointer target type [enabled by default]
target thumb C: init <= system/core/init/init.c
system/core/init/init.c: In function 'main':
system/core/init/init.c:1164:17: warning: assignment from incompatible pointer type [enabled by default]
target thumb C: init <= system/core/init/devices.c
target thumb C: init <= system/core/init/property_service.c
system/core/init/property_service.c: In function 'check_mac_perms':
system/core/init/property_service.c:188:5: warning: passing argument 5 of 'selinux_check_access' discards 'const' qualifier from pointer target type [enabled by default]
In file included from system/core/init/property_service.c:44:0:
/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/selinux/selinux.h:276:12: note: expected 'void *' but argument is of type 'const char *'
target thumb C: init <= system/core/init/util.c
system/core/init/util.c: In function 'create_socket':
system/core/init/util.c:94:9: warning: passing argument 1 of 'setsockcreatecon' discards 'const' qualifier from pointer target type [enabled by default]
In file included from /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/selinux/label.h:10:0,
                 from system/core/init/util.c:27:
/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/include/selinux/selinux.h:82:12: note: expected 'security_context_t' but argument is of type 'const char *'
target thumb C: init <= system/core/init/parser.c
target thumb C: init <= system/core/init/keychords.c
target thumb C: init <= system/core/init/signal_handler.c
target thumb C: init <= system/core/init/init_parser.c
target thumb C: init <= system/core/init/ueventd.c
target thumb C: init <= system/core/init/ueventd_parser.c
target thumb C: init <= system/core/init/watchdogd.c
target thumb C: init <= system/core/init/vendor_init.c
target thumb C: init <= system/core/init/logo.c
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libfs_mgr_intermediates/import_includes
target thumb C: libfs_mgr <= system/core/fs_mgr/fs_mgr.c
target thumb C: libfs_mgr <= system/core/fs_mgr/fs_mgr_verity.c
target StaticLib: libfs_mgr (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libfs_mgr_intermediates/libfs_mgr.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/liblogwrap_intermediates/import_includes
target thumb C: liblogwrap <= system/core/logwrapper/logwrap.c
target StaticLib: liblogwrap (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/liblogwrap_intermediates/liblogwrap.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libselinux_intermediates/import_includes
target thumb C: libselinux <= external/libselinux/src/booleans.c
target thumb C: libselinux <= external/libselinux/src/canonicalize_context.c
target thumb C: libselinux <= external/libselinux/src/disable.c
target thumb C: libselinux <= external/libselinux/src/enabled.c
target thumb C: libselinux <= external/libselinux/src/fgetfilecon.c
target thumb C: libselinux <= external/libselinux/src/fsetfilecon.c
target thumb C: libselinux <= external/libselinux/src/getenforce.c
target thumb C: libselinux <= external/libselinux/src/getfilecon.c
target thumb C: libselinux <= external/libselinux/src/getpeercon.c
target thumb C: libselinux <= external/libselinux/src/lgetfilecon.c
target thumb C: libselinux <= external/libselinux/src/load_policy.c
target thumb C: libselinux <= external/libselinux/src/lsetfilecon.c
target thumb C: libselinux <= external/libselinux/src/policyvers.c
target thumb C: libselinux <= external/libselinux/src/procattr.c
target thumb C: libselinux <= external/libselinux/src/setenforce.c
target thumb C: libselinux <= external/libselinux/src/setfilecon.c
target thumb C: libselinux <= external/libselinux/src/context.c
target thumb C: libselinux <= external/libselinux/src/mapping.c
target thumb C: libselinux <= external/libselinux/src/stringrep.c
target thumb C: libselinux <= external/libselinux/src/compute_create.c
target thumb C: libselinux <= external/libselinux/src/compute_av.c
target thumb C: libselinux <= external/libselinux/src/avc.c
target thumb C: libselinux <= external/libselinux/src/avc_internal.c
target thumb C: libselinux <= external/libselinux/src/avc_sidtab.c
target thumb C: libselinux <= external/libselinux/src/get_initial_context.c
target thumb C: libselinux <= external/libselinux/src/checkAccess.c
target thumb C: libselinux <= external/libselinux/src/sestatus.c
target thumb C: libselinux <= external/libselinux/src/deny_unknown.c
target thumb C: libselinux <= external/libselinux/src/callbacks.c
target thumb C: libselinux <= external/libselinux/src/check_context.c
target thumb C: libselinux <= external/libselinux/src/freecon.c
target thumb C: libselinux <= external/libselinux/src/init.c
target thumb C: libselinux <= external/libselinux/src/label.c
target thumb C: libselinux <= external/libselinux/src/label_file.c
target thumb C: libselinux <= external/libselinux/src/label_android_property.c
target thumb C: libselinux <= external/libselinux/src/android.c
target StaticLib: libselinux (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libselinux_intermediates/libselinux.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libmincrypt_intermediates/import_includes
target thumb C: libmincrypt <= system/core/libmincrypt/rsa.c
target thumb C: libmincrypt <= system/core/libmincrypt/sha.c
target thumb C: libmincrypt <= system/core/libmincrypt/sha256.c
target StaticLib: libmincrypt (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libmincrypt_intermediates/libmincrypt.a)
Export includes file: system/core/libsparse/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libsparse_static_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libext4_utils_static_intermediates/import_includes
target thumb C: libext4_utils_static <= system/extras/ext4_utils/make_ext4fs.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/ext4fixup.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/ext4_utils.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/allocate.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/contents.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/extent.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/indirect.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/uuid.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/sha1.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/wipe.c
target thumb C: libext4_utils_static <= system/extras/ext4_utils/crc16.c
target StaticLib: libext4_utils_static (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libext4_utils_static_intermediates/libext4_utils_static.a)
target StaticExecutable: init (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/init_intermediates/LINKED/init)
target Symbolic: init (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/init)
Export includes file: system/core/init/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/init_intermediates/export_includes
target Strip: init (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/init_intermediates/init)
Notice file: system/core/init/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//root/init.txt
Notice file: system/core/logwrapper/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/liblogwrap.a.txt
Notice file: external/libselinux/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libselinux.a.txt
Notice file: system/core/libmincrypt/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libmincrypt.a.txt
Notice file: system/extras/ext4_utils/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libext4_utils_static.a.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init
Generate: system/core/rootdir/init.environ.rc.in -> /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/init.environ.rc_intermediates/init.environ.rc
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.environ.rc
mkdir -p /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/sbin /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/dev /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/proc /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/sys /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/system /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/data
target Prebuilt: init.rc (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/init.rc_intermediates/init.rc)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.rc
Notice file: external/sepolicy/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//root/property_contexts.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/property_contexts
target Prebuilt: system_core_charger_battery_0.png (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/system_core_charger_battery_0.png_intermediates/battery_0.png)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/res/images/charger/battery_0.png
target Prebuilt: system_core_charger_battery_1.png (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/system_core_charger_battery_1.png_intermediates/battery_1.png)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/res/images/charger/battery_1.png
target Prebuilt: system_core_charger_battery_2.png (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/system_core_charger_battery_2.png_intermediates/battery_2.png)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/res/images/charger/battery_2.png
target Prebuilt: system_core_charger_battery_3.png (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/system_core_charger_battery_3.png_intermediates/battery_3.png)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/res/images/charger/battery_3.png
target Prebuilt: system_core_charger_battery_4.png (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/system_core_charger_battery_4.png_intermediates/battery_4.png)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/res/images/charger/battery_4.png
target Prebuilt: system_core_charger_battery_5.png (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/system_core_charger_battery_5.png_intermediates/battery_5.png)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/res/images/charger/battery_5.png
target Prebuilt: system_core_charger_battery_charge.png (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/system_core_charger_battery_charge.png_intermediates/battery_charge.png)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/res/images/charger/battery_charge.png
target Prebuilt: system_core_charger_battery_fail.png (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/system_core_charger_battery_fail.png_intermediates/battery_fail.png)
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/res/images/charger/battery_fail.png
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/adbd_intermediates/import_includes
target thumb C: adbd <= system/core/adb/adb.c
target thumb C: adbd <= system/core/adb/backup_service.c
target thumb C: adbd <= system/core/adb/fdevent.c
target thumb C: adbd <= system/core/adb/transport.c
target thumb C: adbd <= system/core/adb/transport_local.c
target thumb C: adbd <= system/core/adb/transport_usb.c
target thumb C: adbd <= system/core/adb/adb_auth_client.c
target thumb C: adbd <= system/core/adb/sockets.c
target thumb C: adbd <= system/core/adb/services.c
target thumb C: adbd <= system/core/adb/file_sync_service.c
target thumb C: adbd <= system/core/adb/jdwp_service.c
target thumb C: adbd <= system/core/adb/framebuffer_service.c
system/core/adb/framebuffer_service.c: In function 'framebuffer_service':
system/core/adb/framebuffer_service.c:175:5: warning: 'pid' may be used uninitialized in this function [-Wmaybe-uninitialized]
target thumb C: adbd <= system/core/adb/remount_service.c
target thumb C: adbd <= system/core/adb/usb_linux_client.c
target thumb C: adbd <= system/core/adb/log_service.c
target StaticExecutable: adbd (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/adbd_intermediates/LINKED/adbd)
target Symbolic: adbd (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/sbin/adbd)
Export includes file: system/core/adb/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/adbd_intermediates/export_includes
target Strip: adbd (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/adbd_intermediates/adbd)
Notice file: system/core/adb/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//root/sbin/adbd.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/sbin/adbd
Export includes file: frameworks/native/services/batteryservice/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbatteryservice_intermediates/export_includes
Export includes file: frameworks/native/libs/binder/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbinder_intermediates/export_includes
Export includes file: system/core/libutils/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libutils_intermediates/export_includes
Export includes file: system/core/healthd/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libhealthd.default_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/healthd_intermediates/import_includes
target thumb C++: healthd <= system/core/healthd/healthd.cpp
target thumb C++: healthd <= system/core/healthd/BatteryMonitor.cpp
system/core/healthd/BatteryMonitor.cpp: In member function 'int android::BatteryMonitor::getBatteryStatus(const char*)':
system/core/healthd/BatteryMonitor.cpp:63:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:63:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:63:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:63:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:63:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp: In member function 'int android::BatteryMonitor::getBatteryHealth(const char*)':
system/core/healthd/BatteryMonitor.cpp:85:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:85:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:85:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:85:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:85:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:85:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:85:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp: In member function 'android::BatteryMonitor::PowerSupplyType android::BatteryMonitor::readPowerSupplyType(const android::String8&)':
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp:138:5: warning: deprecated conversion from string constant to 'char*' [-Wwrite-strings]
system/core/healthd/BatteryMonitor.cpp: In member function 'bool android::BatteryMonitor::update()':
system/core/healthd/BatteryMonitor.cpp:315:62: warning: zero-length gnu_printf format string [-Wformat-zero-length]
target thumb C++: healthd <= system/core/healthd/BatteryPropertiesRegistrar.cpp
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbatteryservice_intermediates/import_includes
target thumb C++: libbatteryservice <= frameworks/native/services/batteryservice/BatteryProperties.cpp
target thumb C++: libbatteryservice <= frameworks/native/services/batteryservice/IBatteryPropertiesListener.cpp
target thumb C++: libbatteryservice <= frameworks/native/services/batteryservice/IBatteryPropertiesRegistrar.cpp
target StaticLib: libbatteryservice (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbatteryservice_intermediates/libbatteryservice.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbinder_intermediates/import_includes
target thumb C++: libbinder <= frameworks/native/libs/binder/AppOpsManager.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/Binder.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/BpBinder.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/BufferedTextOutput.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/Debug.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/IAppOpsCallback.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/IAppOpsService.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/IInterface.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/IMemory.cpp
frameworks/native/libs/binder/IMemory.cpp: In member function 'void android::BpMemoryHeap::assertReallyMapped() const':
frameworks/native/libs/binder/IMemory.cpp:303:9: warning: format '%ld' expects argument of type 'long int', but argument 6 has type 'ssize_t {aka int}' [-Wformat]
frameworks/native/libs/binder/IMemory.cpp:315:9: warning: format '%ld' expects argument of type 'long int', but argument 5 has type 'ssize_t {aka int}' [-Wformat]
frameworks/native/libs/binder/IMemory.cpp:337:17: warning: format '%ld' expects argument of type 'long int', but argument 5 has type 'ssize_t {aka int}' [-Wformat]
target thumb C++: libbinder <= frameworks/native/libs/binder/IPCThreadState.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/IPermissionController.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/IServiceManager.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/MemoryDealer.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/MemoryBase.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/MemoryHeapBase.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/Parcel.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/PermissionCache.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/ProcessState.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/Static.cpp
target thumb C++: libbinder <= frameworks/native/libs/binder/TextOutput.cpp
target StaticLib: libbinder (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libbinder_intermediates/libbinder.a)
Export includes file: system/core/libcorkscrew/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/SHARED_LIBRARIES/libcorkscrew_intermediates/export_includes
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libutils_intermediates/import_includes
target thumb C++: libutils <= system/core/libutils/BasicHashtable.cpp
target thumb C++: libutils <= system/core/libutils/BlobCache.cpp
target thumb C++: libutils <= system/core/libutils/CallStack.cpp
target thumb C++: libutils <= system/core/libutils/FileMap.cpp
target thumb C++: libutils <= system/core/libutils/JenkinsHash.cpp
target thumb C++: libutils <= system/core/libutils/LinearAllocator.cpp
target thumb C++: libutils <= system/core/libutils/LinearTransform.cpp
target thumb C++: libutils <= system/core/libutils/Log.cpp
target thumb C++: libutils <= system/core/libutils/Printer.cpp
target thumb C++: libutils <= system/core/libutils/ProcessCallStack.cpp
target thumb C++: libutils <= system/core/libutils/PropertyMap.cpp
target thumb C++: libutils <= system/core/libutils/RefBase.cpp
target thumb C++: libutils <= system/core/libutils/SharedBuffer.cpp
target thumb C++: libutils <= system/core/libutils/Static.cpp
target thumb C++: libutils <= system/core/libutils/StopWatch.cpp
target thumb C++: libutils <= system/core/libutils/String8.cpp
target thumb C++: libutils <= system/core/libutils/String16.cpp
target thumb C++: libutils <= system/core/libutils/SystemClock.cpp
target thumb C++: libutils <= system/core/libutils/Threads.cpp
target thumb C++: libutils <= system/core/libutils/Timers.cpp
target thumb C++: libutils <= system/core/libutils/Tokenizer.cpp
target thumb C++: libutils <= system/core/libutils/Unicode.cpp
target thumb C++: libutils <= system/core/libutils/VectorImpl.cpp
target thumb C++: libutils <= system/core/libutils/misc.cpp
target thumb C++: libutils <= system/core/libutils/Looper.cpp
target thumb C++: libutils <= system/core/libutils/Trace.cpp
target StaticLib: libutils (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libutils_intermediates/libutils.a)
Import includes file: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libhealthd.default_intermediates/import_includes
target thumb C++: libhealthd.default <= system/core/healthd/healthd_board_default.cpp
target StaticLib: libhealthd.default (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/STATIC_LIBRARIES/libhealthd.default_intermediates/libhealthd.default.a)
target StaticExecutable: healthd (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/healthd_intermediates/LINKED/healthd)
target Symbolic: healthd (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/symbols/sbin/healthd)
Export includes file: system/core/healthd/Android.mk -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/healthd_intermediates/export_includes
target Strip: healthd (/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/EXECUTABLES/healthd_intermediates/healthd)
Notice file: system/core/libutils/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//system/lib/libutils.a.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/sbin/healthd
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/sbin/ueventd -> ../init
Symlink: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/sbin/watchdogd -> ../init
Import includes file: /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkseapp_intermediates/import_includes
host C: checkseapp <= external/sepolicy/tools/check_seapp.c
Export includes file: external/sepolicy/tools/Android.mk -- /home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkseapp_intermediates/export_includes
host Executable: checkseapp (/home/hhp211/Source/AOSPA/out/host/linux-x86/obj/EXECUTABLES/checkseapp_intermediates/checkseapp)
Install: /home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkseapp
/home/hhp211/Source/AOSPA/out/host/linux-x86/bin/checkseapp -p /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/sepolicy_intermediates/sepolicy -o /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/seapp_contexts_intermediates/seapp_contexts /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/ETC/seapp_contexts_intermediates/seapp_contexts.tmp
Notice file: external/sepolicy/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//root/seapp_contexts.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/seapp_contexts
Notice file: external/sepolicy/NOTICE -- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/obj/NOTICE_FILES/src//root/sepolicy.txt
Install: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/sepolicy
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.pa.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.aries.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.aries.usb.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.recovery.aries.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/lpm.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/ueventd.aries.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/fstab.aries
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/sbin/setupdatadata.sh
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.usb.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.trace.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/ueventd.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/fstab.goldfish
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/init.goldfish.rc
Copy: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/ueventd.goldfish.rc
Target buildinfo: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/default.prop
build/tools/post_process_props.py /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/root/default.prop
Target ram disk: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/ramdisk.img
make: Circular /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img <- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/kernel dependency dropped.
make: Circular /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img <- /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/kernel dependency dropped.
Boot image: /home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img
acp: file '/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/kernel' does not exist
make: *** [/home/hhp211/Source/AOSPA/out/target/product/fascinatemtd/boot.img] Error 1
hhp211@hhp211-Q500A:~/Source/AOSPA$ 




