<p align="center">
  <img src="assets/profile-banner.svg" alt="Embedded systems · Real-time · Control · Telemetry" width="100%">
</p>

<h1 align="center">mamorrozer</h1>

<p align="center">
  <strong>嵌入式软件 · 实时系统 · MCU 控制与通信</strong><br>
  从外设驱动、任务调度到设备联网，持续做可运行、可验证的工程项目。
</p>

<p align="center">
  <a href="https://github.com/mamorrozer/f407-freertos-esp32-telemetry">查看 FreeRTOS 双 MCU 遥测终端</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/C-embedded-173B5E?style=flat-square&logo=c" alt="C">
  <img src="https://img.shields.io/badge/STM32F407-Cortex--M4-173B5E?style=flat-square&logo=stmicroelectronics" alt="STM32F407">
  <img src="https://img.shields.io/badge/FreeRTOS-real--time-147D92?style=flat-square" alt="FreeRTOS">
  <img src="https://img.shields.io/badge/ESP32--S3-ESP--IDF-147D92?style=flat-square&logo=espressif" alt="ESP32-S3 and ESP-IDF">
  <img src="https://img.shields.io/badge/MQTT-device%20telemetry-3977A8?style=flat-square" alt="MQTT">
</p>

## 代表项目

### STM32F407 + FreeRTOS 环境遥测终端

基于 STM32F407 与 ESP32-S3 的双 MCU 项目：F407 采集 BMP280 / AHT20、刷新 TFT 并通过 UART 发送遥测；ESP32-S3 负责 Wi-Fi 和 MQTT。项目包含任务与队列划分、文本/二进制协议、CRC16、有限 RAM 缓存、断线恢复，以及 CMake / CTest 主机测试。

[查看源码、架构与验证记录 →](https://github.com/mamorrozer/f407-freertos-esp32-telemetry)

<p align="center">
  <a href="https://github.com/mamorrozer/f407-freertos-esp32-telemetry">
    <img src="https://raw.githubusercontent.com/mamorrozer/f407-freertos-esp32-telemetry/main/docs/assets/architecture.svg" alt="F407 sensor acquisition and TFT, UART telemetry to ESP32-S3, Wi-Fi and MQTT" width="92%">
  </a>
</p>

## 技术方向

| 方向 | 项目中使用的技术 |
|---|---|
| MCU 与固件 | C、STM32F407、TI MSPM0G3507、ESP32-S3 |
| 实时系统 | FreeRTOS 任务、周期调度、队列、运行状态观测 |
| 外设与通信 | UART、I²C、SPI、CRC16、MQTT |
| 构建与验证 | ESP-IDF、CMake、CTest、串口日志与双板联调 |

## 竞赛经历

- 2026 年全国大学生电子设计竞赛广东赛区省级三等奖。
- 第二十一届“信息杯”社会调研比赛二等奖（团队赛，2025 年 12 月）。

## 项目记录

我会在仓库中记录设计取舍、验证范围和未覆盖的情况。项目中的独立模块、主机测试结果与实机验证会分开说明；技术栈按实际项目使用经历列出。
