# Peripheral Details

---

## QSPI Flash

- Interface: QUADSPI (Bank 1)
- Type: NOR Flash
- Density: 128 Mb (16M x 8)
- Protocol support: SPI / Quad I/O / QPI / DTR
- Max clock: 133 MHz
- Package: 8-SOIC
---

## SDRAM

- Interface: FMC (Bank 5 / SDRAM Bank 1)
- Density: 256 Mb (16M x 16), equivalent to 32 MB
- Type: SDR SDRAM (parallel)
- Max clock: 166 MHz (5 ns)
- Package: 54-TSOP II

---

## TF Card

- Interface: SDMMC1 (4-bit)
- Card detect pin: not present on this board
- Connector: Micro SD card socket (push-push)


---

## EEPROM

- Interface: I2C (likely I2C4 mapped to PH4/PH5)
- Device class: 24C02 serial EEPROM (2 Kbit)
- Top marking observed: `ATMLH518 02CM TH 2518KM3`
- Datasheet: not identified yet


---

## USB

- Mode: USB Full Speed (Device or OTG)
- Connector: USB-C

---

## COM Ports

- **USART1** (PA9/PA10) is routed to a USB-to-UART bridge (CH340G)
- Connector type for this serial port: USB-C
- Field note: the USB-UART path was pulling MCU `NRST` low when a serial monitor connected; after removing the diode in that reset coupling path, behavior normalized



---

## LEDs

Two active-low LEDs controlled via GPIO output.

- **LED0 (PB0):** red, active low
- **LED1 (PB1):** green, active low
- **PWR LED:** red, tied to power rail (always on when powered)



---

## Keys / Buttons

- **WK_UP (PA0):** active high, can be used as wake-up source from low-power modes
- **KEY0 (PA1):** active high
- **RESET button:** active low, with a capacitor in parallel


---

## LCD1 — RGB Interface <a id="lcd1-rgb"></a>

- Interface: RGB parallel (likely 16-bit or 24-bit)
- Status: still pending detailed characterization; pin-level mapping and exact panel standard need to be documented.

---

## LCD2 — SPI Interface <a id="lcd2-spi"></a>

- Interface: SPI
- Status: still pending detailed characterization; pin-level mapping and exact panel standard need to be documented.

---

## Camera (DVP) <a id="camera"></a>

- Interface: DCMI (parallel digital camera interface)
- Status: still pending detailed characterization; sensor standard and full pin mapping need to be documented.

---

## GPIO Expansion Header

A header breaks out additional GPIO pins for user expansion. Exact pins to be documented.

---

## SWD

Standard 4-pin SWD debug interface:

| Pin | Signal |
|-----|--------|
| 1 | VCC (3.3V) |
| 2 | SWDIO (PA13) |
| 3 | SWCLK (PA14) |
| 4 | GND |

Compatible with ST-Link V2, J-Link, and similar debuggers.

---

## Power

- Input voltage: not confirmed — likely 5V via USB or header
- On-board 3.3V regulator for MCU and peripherals
- Check board for LDO marking (e.g. AMS1117-3.3)

