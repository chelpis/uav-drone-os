# 20250509 SensorHub

SensorHub描述一層軟硬體元件，讓offboard application能取用多種sensor的資料

## 支援sensor列表

### 接在 FMU 上的 sensor

此類 sensor 的 driver 會由 PX4 支援，其數據會直接被 PX4 使用
此數據 (或者某些情況下的raw data) 將透過 MAVLink 傳送至 Companion Computer (CC) 
使的 offboard application 能取用

- IMU
  - Analog Devices 
    - ADIS16448/16470/16477/16497/16507
  - Bosch 
    - BMI055/085/088/088-i2c/270
  - Invensense 
    - IAM20680hp
    - ICM20602/200608g/20649/20689/20948/40609d/42605/42670p/42688p/45686
    - IIM42652/42653
    - MPU6000/6500/9250
  - Murata
    - SCH16T
  - NXP
    - FXAS21002C
    - FXOS8701CQ
  - ST
    - L3GD20
    - LSM303D/9DS1
  - Invensense
    - ICP101xx/201xx
  - 
- 空速計
  - [TFSLOT](https://docs.px4.io/main/en/sensor/airspeed_tfslot.html)
- 氣壓計
  - Bosch
    - BMP280/388/581
  - Infineon
    - DPS310
  - GOERTEK
    - SPA06
    - SPL06
  - ST
    - LPS22HB/25H/33HW
  - Maiertek
    - MPC2520
  - NXP
    - MPL3115A2
  - TE Connectivity
    - MS5611/5837
  - 上海路溱微
    - TCBP001TA
- 距離偵測
  - [VL53L1X](https://holybro.com/products/st-vl53l1x-lidar)
  - [HC-SR04](https://www.taiwaniot.com.tw/product/hc-sr04/)
  - LightWare Lidar
    - SF1X/02/45
    - LW20
  - Ainstein US-D1 
  - LeddarOne Lidar
  - Benewake TFmini LiDAR
  - Lidar-Lite
  - TeraRanger
  - Avionics Anonymous Laser Altimeter DroneCan Interface
- GNSS
  - ARK GPS (CAN)
  - ARK SAM GPS
  - ARK TESEO GPS
  - CUAV NEO 3 GPS
  - CUAV NEO 3 Pro GPS (CAN)
  - CUAV NEO 3X GPS (CAN)
  - Holybro DroneCAN M8N GPS (CAN)
  - LOCOSYS Hawk A1 GNSS
  - Holybro M8N & M9N GPS
  - Sky-Drones SmartAP GPS
- RTK GNSS
  - ARK RTK GPS (CAN)
  - ARK MOSAIC-X5 RTK GPS (CAN)
  - RTK GPS Heading with Dual u-blox F9P
  - CUAV C-RTK
  - CUAV C-RTK2 PPK/RTK GNSS
  - CUAV C-RTK 9Ps
  - DATAGNSS GEM1305 RTK GNSS
  - Femtones MINI2 Receiver
  - Freefly RTK GPS
  - Holybro H-RTK ZED-F9P (DroneCAN)
  - Holybro H-RTK-F9P
  - Holybro H-RTK-M8P
  - Holybro H-RTK Unicore UM982 GPS
  - Locosys Hawk R1
  - Locosys Hawk R2
  - Septentrio GNSS Receivers
  - rimble MB-Two
  - HEX/ProfiCNC Here+ RTK GPS
- 慣性導航
  - [VectorNav](https://docs.px4.io/main/en/sensor/vectornav.html)
- 光流+距離偵測
  - [micoair MTF-02P](https://micoair.com/optical_range_sensor_mtf-02p/)
  - [ARK Flow](https://docs.px4.io/main/en/dronecan/ark_flow.html)
  - [ARK Flow MR](https://docs.px4.io/main/en/dronecan/ark_flow_mr.html)
  - [PMW3901-Based Flow Sensors](https://docs.px4.io/main/en/sensor/pmw3901.html)

### 接在 Companion Computer (CC) 上的 sensor

此類 sensor 的 driver 會由 CC 支援，使的 offboard application 能取用

- 360度2D光達
  - [waveshare D500 LIDAR KIT](https://www.waveshare.com/product/robotics/drivers-sensors/lidar/d500-lidar-kit.htm)
- RGB 相機
  - Raspberry Pi Camera Module V2
- RGBD 深度相機
  - Intel RealSense D4XX
