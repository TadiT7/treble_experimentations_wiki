Device supported.

Known work-arounds:
- Full-screen composer: https://github.com/phhusson/platform_frameworks_native/commit/632d84faa78ab02286d7663efdd325d374a9d9ba
- Partial screen damage
https://github.com/phhusson/platform_frameworks_native/commit/cdc0f4b5e81347a39af157472f2f21f84652eade
- WiFi property permission fail: https://github.com/phhusson/platform_frameworks_opt_net_wifi/commit/7d627793de0986b233d67cc412224b8f84ff5820

Kwown bugs:
- In some cases (TBD), the user needs to hotplug SIM card for it to be detected
- In some cases, the device no longer wants to register touchscreen events when learning. This is probably linked to some factory reset issues.

Additional infos:
- Ported stock Camera exists and mostly work, keeping original quality.