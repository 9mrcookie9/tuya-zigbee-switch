# Supported devices

Support new devices: [contribute/porting.md](/docs/contribute/porting.md)  

### Quick-picks
- **modules:** AVATTO, Aubess, iHseno
- **switches:** Moes 1-3gang (any design, except Star Feather)

### Careful with
- generic 1-gang modules - might not support OTA conversion
- BSEED switches - too many variants (can't know which you'll receive)

### Legend

| Symbol | Meaning  |                    |                     |                |                |           |          |
| :----: | -------- | ------------------ | ------------------- | -------------- | -------------- | --------- | -------- |
|   🚧️   | Status   | 🟩️ Fully supported | 🟨️ Mostly supported | 🟧️ In progress | 🟥️ Unsupported |           |          |
|   📦️   | Build    | ✔️ Available       | ❌️ Unavailable      |                |                |           |          |
|   💡️   | Category | 🇲️ Module          | 🇸️ Switch           | 🇴️ Outlet      | 🇵 Plug        | 🇷️ Remote | 🇧️ Board | 
|   ⚡️   | Power    | 🔌️ Mains           | 🔋️ Battery          | 🔱️ USB         |                |           |          |
|   📲️   | Install  | 🛜️ Wireless        | ➿️ By wire          | ❓️ Unknown     |                |           |          |
|   🏭️   | MCU      | `TL` Telink        | `SL` Silicon Labs   | `NXP` NXP      |                |           |          |
|   🅰   | Variant  | 🅰                  | 🅱                  | 🅲             | 🅳              | 🅴        | 🅵        |

<!-------------------------------------------------------------------
  `supported.md` is generated. 
  
  Do not edit it directly! Instead, edit:
  - `device_db.yaml`             - add or edit devices
  - `supported_devices.md.jinja` - update the template
  - `make_supported_devices.py`  - update generation script

  Generate with: `make tools/update_supported_devices`
-------------------------------------------------------------------->

> [!IMPORTANT]  
> Identify your device by **Zigbee Manufacturer** and linked threads/stores!  
> *Z2M pages are sometimes generic.*

### Device list

| 🚧 | 📦 | 💡 | ⚡️ | 📲 |  🏭  | Zb&nbsp;Manufacturer <br> Zb&nbsp;Model | Name <br> Z2M&nbsp;page&nbsp;🔗 | Store | Threads | Status |
| -- | -- | -- | -- | -- | :--: | :-------------------------------------- | :------------------------------ | ----: | ------: | :----- |
| 🟧 | ✔️ | 🇲 | 🔌 | 🛜 | **TL** | `_TZ3210_aksyshpw` <br> `TS0003` | [Tuya common 3-gang](https://www.zigbee2mqtt.io/devices/TS0003_switch_module_1.html) |   |   | Supported | 
| 🟩 | ✔️ | 🇸 | 🔌 | ➿ | **SL** | `_TZ3000_mrduubod` <br> `TS0014` | [Moes 4-gang switches (all variants)](https://www.zigbee2mqtt.io/devices/TS0014.html) | [`Moes`](https://moeshouse.com/collections/light-switch?gf_59186=ZigBee) [`Moes`](https://moeshouse.com/collections/eu-star-ring) [`AlEx`](https://www.aliexpress.com/item/1005005178075186.html) [`AlEx`](https://www.aliexpress.com/item/1005005178430448.html) | [`#014`](https://github.com/romasku/tuya-zigbee-switch/issues/14) | Supported | 
| 🟧 | ✔️ | 🇸 | 🔌 | 🛜 | **TL** | `_TZ3000_cmgs1zkr` <br> `TS0002` | [PSMART T442/T452 TL](https://www.zigbee2mqtt.io/devices/TS0002.html) | [`Store`](https://psmart.pl/pl/p/PSMART-Przelacznik-2-obwody-C-RM-ZigBee-TUYA/2052) | [`#252`](https://github.com/romasku/tuya-zigbee-switch/issues/252) | Needs pinout | 
| 🟨 | ✔️ | 🇸 | 🔌 | ➿ | **SL** | `_TZ3000_myaaknbq` <br> `TS0001` | [PSMART T441/T451 SL](https://www.zigbee2mqtt.io/devices/T441.html) | [`Store`](https://psmart.pl/pl/p/PSMART-Przelacznik-1-obwod-C-RM-ZigBee-TUYA/2053) | [`#252`](https://github.com/romasku/tuya-zigbee-switch/issues/252) | Backlight on A5. If relay is not used, see alt_config. | 
| 🟨 | ✔️ | 🇸 | 🔌 | ➿ | **SL** | `_TZ3000_mufwv0ry` <br> `TS0002` | [PSMART T442/T452 SL](https://www.zigbee2mqtt.io/devices/T442.html) | [`Store`](https://psmart.pl/pl/p/PSMART-Przelacznik-2-obwody-C-RM-ZigBee-TUYA/2052) | [`#252`](https://github.com/romasku/tuya-zigbee-switch/issues/252) | Backlight on A5 (3rd relay with alt_config) | 
| 🟨 | ✔️ | 🇸 | 🔌 | ➿ | **SL** | `_TZ3000_lsunm46z` <br> `TS0003` | [PSMART T443/T453 SL](https://www.zigbee2mqtt.io/devices/ZM-L03E-Z.html) | [`Store`](https://psmart.pl/pl/p/PSMART-Przelacznik-3-obwody-C-RM-ZigBee-TUYA/2051) | [`#252`](https://github.com/romasku/tuya-zigbee-switch/issues/252) | Backlight on A5 | 

Data from [`device_db.yaml`](/device_db.yaml)
