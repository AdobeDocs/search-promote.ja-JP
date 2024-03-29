---
description: Search&amp;Promote 8.13.0リリースノート。
solution: Target
title: Search&amp;Promote 8.13.0リリースノート（2014年4月17日）
topic-legacy: Release Notes,Site search and merchandising
uuid: b3524992-ff00-4a7c-a404-078242456734
exl-id: cba582ad-d388-4317-af06-b8b12b300f02
translation-type: tm+mt
source-git-commit: 7559f5f7437d46e3510d4659772308666425ec96
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 57%

---

# Search&amp;Promote8.13.0リリースノート（2014年4月17日）{#search-promote-release-notes}

| 新機能と機能強化 | 説明 |
|----------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 完全テーブル一致を含む動的ファセットのサポート | 一部のお客様は、多くの「SKUレベル」属性を持っており、動的ファセットを使用して選択および表示したいと考えていました。 その場合、オプションで、各動的ファセットフィールドを静的アカウント設定の最大 1 つのテーブル名に関連付けることができます。こうしたテーブルのリレーションシップは、検索時に、その検索に関連する動的ファセットフィールドに適用できます。[動的ファクトについて](../c-about-design-menu/c-about-dynamic-facets.md#concept_E65A70C9C2E04804BF24FBE1B3CAD899)を参照してください。 |

**修正点**

* データ表示の説明フィールドが変更され、`<search-description>`ではなく`<search-display-field>`タグを使用するようになりました。
* Index Connector に、プライマリキーに 2 つ以上のフィールドを連結する機能が追加されました。
* AttributeLoader-Regen-Enabled スクリプトの `attributeloader-regen.pl` が変更され、HTML エンコードされた値でなくなりました。
* 「範囲検索」クエリーのインデックス時間と検索時間の空白文字の処理が一致するようになりました。
* 動的ファセットを有効にすると、ビジネスルールの追加がエラーになることがあった問題を修正しました。

   [ビジネスルールについて](../c-about-rules-menu/c-about-business-rules.md#concept_2A93D76216754D3D8412CDEA00BD26BD)を参照してください。

* JavaScriptエラーが発生し、**設定**/**SPIN**/**IndexConnector**&#x200B;の定義を追加または編集できませんでした。
* ビジネスルールの作成時に時間が選択されると、ビジネスルールが保存された後、GMTタイムゾーンがデフォルトに設定されていた問題を修正しました。 ビジネスルールの保存後、アカウントのタイムゾーンで表示され、実施されていました。

   [ビジネスルールについて](../c-about-rules-menu/c-about-business-rules.md#concept_2A93D76216754D3D8412CDEA00BD26BD)を参照してください。

* ステージでのビジネスルールの並び替えが正しく動作していなかった問題を修正しました。

   [ビジネスルールについて](../c-about-rules-menu/c-about-business-rules.md#concept_2A93D76216754D3D8412CDEA00BD26BD)を参照してください。

* 検索パフォーマンスレポートが強化され、電子メール配信のレポートをスケジュールできるようになりました。
* ビジネスルールのスケジュールが修正され、自動的に夏時間に変更されるようになりました。

   [ビジネスルールについて](../c-about-rules-menu/c-about-business-rules.md#concept_2A93D76216754D3D8412CDEA00BD26BD)を参照してください。

* 多数の動的ファセットフィールドが定義された場合、主要な検索の応答時間が遅くなっていました。
* 正しくない範囲インデックスエラーが発生していた問題を修正しました。
* 北米以外のデータセンターでのDynamic Mediaクラシックアクセスが切断されていた問題を修正しました。
* SPIN XPath 検証関数が誤検知エラーを返していた問題を修正しました。

* SPIN の有効化／無効化の操作の後、ユーザーがメンバーセンターログインページにリダイレクトされていた問題を修正しました。
