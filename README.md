# SoftwareDesignDocument

ソフトウェア開発で用いる設計書・計画書・契約書の**サンプル (記載例) 集**です。  
各書類の構成・記載粒度・書式の見本として利用できます。  

> **注意**:  
> 各サンプルに登場するシステム名・ライブラリ名 (`MochDat` 等)・会社名・人名・数値は、全て架空の記入例です。  
> 内容をそのまま実案件へ流用せず、構成や書き方の参考としてください。  

## ディレクトリ構造

```
.
├── Analysis_Flow_Specification/        # 解析フロー設計書
│   ├── README.md
│   └── [解析フロー設計書]MochDat_DAT解析.xlsx
├── Database_Design/                    # データベース設計書 (4分冊)
│   ├── README.md
│   ├── [スキーマ定義書]記載例_図書貸出管理システム.xlsx
│   ├── [テーブル定義書]記載例_図書貸出管理システム.xlsx
│   ├── [ストアド定義書]記載例_図書貸出管理システム.xlsx
│   └── [トリガー設定書]記載例_図書貸出管理システム.xlsx
├── File_Format_Definition/             # ファイルフォーマット定義書
│   ├── README.md
│   └── [ファイルフォーマット定義書]記載例_計測データ収集システム.xlsx
├── Functional_Overview/                # 機能概要書
│   ├── README.md
│   └── [機能概要書]掲示板閲覧・投稿.xlsx
├── NDA/                                # 秘密保持契約書 (外注先用)
│   ├── README.md
│   ├── 秘密保持契約書_外注先用.docx
│   └── 秘密保持契約書_外注先用_記入編集マニュアル.docx
├── Project_Plan/                       # プロジェクト計画書
│   ├── README.md
│   ├── [プロジェクト計画書]コンペ例_経費精算業務改革プロジェクト.pptx
│   └── [プロジェクト計画書]記載例_経費精算業務改革プロジェクト.pptx
└── library-specifications/             # ライブラリ設計書・開発委託仕様書
    ├── README.md
    ├── LICENSE
    ├── library-specifications/         # ライブラリ設計書
    │   ├── README.md
    │   ├── [ライブラリ設計書]MochDat_Linux(.so).xlsx
    │   ├── [ライブラリ設計書]MochDat_Linux(.a).xlsx
    │   ├── [ライブラリ設計書]MochDat_Windows(.dll).xlsx
    │   └── [ライブラリ設計書]MochDat_Windows(.lib).xlsx
    └── outsourcing-specifications/     # 開発委託仕様書 (RFP)
        ├── README.md
        ├── [開発委託仕様書]MochDat_Linux(.so).xlsx
        └── [開発委託仕様書]MochDat_Windows(.dll).xlsx
```

各ディレクトリの`README.md`には、そのディレクトリのサンプルについてシート・章・条項ごとの記載項目の説明があります。  

## 各ディレクトリの説明

### [Analysis_Flow_Specification](Analysis_Flow_Specification/README.md) - 解析フロー設計書

プログラム / ライブラリが行う解析処理 (ファイル・データの読込と解析) の流れを記載する書類です。  
1冊で1つの解析フローを扱います。  

| ファイル | 内容 |
|---|---|
| `[解析フロー設計書]MochDat_DAT解析.xlsx` | 架空ライブラリ`MochDat`のDATファイル解析を題材にした見本<br>解析概要、概要解析フロー図、詳細フロー (文字コード判定・行解析)、判定・分岐一覧、入出力処理設計 |

### [Database_Design](Database_Design/README.md) - データベース設計書

架空の「図書貸出管理システム」(PostgreSQL 16) を題材にした、4分冊構成のデータベース設計書です。  

| ファイル | 内容 |
|---|---|
| `[スキーマ定義書]記載例_図書貸出管理システム.xlsx` | DB全体の前提 (共通仕様・データベース / スキーマ / 権限等) |
| `[テーブル定義書]記載例_図書貸出管理システム.xlsx` | ER図・テーブル一覧・テーブル (ビュー) ごとの定義・コード値 |
| `[ストアド定義書]記載例_図書貸出管理システム.xlsx` | ストアドプロシージャ・ファンクションの定義 |
| `[トリガー設定書]記載例_図書貸出管理システム.xlsx` | トリガーの定義 |

### [File_Format_Definition](File_Format_Definition/README.md) - ファイルフォーマット定義書

架空の「計測データ収集システム」が入出力するファイル・電文の仕様を定義した記載例です。  

| ファイル | 内容 |
|---|---|
| `[ファイルフォーマット定義書]記載例_計測データ収集システム.xlsx` | 6種類のファイル・電文 (JSON / CSV / 固定長 / バイナリ / HTTP / TOML) の定義<br>共通仕様、ファイル一覧、ファイル連携タイミング一覧、コード値一覧 |

### [Functional_Overview](Functional_Overview/README.md) - 機能概要書

1冊 = 1大分類機能として、機能階層・画面遷移・データフローと、画面ごとのレイアウト・処理記述・項目一覧を記載する機能概要書の見本です。  

| ファイル | 内容 |
|---|---|
| `[機能概要書]掲示板閲覧・投稿.xlsx` | 掲示板の閲覧・投稿機能を題材にした見本 (画面6件・全21シート) |

### [NDA](NDA/README.md) - 秘密保持契約書 (外注先用)

自社 (甲=委託者) と外注先 (乙=受託者) が、ソフトウェア開発業務の検討・遂行に先立ち締結する双務型NDAのひな形です。  

| ファイル | 内容 |
|---|---|
| `秘密保持契約書_外注先用.docx` | NDAのひな形本体<br>本文第1条〜第21条、別紙1 (業務概要・秘密情報の指定)、別紙2 (返還・廃棄証明書の様式)<br>`【　】`で囲まれた部分を案件に合わせて記入する |
| `秘密保持契約書_外注先用_記入編集マニュアル.docx` | ひな形の記入・編集方法を説明する社内用マニュアル (相手方には送付しない) |

### [Project_Plan](Project_Plan/README.md) - プロジェクト計画書

架空の「経費精算業務改革プロジェクト」を題材にしたプロジェクト計画書です。  
方針、スケジュール、体制、コミュニケーション計画、プロジェクト管理計画、プロジェクトルール等の章で構成されます。  

| ファイル | 内容 |
|---|---|
| `[プロジェクト計画書]コンペ例_経費精算業務改革プロジェクト.pptx` | コンペ・提案提出用 (85枚)<br>記載例の項目に提案向けの節を追加した完全版 |
| `[プロジェクト計画書]記載例_経費精算業務改革プロジェクト.pptx` | 計画書の標準的な記載例 (46枚)<br>必須節と主要な任意節のみ |

### [library-specifications](library-specifications/README.md) - ライブラリ設計書・開発委託仕様書

架空のライブラリ`MochDat`を題材にした、ライブラリの設計書と開発委託仕様書のサンプル集です。  

| サブディレクトリ | 内容 |
|---|---|
| [library-specifications/](library-specifications/library-specifications/README.md) | **ライブラリ設計書** (Linux `.so` / `.a`、Windows `.dll` / `.lib` の4種)<br>公開API一覧、型定義、エラーコード、呼出シーケンス、API詳細、バイナリ仕様、シンボル一覧、互換性・バージョン方針、ビルド・配布・SBOM等 |
| [outsourcing-specifications/](library-specifications/outsourcing-specifications/README.md) | **開発委託仕様書** (提案依頼書 (RFP) を兼ねる。Linux `.so`、Windows `.dll` の2種)<br>依頼概要、委託範囲・役割分担、機能・インタフェース (ABI)・非機能要件、開発環境、品質・セキュリティ要件、納品物、スケジュール、検収・契約条件等 |

本ディレクトリの内容は[CC BY 4.0](library-specifications/LICENSE)の下で提供されています。  

## ファイル形式と閲覧方法

| 形式 | 対象 | 推奨ソフトウェア |
|---|---|---|
| `.xlsx` | 各種設計書・定義書・仕様書 | OnlyOffice、LibreOffice Calc、Microsoft Excel |
| `.docx` | 秘密保持契約書・記入編集マニュアル | OnlyOffice、LibreOffice Writer、Microsoft Word |
| `.pptx` | プロジェクト計画書 | OnlyOffice、LibreOffice Impress、Microsoft PowerPoint |
