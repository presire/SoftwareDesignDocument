# library-specifications

ライブラリ (`.so` / `.dll` / `.a` / `.lib`) の**ライブラリ設計書**と**開発委託仕様書**のサンプル集です。  

> **注意**:  
> 掲載しているライブラリ `MochDat` は、サンプル用に作成した **架空のライブラリ** です。  
> 文書中の会社名 (株式会社サンプルソフト)、メールアドレス (`example.jp`) 等も全てダミーです。  

## 構成

```
.
├── library-specifications/      # ライブラリ設計書
│   ├── [ライブラリ設計書]MochDat_Linux(.so).xlsx      # 動的ライブラリ (Linux)
│   ├── [ライブラリ設計書]MochDat_Linux(.a).xlsx       # 静的ライブラリ (Linux)
│   ├── [ライブラリ設計書]MochDat_Windows(.dll).xlsx   # 動的ライブラリ (Windows)
│   └── [ライブラリ設計書]MochDat_Windows(.lib).xlsx   # 静的ライブラリ (Windows)
└── outsourcing-specifications/  # 開発委託仕様書 (RFP)
    ├── [開発委託仕様書]MochDat_Linux(.so).xlsx
    └── [開発委託仕様書]MochDat_Windows(.dll).xlsx
```

| 文書 | 内容 |
|---|---|
| ライブラリ設計書 | 公開API一覧<br>型定義エラーコード<br>呼出シーケンス<br>バイナリ仕様<br>エクスポートシンボル<br>互換性・バージョン方針<br>ビルド・配布・SBOMなど |
| 開発委託仕様書 | 依頼概要<br>委託範囲<br>機能・インタフェース (ABI)・非機能要件<br>開発環境<br>品質・セキュリティ要件<br>納品物<br>スケジュール<br>検収・契約条件など |

## 使い方

OnlyOfficeまたはLibreOffice Calcで開いてください。  
自分のライブラリの設計書を作成する時の構成・記載粒度・書式の見本として利用できます。  

## ライセンス

本リポジトリの内容は、[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)の下で提供されます。  
表示 (クレジット) を行えば、改変・再配布・商用利用が可能です。  

詳細は、[LICENSE](LICENSE)を参照してください。  

Copyright (c) 2026 Presire  
