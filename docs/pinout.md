# Pin Assignments

Extracted from schematic V1.3. Verify against your board before use.

---

## TF Card (SDMMC1)

| Signal     | MCU Pin |
|------------|---------|
| SDMMC1_D0  | PC8     |
| SDMMC1_D1  | PC9     |
| SDMMC1_D2  | PC10    |
| SDMMC1_D3  | PC11    |
| SDMMC1_CK  | PC12    |
| SDMMC1_CMD | PD2     |

---

## QSPI Flash

| Signal      | MCU Pin |
|-------------|---------|
| QUADSPI_IO0 | PF8     |
| QUADSPI_IO1 | PF9     |
| QUADSPI_IO2 | PF7     |
| QUADSPI_IO3 | PF6     |
| QUADSPI_CLK | PF10    |
| QUADSPI_NCS | PB6     |

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
| FMC_A14    | PG4     |
| FMC_A15    | PG5     |

---

## EEPROM (I2C)

| Signal  | MCU Pin |
|---------|---------|
| I2C_SCL | PH4     |
| I2C_SDA | PH5     |

---

## USB (Full Speed)

| Signal | MCU Pin |
|--------|---------|
| USB_D+ | PA12    |
| USB_D- | PA11    |

---

## USART / COM Ports

| Signal    | MCU Pin |
|-----------|---------|
| USART1_TX | PA9     |
| USART1_RX | PA10    |

---

## LEDs

| Label | MCU Pin | Active |
|-------|---------|--------|
| LED0  | PB0     | Low    |
| LED1  | PB1     | Low    |

---

## Keys / Buttons

| Label | MCU Pin | Active |
|-------|---------|--------|
| WK_UP | PA0     | High   |
| KEY0  | PE4     | Low    |

---

## SWD Debug

| Signal | MCU Pin |
|--------|---------|
| SWDIO  | PA13    |
| SWCLK  | PA14    |

---

## Header P1 (50 pins)

> Pins marked ⚠️ are shared with on-board peripherals — check before use.

| Pin | MCU Pin | Capabilities |
|-----|---------|-------------|
| 1   | 3.3V    | Power supply |
| 2   | GND     | Ground |
| 3   | 3.3V    | Power supply |
| 4   | GND     | Ground |
| 5   | VREF+   | ADC/DAC voltage reference |
| 6   | NRST    | System reset |
| 7   | PC1     | SPI2_MOSI/I2S2, SAI1/4, SDMMC2_CK, ETH_MDC, MDIOS_MDC — ADC123 |
| 8   | PC2     | SPI2_MISO/I2S2, DFSDM1, OTG_HS_ULPI_DIR, ETH_TXD2, FMC_SDNE0 — ADC123 |
| 9   | PC3     | SPI2_MOSI/I2S2, DFSDM1, OTG_HS_ULPI_NXT, ETH_TX_CLK, FMC_SDCKE0 — ADC12 |
| 10  | PF10    | TIM16_BKIN, SAI1/4_D3, QUADSPI_CLK, DCMI_D11, LCD_DE — ADC3 |
| 11  | PA0     | TIM2_CH1/ETR, TIM5_CH1, TIM8_ETR, TIM15_BKIN, USART2_CTS, UART4_TX, SDMMC2_CMD, SAI2_SD_B, ETH_CRS — ADC1_INP16, WKUP1 |
| 12  | PA1     | TIM2_CH2, TIM5_CH2, LPTIM3, TIM15_CH1N, USART2_RTS, UART4_RX, QUADSPI_BK1_IO3, SAI2_MCLK_B, ETH_RX_CLK, LCD_R2 — ADC1 |
| 13  | PA2     | TIM2_CH3, TIM5_CH3, LPTIM4, TIM15_CH1, USART2_TX, SAI2_SCK_B, ETH_MDIO, MDIOS_MDIO, LCD_R1 — ADC12, WKUP2 |
| 14  | PH4     | I2C2_SCL, LCD_G5/G4, OTG_HS_ULPI_NXT — ADC3 ⚠️ EEPROM SCL |
| 15  | PH5     | I2C2_SDA, SPI5_NSS, FMC_SDNWE — ADC3 ⚠️ EEPROM SDA |
| 16  | PA3     | TIM2_CH4, TIM5_CH4, LPTIM5, TIM15_CH2, USART2_RX, OTG_HS_ULPI_D0, ETH_COL, LCD_B2/B5 — ADC12 |
| 17  | GND     | Ground |
| 18  | PA5     | TIM2_CH1/ETR, TIM8_CH1N, SPI1_SCK/I2S1_CK, SPI6_SCK, OTG_HS_ULPI_CK, LCD_R4 — ADC12, DAC1_OUT2 |
| 19  | GND     | Ground |
| 20  | PA7     | TIM1_CH1N, TIM3_CH2, TIM8_CH1N, SPI1_MOSI/I2S1, SPI6_MOSI, TIM14_CH1, ETH_RX_DV/RMII_CRS_DV, FMC_SDNWE — ADC12, OPAMP1_VINM |
| 21  | PC4     | DFSDM1_CKIN2, I2S1_MCK, SPDIFRX_IN3, ETH_RXD0/RMII_RXD0, FMC_SDNE0 — ADC12, OPAMP1_VOUT, COMP1_INM |
| 22  | PC5     | SAI1/4_D3, DFSDM1_DATIN2, SPDIFRX_IN4, ETH_RXD1/RMII_RXD1, FMC_SDCKE0, COMP1_OUT — ADC12, OPAMP1_VINM |
| 23  | PB0     | TIM1_CH2N, TIM3_CH3, TIM8_CH2N, DFSDM1, UART4_CTS, OTG_HS_ULPI_D1, ETH_RXD2, LCD_R3/G1 — ADC12, OPAMP1_VINP, COMP1_INP ⚠️ LED0 |
| 24  | PB1     | TIM1_CH3N, TIM3_CH4, TIM8_CH3N, DFSDM1, OTG_HS_ULPI_D2, ETH_RXD3, LCD_R6/G0 — ADC12, COMP1_INM ⚠️ LED1 |
| 25  | PB10    | TIM2_CH3, HRTIM_SCOUT, LPTIM2_IN1, I2C2_SCL, SPI2_SCK/I2S2, DFSDM1, USART3_TX, QUADSPI_BK1_NCS, OTG_HS_ULPI_D3, ETH_RX_ER, LCD_G4 ⚠️ DCMI_SDA |
| 26  | PB11    | TIM2_CH4, HRTIM_SCIN, LPTIM2_ETR, I2C2_SDA, DFSDM1, USART3_RX, OTG_HS_ULPI_D4, ETH_TX_EN/RMII_TX_EN, LCD_G5 |
| 27  | PH6     | TIM12_CH1, I2C2_SMBA, SPI5_SCK, ETH_RXD2, FMC_SDNE1, DCMI_D8 |
| 28  | PH7     | I2C3_SCL, SPI5_MISO, ETH_RXD3, FMC_SDCKE1, DCMI_D9 |
| 29  | PH8     | TIM5_ETR, I2C3_SDA, FMC_D16, DCMI_HSYNC, LCD_R2 |
| 30  | PH9     | TIM12_CH2, I2C3_SMBA, FMC_D17, DCMI_D0, LCD_R3 |
| 31  | PH10    | TIM5_CH1, I2C4_SMBA, FMC_D18, DCMI_D1, LCD_R4 |
| 32  | PH11    | TIM5_CH2, I2C4_SCL, FMC_D19, DCMI_D2, LCD_R5 |
| 33  | PH12    | TIM5_CH3, I2C4_SDA, FMC_D20, DCMI_D3, LCD_R6 |
| 34  | PB12    | TIM1_BKIN, I2C2_SMBA, SPI2_NSS/I2S2_WS, DFSDM1, USART3_CK, FDCAN2_RX, OTG_HS_ULPI_D5, ETH_TXD0/RMII_TXD0, OTG_HS_ID, UART5_RX |
| 35  | PB13    | TIM1_CH1N, LPTIM2_OUT, SPI2_SCK/I2S2, DFSDM1, USART3_CTS, FDCAN2_TX, OTG_HS_ULPI_D6, ETH_TXD1/RMII_TXD1, UART5_TX |
| 36  | PB14    | TIM1_CH2N, TIM12_CH1, TIM8_CH2N, USART1_TX, SPI2_MISO/I2S2, DFSDM1, USART3_RTS, UART4_RTS, SDMMC2_D0, OTG_HS_DM |
| 37  | PB15    | TIM1_CH3N, TIM12_CH2, TIM8_CH3N, USART1_RX, SPI2_MOSI/I2S2, DFSDM1, UART4_CTS, SDMMC2_D1, OTG_HS_DP |
| 38  | PD11    | LPTIM2_IN2, I2C4_SMBA, USART3_CTS, QUADSPI_BK1_IO0, SAI2_SD_A, FMC_A16 |
| 39  | PD12    | LPTIM1/2_IN1, TIM4_CH1, I2C4_SCL, USART3_RTS, QUADSPI_BK1_IO1, SAI2_FS_A, FMC_A17 |
| 40  | PD13    | LPTIM1_OUT, TIM4_CH2, I2C4_SDA, QUADSPI_BK1_IO3, SAI2_SCK_A, FMC_A18 |
| 41  | PG3     | TIM8_BKIN2, FMC_A13 ⚠️ DCMI_SCL |
| 42  | PG6     | TIM17_BKIN, HRTIM_CHE1, QUADSPI_BK1_NCS, FMC_NE3, DCMI_D12, LCD_R7 |
| 43  | GND     | Ground |
| 44  | PC6     | HRTIM_CHA1, TIM3_CH1, TIM8_CH1, I2S2_MCK, USART6_TX, SDMMC2_D6, FMC_NWAIT, SDMMC1_D6, DCMI_D0, LCD_HSYNC, SWPMI_IO ⚠️ SDMMC1_D6 |
| 45  | PC7     | HRTIM_CHA2, TIM3_CH2, TIM8_CH2, I2S3_MCK, USART6_RX, SDMMC2_D7, FMC_NE1, SDMMC1_D7, DCMI_D1, LCD_G6, SWPMI_TX ⚠️ SDMMC1_D7 |
| 46  | PC8     | TIM3_CH3, TIM8_CH3, USART6_CK, UART5_RTS, FMC_NE2, SWPMI_RX, SDMMC1_D0, DCMI_D2 ⚠️ SDMMC1_D0 |
| 47  | PC9     | MCO2, TIM3_CH4, TIM8_CH4, I2C3_SDA, UART5_CTS, QUADSPI_BK1_IO0, LCD_G3, SDMMC1_D1, DCMI_D3, LCD_B2 ⚠️ SDMMC1_D1 |
| 48  | PA8     | MCO1, TIM1_CH1, HRTIM_CHB2, TIM8_BKIN2, I2C3_SCL, USART1_CK, OTG_FS_SOF, UART7_RX, LCD_B3/R6 |
| 49  | PA13    | JTMS/SWDIO ⚠️ SWD debug |
| 50  | PH13    | TIM8_CH1N, UART4_TX, FDCAN1_TX, FMC_D21, LCD_G2 |

---


## Header P2 (50 pins)

> Pins marked ⚠️ are shared with on-board peripherals — check before use.

| Pin | MCU Pin | Capabilities |
|-----|---------|-------------|
| 1   | GND     | Ground |
| 2   | VCC5    | 5 V power supply |
| 3   | GND     | Ground |
| 4   | VCC5    | 5 V power supply |
| 5   | VBAT    | Battery / RTC power input |
| 6   | BOOT0   | Boot mode selection |
| 7   | PI11    | OTG_HS_ULPI_DIR, WKUP5 |
| 8   | PI10    | ETH_MII_RX_ER, FMC_D31, LCD_HSYNC |
| 9   | PI9     | UART4_RX, FDCAN1_RX, FMC_D30, LCD_VSYNC |
| 10  | PC13    | RTC_OUT/TAMP1/TS, WKUP4 |
| 11  | PI8     | RTC_TAMP2, WKUP3 |
| 12  | PE6     | TIM1_BKIN2, SAI1/4_D1, TIM15_CH2, SPI4_MOSI, SAI1_SD_A, SAI2_MCL_B, FMC_A22, DCMI_D7, LCD_G1 |
| 13  | PE5     | SAI1_CK2, DFSDM1_CKIN3, TIM15_CH1, SPI4_MISO, SAI1/4_SCK_A, FMC_A21, DCMI_D6, LCD_G0 |
| 14  | PE4     | SAI1_D2, DFSDM1_DATIN3, TIM15_CH1N, SPI4_NSS, SAI1/4_FS_A, FMC_A20, DCMI_D4, LCD_B0 ⚠️ KEY0 |
| 15  | PE3     | TRACED0, SAI1_SD_B, FMC_A19 |
| 16  | PE2     | TRACECLK, SAI1_CK1, SPI4_SCK, SAI1/4_MCLK_A, QUADSPI_BK1_IO2, ETH_TXD3, FMC_A23 |
| 17  | PI7     | TIM8_CH3, SAI2_FS_A, FMC_D29, DCMI_D7, LCD_B7 |
| 18  | PI6     | TIM8_CH2, SAI2_SD_A, FMC_D28, DCMI_D6, LCD_B6 |
| 19  | PI5     | TIM8_CH1, SAI2_SCK_A, FMC_NBL3, DCMI_VSYNC, LCD_B5 |
| 20  | PI4     | TIM8_BKIN, SAI2_MCLK_A, FMC_NBL2, DCMI_D5, LCD_B4 |
| 21  | PB9     | TIM17_CH1, TIM4_CH4, DFSDM1, I2C1_SDA, SPI2_NSS/I2S2, I2C4_SDA, SDMMC1_CDIR, UART4_TX, FDCAN1_TX, SDMMC2_D5, SDMMC1_D5, DCMI_D7, LCD_B7 |
| 22  | PB8     | TIM16_CH1, TIM4_CH3, DFSDM1, I2C1_SCL, I2C4_SCL, SDMMC1_CKIN, UART4_RX, FDCAN1_RX, SDMMC2_D4, ETH_TXD3, SDMMC1_D4, DCMI_D6, LCD_B6 |
| 23  | PB7     | TIM17_CH1N, TIM4_CH2, I2C1_SDA, I2C4_SDA, USART1_RX, LPUART1_RX, DFSDM1, FMC_NL, DCMI_VSYNC ⚠️ DCMI_VSYNC |
| 24  | PB6     | TIM16_CH1N, TIM4_CH1, I2C1_SCL, CEC, I2C4_SCL, USART1_TX, LPUART1_TX, FDCAN2_TX, QUADSPI_BK1_NCS, DFSDM1, FMC_SDNE1, DCMI_D5, UART5_TX ⚠️ QUADSPI_NCS |
| 25  | PB5     | TIM17_BKIN, TIM3_CH2, I2C1_SMBA, SPI1_MOSI/I2S1, I2C4_SMBA, SPI3_MOSI/I2S3, SPI6_MOSI, FDCAN2_RX, OTG_HS_ULPI_D7, ETH_PPS_OUT, FMC_SDCKE1, DCMI_D10, UART5_RX |
| 26  | PB4     | NJTRST, TIM16_BKIN, TIM3_CH1, SPI1_MISO/I2S1, SPI3_MISO/I2S3, SPI2_NSS/I2S2, SPI6_MISO, SDMMC2_D3, UART7_TX |
| 27  | PB3     | JTDO/TRACESWO, TIM2_CH2, SPI1_SCK/I2S1, SPI3_SCK/I2S3, SPI6_SCK, SDMMC2_D2, CRS_SYNC, UART7_RX |
| 28  | PG14    | LPTIM1_ETR, SPI6_MOSI, USART6_TX, QUADSPI_BK2_IO3, ETH_TXD1/RMII_TXD1, FMC_A25, LCD_B0 |
| 29  | PG13    | LPTIM1_OUT, SPI6_SCK, USART6_CTS, ETH_TXD0/RMII_TXD0, FMC_A24, LCD_R0 |
| 30  | PG12    | LPTIM1_IN1, SPI6_MISO, USART6_RTS, SPDIFRX_IN2, ETH_TXD1/RMII_TXD1, FMC_NE4, LCD_B1 |
| 31  | PG11    | LPTIM1_IN2, SPI1_SCK/I2S1, SPDIFRX_IN1, SDMMC2_D2, ETH_TX_EN/RMII_TX_EN, DCMI_D3, LCD_B3 |
| 32  | PG10    | SPI1_NSS/I2S1_WS, SAI2_SD_B, FMC_NE3, DCMI_D2, LCD_G3/B2 |
| 33  | PG9     | SPI1_MISO/I2S1, USART6_RX, SPDIFRX_IN4, QUADSPI_BK2_IO2, SAI2_FS_B, FMC_NE2, DCMI_VSYNC |
| 34  | PD7     | SPI1_MOSI/I2S1, DFSDM1, USART2_CK, SPDIFRX_IN1, SDMMC2_CMD, FMC_NE1 |
| 35  | PD6     | SAI1/4_D1, DFSDM1, SPI3_MOSI/I2S3, USART2_RX, SDMMC2_CK, FMC_NWAIT, DCMI_D10, LCD_B2 |
| 36  | PD5     | HRTIM_EEV3, USART2_TX, FMC_NWE |
| 37  | PD4     | HRTIM_FLT3, SAI3_FS_A, USART2_RTS, FMC_NOE |
| 38  | PD3     | DFSDM1_CKOUT, SPI2_SCK/I2S2, USART2_CTS, FMC_CLK, DCMI_D5, LCD_G7 ⚠️ DCMI_D5 |
| 39  | PD2     | TIM3_ETR, UART5_RX, SDMMC1_CMD, DCMI_D11 ⚠️ SDMMC1_CMD |
| 40  | PC12    | SPI3_MOSI/I2S3, USART3_CK, UART5_TX, SDMMC1_CK, DCMI_D9 ⚠️ SDMMC1_CK |
| 41  | PC11    | DFSDM1, SPI3_MISO/I2S3, USART3_RX, UART4_RX, QUADSPI_BK2_NCS, SDMMC1_D3, DCMI_D4 ⚠️ SDMMC1_D3 |
| 42  | PC10    | DFSDM1, SPI3_SCK/I2S3, USART3_TX, UART4_TX, QUADSPI_BK1_IO1, SDMMC1_D2, DCMI_D8, LCD_R2 ⚠️ SDMMC1_D2 |
| 43  | PA15    | JTDI, TIM2_CH1/ETR, CEC, SPI1_NSS/I2S1_WS, SPI3_NSS/I2S3_WS, SPI6_NSS, UART4_RTS, UART7_TX |
| 44  | PA14    | JTCK/SWCLK ⚠️ SWD debug |
| 45  | PI3     | TIM8_ETR, SPI2_MOSI/I2S2, FMC_D27, DCMI_D10 ⚠️ DCMI_PWDN |
| 46  | PI2     | TIM8_CH4, SPI2_MISO/I2S2, FMC_D26, DCMI_D9, LCD_G7 |
| 47  | PI1     | TIM8_BKIN2, SPI2_SCK/I2S2, FMC_D25, DCMI_D8, LCD_G6 |
| 48  | PI0     | TIM5_CH4, SPI2_NSS/I2S2_WS, FMC_D24, DCMI_D13, LCD_G5 |
| 49  | PH15    | TIM8_CH3N, FMC_D23, DCMI_D11, LCD_G4 |
| 50  | PH14    | TIM8_CH2N, UART4_RX, FDCAN1_RX, FMC_D22, DCMI_D4, LCD_G3 |

---


## Camera (DVP)

DCMI-18PIN connector:

| Connector Pin | Signal     | MCU Pin                        |
|---------------|------------|--------------------------------|
| 1             | CAM_3V3    | 3.3V (dedicated camera supply) |
| 2             | GND        | GND                            |
| 3             | DCMI_VSYNC | PB7                            |
| 4             | DCMI_SCL   | PG3                            |
| 5             | DCMI_HSYNC | PA4                            |
| 6             | DCMI_SDA   | PB10                           |
| 7             | DCMI_RST   | PC5                            |
| 8             | DCMI_D0    | PC6                            |
| 9             | DCMI_D1    | PC7                            |
| 10            | DCMI_D2    | PC8                            |
| 11            | DCMI_D3    | PC9                            |
| 12            | DCMI_D4    | PC11                           |
| 13            | DCMI_D5    | PD3                            |
| 14            | DCMI_D6    | PB8                            |
| 15            | DCMI_D7    | PB9                            |
| 16            | DCMI_PCLK  | PA6                            |
| 17            | LED_EN     | PC4                            |
| 18            | DCMI_PWDN  | PI3                            |

---

## LCD1 — RGB Interface

RGB parallel display + touch panel header. Exact pin mapping to be confirmed — see [peripherals.md](peripherals.md#lcd1-rgb).

---

## LCD2 — SPI Interface

SPI display + touch panel header. Exact pin mapping to be confirmed — see `docs/peripherals.md`.
