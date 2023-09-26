               USB
               _____
        ------|     |------
      1 |o    |_____|    o| 40 
      2 |o               o| 39
      3 |o               o| 38 
      4 |o               o| 37
      5 |o               o| 36
      6 |o               o| 35
      7 |o               o| 34
      8 |o               o| 33
      9 |o               o| 32
     10 |o               o| 31
     11 |o               o| 30
     12 |o               o| 29
     13 |o               o| 28
     14 |o               o| 27
     15 |o               o| 26
     16 |o               o| 25
     17 |o               o| 24
     18 |o               o| 23
     19 |o               o| 22
     20 |o   O  ooo  O   o| 21
        -------------------
                /|\
          SWCLK- | -SWDIO
                GND

| UART     | I2C      | SPI      | GPIO/GND | PIN |     | PIN | GPIO/PWR/GND   | ADC/SPI  | I2C      | UART     |
|----------|----------|----------|----------|-----|-----|-----|----------------|----------|----------|----------|
| UART0 TX | I2C0 SDA | SPI0 RX  | GP0      | 1   |     | 40  | VBUS           |          |          |          |
| UART0 RX | I2C0 SCL | SPI0 SCL | GP1      | 2   |     | 39  | VSYS           |          |          |          |
|          |          |          | Ground   | 3   |     | 38  | Ground         |          |          |          |
|          | I2C1 SDA | SPI0 SCK | GP2      | 4   |     | 37  | 3V3_EN         |          |          |          |
|          | I2C1 SCL | SPI0 TX  | GP3      | 5   |     | 36  | 3V3(OUT)       |          |          |          |
| UART1 TX | I2C0 SDA | SPI0 RX  | GP4      | 6   |     | 35  |                | ADC_VREF |          |          |
| UART1 RX | I2C0 SCL | SPI CSn  | GP5      | 7   |     | 34  | GP28           | ADC2     |          |          |
|          |          |          | Ground   | 8   |     | 33  | Ground         | AGND     |          |          |
|          | I2C1 SDA | SPI0 SCK | GP6      | 9   |     | 32  | GP27           | ADC1     | I2C1 SCL |          |
|          | I2C1 SCL | SPI0 TX  | GP7      | 10  |     | 31  | GP26           | ADC0     | I2C1 SDA |          |
| UART1 TX | I2C0 SDA | SPI1 RX  | GP8      | 11  |     | 30  | RUN            |          |          |          |
| UART1 RX | I2C0 SCL | SPI1 CSn | GP9      | 12  |     | 29  | GP22           |          |          |          |
|          |          |          | Ground   | 13  |     | 28  | Ground         |          |          |          |
|          | I2C1 SDA | SPI1 SCK | GP10     | 14  |     | 27  | GP21           |          | I2C0 SCL |          |
|          | I2C1 SCL | SPI1 TX  | GP11     | 15  |     | 26  | GP20           |          | I2C0 SDA |          |
| UART0 TX | I2C0 SDA | SPI1 RX  | GP12     | 16  |     | 25  | GP19           | SPI0 TX  | I2C1 SCL |          |
| UART0 RX | I2C0 SCL | SPI1 CSn | GP13     | 17  |     | 24  | GP18           | SPI0 RX  | I2C1 SDA |          |
|          |          |          | Ground   | 18  |     | 23  | Ground         |          |          |          |
|          | I2C1 SDA | SPI1 SCK | GP14     | 19  |     | 22  | GP17           | SPI0 CSn | I2C0 SCL | UART0 RX |
|          | I2C1 SCL | SPI1 TX  | GP15     | 20  |     | 21  | GP16           | SPI0 RX  | I2C0 SDA | UART0 TX |
 
|          | DEBUG      |           |
|----------|------------|-----------|
| **Left** | **Middle** | **Right** |
| SWCLK    | Ground     | SWDIO     |

LED=GP25
