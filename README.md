# BluBoard
<img width="4000"  alt="banner_ortho" src="https://github.com/user-attachments/assets/4edf628e-e06e-4548-ae24-e67ef5867d3c" />

An nRF52840 dev board made to be embedded in a custom mechanical keyboard, with as many pins broken out as possible within JLCPCB's 6-layer specs.

---

## What is this?

BluBoard is a custom nRF52840 development board built for use inside a mechanical keyboard. The main goal was to break out as many GPIO pins as possible and also having proper RF capabilities 
most off-the-shelf options such as the nice nano is powerful, but comes at high cost while having low gpio count, this board tries to fix that.

---

## Form Factor

Slightly wider than a Raspberry Pi Pico. Uses two 1×20 pin headers, plus an extra two 1×3 headers near the usb c port for the pins that didn't fit in the main rows.

---

## Features

- **nRF52840** - ARM Cortex-M4F, BLE 5.x, 1MB flash, 256KB RAM
- **USB-C** - power and programming
- **BLE 5.x** - wireless support built in with trace antenna
- **SWD debug header** - for debugging
- **I2C** - broken out, available on most pins
- **SPI** - broken out, available on most pins
- **Analog IO** - most analog pins are broken out, on top or bottom layer with 1oz copper for signal
- **6-layer PCB** - JLCPCB, ENIG finish, filled via for bga
- **Built-in power management** - built in battery support through a jst-ph connector and a BQ24075 charger

---

## Pin Breakout

Power, ground, and GPIO are spread across both 1×20 headers. The extra 1×3 headers cover the remaining pins and utils such as swd.

> Full pinout table coming soon. Check the KiCad schematic in the meantime.

---

## Firmware

BluBoard targets **ZMK**, which has native nRF52840 support and works well for wireless keyboards. Bare metal / Nordic SDK also works if you need it.

> A ZMK shield definition for BluBoard is planned but not yet published.

---


## Why 6 layers?

Jlc's manufacturing options allow for cheap manufacturing of 6 layer boards, in addition, at this form factor, their 6 layer boards are cheaper than 4 layer, while having additional benefits such as enig finish, and free filled vias, so the bga solder points would not be a possible point of failure

---

## Previews
### Schematic
<img height="400" alt="image" src="https://github.com/user-attachments/assets/fc130243-2a68-4db1-ad74-be2882d0b153" />
(don't ask why I did this)
<img height="400" alt="image" src="https://github.com/user-attachments/assets/28c11495-975c-43df-9145-3f52e2b11357" />
<img height="400" alt="image" src="https://github.com/user-attachments/assets/71a4bddb-1bb6-42f5-b67d-dbab579974e1" />

### PCB
#### All
<img  height="500" alt="image" src="https://github.com/user-attachments/assets/cbc17d5e-c328-4029-82be-97fc1f120efe" />

#### Top
<img  height="500" alt="image" src="https://github.com/user-attachments/assets/da4d63dd-15dc-42e0-924c-e3226f625f2f" />

#### In.1
<img  height="500" alt="image" src="https://github.com/user-attachments/assets/6fdb387f-a714-41b6-8aa4-95c5673544ce" />

#### In.2
<img height="500" alt="image" src="https://github.com/user-attachments/assets/30f1cdf0-5c34-4351-8ad3-dbfbf3456402" />

#### In.3
<img  height="500" alt="image" src="https://github.com/user-attachments/assets/ff1f8615-0019-4e97-8eb0-425bd015c601" />

#### In.4
<img  height="500" alt="image" src="https://github.com/user-attachments/assets/ed933824-499e-4a4b-beb3-40059bb41315" />

#### Bottom
<img  height="500" alt="image" src="https://github.com/user-attachments/assets/e71ac7fd-2540-40a9-aa3f-80305a2c9dd0" />





*Built with KiCad 9 and 10 · Fabricated via JLCPCB · Part of Hack Club [Blueprint](blueprint.hackclub.com) and [Stasis](stasis.hackclub.com)*
