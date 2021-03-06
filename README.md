AWS MQTT demo example project
=============================

Click to import in Keil Studio Cloud: [![Open in Keil Studio](https://img.shields.io/badge/Keil%20Studio-Import-blue?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAyNS40LjEsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0iTGF5ZXJfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiDQoJIHZpZXdCb3g9IjAgMCA0NyAxNCIgc3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgNDcgMTQ7IiB4bWw6c3BhY2U9InByZXNlcnZlIj4NCjxzdHlsZSB0eXBlPSJ0ZXh0L2NzcyI+DQoJLnN0MHtmaWxsOiNGRkZGRkY7fQ0KPC9zdHlsZT4NCjxwYXRoIGNsYXNzPSJzdDAiIGQ9Ik00LjcsN2MwLDIuMiwxLjQsNC4xLDMuNSw0LjFjMS44LDAsMy42LTEuNCwzLjYtNC4xYzAtMi44LTEuNy00LjItMy42LTQuMkM2LjIsMi45LDQuNyw0LjcsNC43LDcgTTExLjYsMC41DQoJaDIuOXYxM2gtMi45di0xLjNjLTAuOSwxLjEtMi4zLDEuNy0zLjcsMS43QzQsMTMuOSwxLjgsMTAuNiwxLjgsN2MwLTQuMywyLjctNi45LDYuMS02LjljMS41LDAsMi44LDAuNywzLjcsMS45VjAuNXoiLz4NCjxwYXRoIGNsYXNzPSJzdDAiIGQ9Ik0xOCwwLjVIMjF2MS4yYzAuMy0wLjQsMC43LTAuOCwxLjItMS4xYzAuNS0wLjMsMS4yLTAuNCwxLjctMC40YzAuOCwwLDEuNiwwLjIsMi4zLDAuNmwtMS4yLDIuOA0KCWMtMC40LTAuMy0xLTAuNC0xLjUtMC40Yy0wLjctMC4xLTEuMywwLjItMS44LDAuN0MyMSw0LjYsMjEsNS45LDIxLDYuOHY2LjdIMThWMC41eiIvPg0KPHBhdGggY2xhc3M9InN0MCIgZD0iTTI4LjIsMC41aDIuOXYxLjJjMC43LTAuOSwxLjktMS42LDMuMS0xLjZjMS4zLDAsMi42LDAuNywzLjIsMS45YzAuOS0xLjIsMi4yLTEuOSwzLjctMS45DQoJQzQyLjcsMCw0NCwwLjksNDQuNywyLjJjMC4yLDAuNCwwLjcsMS40LDAuNywzLjN2OC4xaC0yLjlWNi4zYzAtMS41LTAuMi0yLjEtMC4yLTIuM2MtMC4yLTAuNy0wLjktMS4yLTEuNy0xLjENCgljLTAuNywwLTEuMywwLjMtMS43LDAuOWMtMC41LDAuOC0wLjYsMS45LTAuNiwyLjl2Ni43aC0yLjlWNi4zYzAtMS41LTAuMi0yLjEtMC4yLTIuM2MtMC4yLTAuNy0wLjktMS4yLTEuNy0xLjENCgljLTAuNywwLTEuMywwLjMtMS43LDAuOWMtMC41LDAuOC0wLjYsMS45LTAuNiwyLjl2Ni43aC0yLjlMMjguMiwwLjV6Ii8+DQo8L3N2Zz4NCg==&logoWidth=47)](https://studio.keil.arm.com/?import=https://github.com/MDK-Packs/IMXRT1050_FreeRTOS-TCP)

Board: NXP IMXRT1050-EVKB
-------------------------

The tables below list the device configuration for this board. The board layer for the NXP IMXRT1050-EVKB is using the software component `::Board Support: SDK Project Template: project_template (Variant: evkbimxrt1050)` from `NXP.EVKB-IMXRT1050_BSP.13.1.0` pack.

The heap/stack setup and the CMSIS-Driver assignment is in configuration files of related software components.

The example project can be re-configured to work on custom hardware. Refer to ["Configuring Example Projects with MCUXpresso Config Tools"](https://github.com/MDK-Packs/Documentation/tree/master/Using_MCUXpresso) for information.

### System Configuration

| System Component        | Setting
|:------------------------|:----------------------------------------
| Device                  | MIMXRT1052DVL6B
| Board                   | IMXRT1050-EVKB
| SDK Version             | ksdk2_0
| Heap                    | 64 kB (configured in linker script MIMXRT1052xxxxx_*.scf file)
| Stack (MSP)             |  1 kB (configured in linker script MIMXRT1052xxxxx_*.scf file)

### Clock Configuration

| Clock                   | Setting
|:------------------------|:----------------------------------------
| AHB_CLK_ROOT            | 600 MHz
| IPG_CLK_ROOT            | 150 MHz
| PERCLK_CLK_ROOT         |  75 MHz
| USDHC1_CLK_ROOT         | 198 MHz
| UART_CLK_ROOT           |  80 MHz
| ENET_125M_CLK           |  50 MHz
| ENET_25M_REF_CLK        |  25 MHz
| ENET_TX_CLK             |  50 MHz

**Note:** configured with Functional Group: `BOARD_BootClockRUN`

### GPIO Configuration and usage

| Functional Group       | Pin | Peripheral | Signal      | Identifier         | Pin Settings                                        | Usage
|:-----------------------|:----|:-----------|:------------|:-------------------|:----------------------------------------------------|:-----
| BOARD_InitDEBUG_UART   | K14 | LPUART1    | TX          | UART1_TXD          | default                                             | UART1 TX for debug console (GPIO_AD_B0_12)
| BOARD_InitDEBUG_UART   | L14 | LPUART1    | RX          | UART1_RXD          | default                                             | UART1 RX for debug console (GPIO_AD_B0_13)
| BOARD_InitENET         | A7  | ENET       | MDC         | ENET_MDC           | default                                             | Ethernet KSZ8081RNB pin MDC (GPIO_EMC_40)
| BOARD_InitENET         | C7  | ENET       | MDIO        | ENET_MDIO          | default                                             | Ethernet KSZ8081RNB pin MDIO (GPIO_EMC_41)
| BOARD_InitENET         | B13 | ENET       | REF_CLK     | ENET_TX_CLK        | default                                             | Ethernet KSZ8081RNB pin XI (GPIO_B1_10)
| BOARD_InitENET         | E12 | ENET       | RX_DATA, 0  | ENET_RXD0          | default                                             | Ethernet KSZ8081RNB pin RXD0 (GPIO_B1_04)
| BOARD_InitENET         | D12 | ENET       | RX_DATA, 1  | ENET_RXD1          | default                                             | Ethernet KSZ8081RNB pin RXD1 (GPIO_B1_05)
| BOARD_InitENET         | C12 | ENET       | RX_EN       | ENET_CRS_DV        | default                                             | Ethernet KSZ8081RNB pin CRS_DV (GPIO_B1_06)
| BOARD_InitENET         | C13 | ENET       | RX_ER       | ENET_RXER          | default                                             | Ethernet KSZ8081RNB pin RXER (GPIO_B1_11)
| BOARD_InitENET         | B12 | ENET       | TX_DATA, 0  | ENET_TXD0          | default                                             | Ethernet KSZ8081RNB pin TXD0 (GPIO_B1_07)
| BOARD_InitENET         | A12 | ENET       | TX_DATA, 1  | ENET_TXD1          | default                                             | Ethernet KSZ8081RNB pin TXD1 (GPIO_B1_08)
| BOARD_InitENET         | A13 | ENET       | TX_EN       | ENET_TXEN          | default                                             | Ethernet KSZ8081RNB pin TXEN (GPIO_B1_09)
| BOARD_InitUSDHC        | J2  | USDHC1     | DATA, 3     | SD1_D3             | default                                             | SD Card pin D3 (GPIO_SD_B0_05)
| BOARD_InitUSDHC        | H2  | USDHC1     | DATA, 2     | SD1_D2             | default                                             | SD Card pin D2 (GPIO_SD_B0_04)
| BOARD_InitUSDHC        | K1  | USDHC1     | DATA, 1     | SD1_D1             | default                                             | SD Card pin D1 (GPIO_SD_B0_03)
| BOARD_InitUSDHC        | J1  | USDHC1     | DATA, 0     | SD1_D0             | default                                             | SD Card pin D0 (GPIO_SD_B0_02)
| BOARD_InitUSDHC        | J4  | USDHC1     | CMD         | SD1_CMD            | default                                             | SD Card pin CMD (GPIO_SD_B0_00)
| BOARD_InitUSDHC        | J3  | USDHC1     | CLK         | SD1_CLK            | default                                             | SD Card pin CLK (GPIO_SD_B0_01)
| BOARD_InitARDUINO_UART | J12 | LPUART3    | TX          | LPUART3_TX         | default                                             | Arduino UNO R3 pin D1 (GPIO_AD_B1_06)
| BOARD_InitARDUINO_UART | K10 | LPUART3    | RX          | LPUART3_RX         | default                                             | Arduino UNO R3 pin D0 (GPIO_AD_B1_07)
| BOARD_InitUSER_LED     | F14 | GPIO1      | gpio_io, 09 | USER_LED           | Direction Output, GPIO initial state 1, mode PullUp | User LED (GPIO_AD_B0_09)
| BOARD_InitUSER_BUTTON  | L6  | GPIO5      | gpio_io, 00 | USER_BUTTON        | Direction Input, mode PullUp                        | User Button SW8 (WAKEUP)
| BOARD_InitI2C          | J11 | LPI2C1     | SCL         | I2C_SCL_FXOS8700CQ | Software Input On, Open drain                       | LPI2C1 for FXOS8700CQ (GPIO_AD_B1_00)
| BOARD_InitI2C          | K11 | LPI2C1     | SDA         | I2C_SDA_FXOS8700CQ | Software Input On, Open drain                       | LPI2C1 for FXOS8700CQ (GPIO_AD_B1_01)

### NVIC Configuration

| NVIC Interrupt      | Priority
|:--------------------|:--------
| ENET                | 8
| USDHC1              | 8
| LPUART3             | 8

**STDIO** is routed to debug console through Virtual COM port (DAP-Link, peripheral = LPUART1, baudrate = 115200)

### CMSIS-Driver mapping

| CMSIS-Driver | Peripheral
|:-------------|:----------
| ETH_MAC0     | ENET
| ETH_PHY0     | KSZ8081RNB (external)
| MCI0         | USDHC1
| USART3       | LPUART3

| CMSIS-Driver VIO  | Physical board hardware
|:------------------|:-----------------------
| vioBUTTON0        | User Button SW8 (WAKEUP)
| vioLED0           | User LED (GPIO_AD_B0_09)
| vioMotionAccelero | 3-Axis Accelerometer (FXOS8700CQ)
| vioMotionMagneto  | 3-Axis Magnetometer (FXOS8700CQ)
