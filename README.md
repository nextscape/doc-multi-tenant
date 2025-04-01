# Microsoft Azure におけるマルチテナント アーキテクチャ設計ガイド
本ドキュメントは、Azure において複数のテナント（顧客）が同一のリソースを共有しながら、テナント毎のデータや設定を分離して管理するためのアーキテクチャ設計ガイダンスです。[ネクストスケープ](https://nextscape.net/)の顧客への導入実績を基に、マルチテナント特有の課題と解決方法、さらに Azure の PaaS / Serverless を活用した設計アプローチをまとめています。  
ここで取り上げた製品・サービスの詳細および最新情報は[製品ドキュメント](https://docs.microsoft.com)をご参照ください。

## [はじめに](./docs/chapter00.md)
マルチテナント アプリケーションの定義と本ドキュメントの対象読者を記載しています。

## [1章 ビジネスゴールの定義](./docs/chapter01.md)
マルチテナント アーキテクチャ設計におけるビジネスゴールの重要性と定義すべきゴールの項目を説明します。

## [2章 マルチテナント アーキテクチャの全体像](./docs/chapter02.md)
マルチテナント アーキテクチャ全体の構造と概念を定義し、構築する優先度の高いアーキテクチャ要素を説明します。

## [3章 テナント分離モデルの選択](./docs/chapter03-00.md)
マルチテナント アーキテクチャの設計で最大の考慮事項の１つは、テナント分離モデルです。アーキテクチャのレイヤーを３つに分けて、各レイヤーにおけるテナント分離モデルの選択肢とそれぞれの特徴を説明します。
- [アプリケーション](./docs/chapter03-01.md)
- [データストア](./docs/chapter03-02.md)
- [バッチ処理](./docs/chapter03-03.md)

## [4章 テナント管理](./docs/chapter04.md)
マルチテナント アプリケーションの設計において、テナント ID などの識別子からテナントを判別する方法について説明します。また、テナントの無効化や削除、デプロイ スタンプ間の移動など、テナントのライフサイクルについても説明します。

## [5章 プロビジョニングの自動化](./docs/chapter05.md)
マルチテナント アプリケーションの更新プログラムの展開に加えて、テナントの追加や更新に関連するプロビジョニング プロセスを自動化する方法について説明します。

## [6章 マルチテナントを考慮すべき非機能要件](./docs/chapter06.md)
Azure をベースとしたシステムを構築する際の非機能要件のうち、マルチテナント特有の要件について説明します。
- ID とアクセス管理
- モニタリング

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.