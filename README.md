# GPIO Connector Adapter Board (TE 5767007-8 / Samtec ASP-122952-01)

このリポジトリは、TE Connectivity製 MICTORコネクタと Samtec製 ASPコネクタを相互接続し、GPIO信号へのアクセスやデバッグを容易にするために設計されたコネクタ基盤（アダプタボード）のハードウェア設計データを管理しています。

## 概要 (Overview)

本基盤は、FPGA評価ボードや高速信号処理ボード等に搭載されているSamtecコネクタから、ロジックアナライザや外部機器接続用として標準的なMICTORコネクタへ信号を引き出す（あるいは相互接続する）ことを目的としています。

### 主な用途
* FPGAボードのGPIO拡張
* ロジックアナライザによる信号解析（MICTORプローブ接続）
* カスタムハードウェア間の信号ブリッジ

## 搭載コネクタ (Components)

| 記号 | メーカー | 型番 | 説明 |
|:---:|:---|:---|:---|
| **CN1** | TE Connectivity | **5767007-8** | MICTOR Connector (38-pin / High Speed) |
| **CN2** | Samtec | **ASP-122952-01** | VITA 57 / FMC Style Connector (High Density Array) |
