# mictorHSMC

**Mictor to HSMC Adapter / Breakout Board**
(Mictorコネクタ - HSMC変換/ブレークアウト基板)

## Overview
This repository contains the KiCad design files for an adapter board that connects a **Mictor connector** (often used for Logic Analyzers and JTAG tracers) to an **HSMC (High-Speed Mezzanine Card)** interface.

This project allows for signal probing or debugging of HSMC-equipped FPGA boards (e.g., Intel/Altera DE-series) using standard Mictor-compatible equipment.

本リポジトリは、MictorコネクタをHSMCインターフェースに変換・接続するためのKiCad設計データを公開するものです。主にFPGAボード（HSMC搭載機）の信号をロジックアナライザ等でデバッグする用途を想定しています。

## Specifications

* **Connector A (Mictor):**
    * Part Number: `5767007-8` (TE Connectivity)
    * Type: 38-pin Mictor Receptacle
* **Connector B (HSMC):**
    * Part Number: `ASP-122952-01` (Samtec)
    * Type: Male Intel® HSMC Specified Q Strip® Connector
* **PCB Tool:** KiCad (v6.0 or later recommended)

## Pin Assignment
The Mictor connector pins are mapped to the HSMC interface as follows.
(Mictorコネクタの各ピンは以下のようにHSMCへ接続されています)

| Mictor Pin | Net Name | HSMC Pin |
| :--- | :--- | :--- |
| 1 | HSM_CLKOUT0 | 39 |
| 2 | HSM_CLKIN0 | 40 |
| 3 | HSM_D0 | 41 |
| 4 | HSM_D1 | 42 |
| 5 | HSM_D2 | 43 |
| 6 | HSM_D3 | 44 |
| 7 | HSM_D4 | 47 |
| 8 | HSM_D5 | 48 |
| 9 | HSM_D6 | 49 |
| 10 | HSM_D7 | 50 |
| 11 | HSM_D8 | 53 |
| 12 | HSM_D9 | 54 |
| 13 | HSM_D10 | 55 |
| 14 | HSM_D11 | 56 |
| 15 | HSM_D12 | 59 |
| 16 | HSM_D13 | 60 |
| 17 | HSM_D14 | 61 |
| 18 | HSM_D15 | 62 |
| 19 | HSM_D16 | 65 |
| 20 | HSM_D17 | 66 |
| 21 | HSM_D18 | 67 |
| 22 | HSM_D19 | 68 |
| 23 | HSM_D20 | 71 |
| 24 | HSM_D21 | 72 |
| 25 | HSM_D22 | 73 |
| 26 | HSM_D23 | 74 |
| 27 | HSM_D24 | 77 |
| 28 | HSM_D25 | 78 |
| 29 | HSM_D26 | 79 |
| 30 | HSM_D27 | 80 |
| 31 | HSM_D28 | 83 |
| 32 | HSM_D29 | 84 |
| 33 | HSM_D30 | 85 |
| 34 | HSM_D31 | 86 |
| 35 | HSM_D32 | 89 |
| 36 | HSM_D33 | 90 |
| 37 | HSM_D34 | 91 |
| 38 | HSM_D35 | 92 |

**Note:** Mictor Shield pins (S1-S5) are connected to the common Ground (HSMC Shield Pins S1-S12).

## ⚠️ Attribution & License for Footprints

This repository includes footprint and symbol data downloaded from **SnapEDA** and other component distributors to ensure the completeness of the project files. These files are included solely for the purpose of reproducing this specific PCB design.

**Note to Users:**
* The footprints and symbols for the connectors (**TE 5767007-8** and **Samtec ASP-122952-01**) are the intellectual property of their respective creators/providers.
* If you intend to use these footprints for a different project, please download the latest and official versions directly from the provider to ensure accuracy and compliance with their licensing terms.

**Sources:**
* [Samtec ASP-122952-01 on SnapEDA](https://www.snapeda.com/parts/ASP-122952-01/Samtec/view-part/)
* [Samtec 5767007-8 on SnapEDA](https://www.snapeda.com/parts/5767007-8/TE%20Connectivity/view-part/)

## Disclaimer
This project is a hobbyist creation and is provided "AS IS" without warranty of any kind. The author is not responsible for any damage to your hardware (FPGA boards, probes, etc.) caused by the use of this design. Please verify pinouts and signal integrity before fabrication.

本設計データは無保証です。使用に伴うハードウェア（FPGAや測定器等）の故障・損害について作者は責任を負いません。製造前にピンアサインや信号品質を十分にご確認ください。
