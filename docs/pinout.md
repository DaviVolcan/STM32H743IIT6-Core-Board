# Pin Assignments

Extracted from schematic V1.3. Verify against your board before use.

---

## TF Card (SDMMC1)

| Signal | MCU Pin |
|--------|---------|
| SDMMC1_D0 | PC8 |
| SDMMC1_D1 | PC9 |
| SDMMC1_D2 | PC10 |
| SDMMC1_D3 | PC11 |
| SDMMC1_CK | PC12 |
| SDMMC1_CMD | PD2 |

---

## QSPI Flash

| Signal | MCU Pin |
|--------|---------|
| QUADSPI_IO0 | PF8 |
| QUADSPI_IO1 | PF9 |
| QUADSPI_IO2 | PF7 |
| QUADSPI_IO3 | PF6 |
| QUADSPI_CLK | PF10 |
| QUADSPI_NCS | PB6 |

---

## SDRAM (FMC)

| Signal     | MCU Pin |
|------------|---------|
| FMC_D0     | PD14    |
| FMC_D1     | PD15    |
| FMC_D2     | PD0     |
| FMC_D3     | PD1     |
| FMC_D4     | PE7     |
| FMC_D5     | PE8     |
| FMC_D6     | PE9     |
| FMC_D7     | PE10    |
| FMC_D8     | PE11    |
| FMC_D9     | PE12    |
| FMC_D10    | PE13    |
| FMC_D11    | PE14    |
| FMC_D12    | PE15    |
| FMC_D13    | PD8     |
| FMC_D14    | PD9     |
| FMC_D15    | PD10    |
| FMC_A0     | PF0     |
| FMC_A1     | PF1     |
| FMC_A2     | PF2     |
| FMC_A3     | PF3     |
| FMC_A4     | PF4     |
| FMC_A5     | PF5     |
| FMC_A6     | PF12    |
| FMC_A7     | PF13    |
| FMC_A8     | PF14    |
| FMC_A9     | PF15    |
| FMC_A10    | PG0     |
| FMC_A11    | PG1     |
| FMC_A12    | PG2     |
| FMC_NBL0   | PE0     |
| FMC_NBL1   | PE1     |
| FMC_SDCLK  | PG8     |
| FMC_SDNWE  | PC0     |
| FMC_SDNRAS | PF11    |
| FMC_SDNCAS | PG15    |
| FMC_SDNE0  | PH3     |
| FMC_SDCKE0 | PH2     |
| FMC_SDCKE0 | PH2     |
| FMC_BS0    | PG4     |
| FMC_BS1    | PG5     |

---

## EEPROM (I2C)

| Signal | MCU Pin |
|--------|---------|
| I2C_SCL | PH4 |
| I2C_SDA | PH5 |


---

## USB (Full Speed)

| Signal | MCU Pin |
|--------|---------|
| USB_D+ | PA12 |
| USB_D- | PA11 |

---

## USART / COM Ports

| Signal | MCU Pin |
|--------|---------|
| USART1_TX | PA9 |
| USART1_RX | PA10 |
| USART2_TX | PA2 |
| USART2_RX | PA3 |

---

## LEDs

| Label | MCU Pin | Active |
|-------|---------|--------|
| LED0 | PB0     | Low |
| LED1 | PB1     | Low |

---

## Keys / Buttons

| Label | MCU Pin | Active |
|-------|---------|--------|
| WK_UP | PA0 | High |
| KEY0 | PE4 | Low |

---

## SWD Debug

| Signal | MCU Pin |
|--------|---------|
| SWDIO | PA13 |
| SWCLK | PA14 |

---

## Camera (DVP)

Parallel camera interface. Exact pin mapping to be confirmed — see [peripherals.md](peripherals.md#camera).

---

## LCD1 — RGB Interface

RGB parallel display + touch panel header. Exact pin mapping to be confirmed — see [peripherals.md](peripherals.md#lcd1-rgb).

---

## LCD2 — SPI Interface

SPI display + touch panel header. Exact pin mapping to be confirmed — see [peripherals.md](peripherals.md#lcd2-spi).
