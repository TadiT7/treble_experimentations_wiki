Missing hardware support:
- fingerprint gestures (WIP at https://github.com/phhusson/treble_experimentations/tree/master/vendor-HAL/Huawei/fingerprint-nav )

Known work-arounds:
- Full-screen composer: https://github.com/phhusson/platform_frameworks_native/commit/632d84faa78ab02286d7663efdd325d374a9d9ba
- Partial screen damage
https://github.com/phhusson/platform_frameworks_native/commit/cdc0f4b5e81347a39af157472f2f21f84652eade
- WiFi property permission fail: https://github.com/phhusson/platform_frameworks_opt_net_wifi/commit/7d627793de0986b233d67cc412224b8f84ff5820

Kwown bugs:
- In some cases (TBD), the user needs to hotplug SIM card for it to be detected
