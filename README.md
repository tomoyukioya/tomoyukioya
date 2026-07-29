# Software Portfolio

放送・通信分野の研究開発をルーツに、**映像・3D計測・組込・分散処理**まで、ハードウェアに近い層からアプリケーションまでを一貫して設計・実装しています。主言語は **C# / .NET**。C/C++・Python・Kotlin も日常的に使います。

![C#](https://img.shields.io/badge/C%23-239120?style=flat&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat&logo=dotnet&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)

> 掲載しているプロダクトは、取引先名や機密に関わる詳細を伏せ、技術的な側面を中心に紹介しています。

---

## 得意領域

- **放送・映像** — MPEG2-TS / ARIB 規格 / HLS 配信
- **3D・計測** — LiDAR・点群（LAS / LAZ） / センサ / AR
- **組込・決済端末** — Android 組込 / FeliCa・NFC / キャッシュレス決済
- **クラウド・分散処理** — AWS / 分散レンダリング基盤
- **無線・電波** — ローカル5G / 電波伝搬・エリア計算
- **業務システム・自動化** — WPF・WinForms / Blazor / スクレイピング・RPA

---

## 主なプロダクト

### 放送・映像
- **MPEG2-TS 解析・修復エンジン + HLS 配信基盤** — ARIB STD-B10 / B24 / B25 に準拠。実放送波に由来する TOT / PCR の不整合を検出・修復し、iOS / Android の再生系まで対応。長期にわたり保守を継続。
- **TS 結合・修復ツール群**（tsrepair / PcrCheck / TotDupCheck / TotGapCheck ほか） — C / C++ 実装。
- **字幕抽出ツール（ARIB STD-B24）**、および **BonDriver の C# 実装**。
- **HLS 動画ダウンローダ** — WebView2 + ffmpeg。

### 3D・計測
- **LiDAR 点群処理 / LAS・LAZ 1.4 パーサ** — .NET から扱えるよう **PDAL の C# ラッパーを自作**。
- **Livox 独自バイナリ（LVX）パーサ**、**多画面点群ビューア**（OpenGL）。
- **SignalR ベースのリアルタイム通信基盤**、**IoT 計測**（潮位センサ）、**AR 表示サーバ**、**3D TOF センサ アプリ**（WPF）。

### 組込・決済端末
- **Android 組込端末アプリ** — キオスク運用・SIP 通話を前提とした実装。見守り／ケアロボット向けへ展開。
- **無人販売・決済端末アプリ** — FeliCa / NFC / クレジット決済 / Adyen / モバイルSuica に対応。署名付き APK 配布、酒類販売対応ほか。

### クラウド・分散処理
- **クラウドレンダリング基盤（サーバ側）** — Maya / Blender / Arnold / V-Ray / ProRender に対応。AWS S3 連携、分散レンダリング、CLI 版、GPU タイプ・サーバ台数選択などを継続的に開発。

### 無線・電波
- **ローカル5G エリア計算アプリ** — ITU-R P.526 / F.1336、国土地理院 DEM・PLATEAU を用いたカバーエリア計算と地図描画。免許情報から既存エリアを生成し干渉を可視化（GPU 利用）。
- **LTE / 5G(NSA) ドライブテスト計測システム** — Kotlin / Chaquopy / Python / FastAPI / Leaflet。Qualcomm 診断ログ、RM520N-GL + Raspberry Pi 4B。

### 業務システム・自動化
- **不動産向け 物件情報管理アプリ** — 物件管理、ポータル自動入力、契約書テンプレートの自動判別・生成。約 **34,000 行・ユニットテスト 167 件**。.NET 8 / EF Core / WebView2 / GPT-4o。
- **ライセンス認証基盤** — サーバ + 常駐サービス + 組込ライブラリ + 管理画面。Blazor Server / ASP.NET Core Identity / RSA2048・SHA-256 / 難読化による解析耐性。
- **高速 A/D 変換ボードの FPGA 更新とホスト制御ソフト** — 200MSPS 化対応。レジスタ制御（ADS5295 / LMK04610 ほか）、DDR3・FIFO キャプチャ、波形ビューア（bin→CSV 変換つき）。
- **メール配信・名簿管理ツール**、**サイト間データ収集ツール**（WebView2 スクレイピング）など。

### Web・PWA
- **ペットシッター向け PWA**（Blazor / PWA / Push Notification）とバックエンド・CRM の開発・改修。

### 分散台帳・トレーディング
- **ERC トークン発行とポータル**（Ethereum / geth / スマートコントラクト）、**取引所 API 連携の自動売買ボット**（Python / BitMEX ほか）。

---

## 公開ソフトウェア（OSS）

| リポジトリ | 言語 | ライセンス | 内容 |
|---|---|---|---|
| [FileHistoryClone](https://github.com/tomoyukioya/FileHistoryClone) | C# | MIT | ファイル履歴風の常駐型・世代バックアップツール（`winget install tomoyukioya.FileHistoryClone`） |
| [WiFiArea](https://github.com/tomoyukioya/WiFiArea) | C# | MIT | ITU-R 勧告に基づく屋内 Wi-Fi エリアシミュレータ（距離損・壁透過・回折を合成） |
| [SmartPhoneCTI](https://github.com/tomoyukioya/SmartPhoneCTI) | C# | MIT | スマートフォンの着信を PC のデスクトップ通知として受け取る CTI（3層構成） |
| [WinKvm](https://github.com/tomoyukioya/WinKvm) | C# | MIT | CH9329 USB HID を用いたソフトウェア KVM コンソール（BIOS/UEFI 画面も操作可） |
| [TH850Library](https://github.com/tomoyukioya/TH850Library) | C# | MIT | USB 歩数計アクセスライブラリ |
| [CheckScreenColor](https://github.com/tomoyukioya/CheckScreenColor) | C# | Apache-2.0 | 画面のドットを監視し特定色で通知 |
| [MicroOvenCalc](https://github.com/tomoyukioya/MicroOvenCalc) | HTML/JS | — | 電子レンジの温め時間計算機 |

---

## 技術スタック

- **言語**: C# / C・C++ / Python / Kotlin・Java / JavaScript
- **.NET**: WPF・WinForms / ASP.NET Core / Blazor / EF Core
- **クラウド・基盤**: AWS（S3・Lambda・WAF） / Azure（App Service・DevOps）
- **データ**: SQL Server / SQLite / LiteDB
- **領域技術**: MPEG2-TS・ARIB / HLS / LiDAR・点群（LAS・LAZ） / FeliCa・NFC・決済 / SignalR / MQTT / ITU-R 電波伝搬

---

## 背景

放送・通信分野で長年にわたり研究開発に従事し、放送システム・情報システムの運用や、限定受信システム（CAS）を含むセキュリティ運用の実務を経験してきました。ハードウェア・通信・セキュリティに根ざした基盤の上に、現在のソフトウェア開発があります。
