---
description: Search&amp;Promote 8.14.0リリースノート。
solution: Target
title: Search&amp;Promote 8.14.0リリースノート（2014年5月23日）
topic-legacy: Release Notes,Site search and merchandising
uuid: 308d84a9-ec38-4fec-b146-e8a353e65be4
exl-id: fcc00d85-128e-4015-aa82-7d31606cb076
translation-type: tm+mt
source-git-commit: 7559f5f7437d46e3510d4659772308666425ec96
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 67%

---

# Search&amp;Promote8.14.0リリースノート（2014年5月23日）{#search-promote-release-notes}

**修正点**

* [!DNL sqlite_open] に失敗する場合、古い SQLite データベースファイルが退避され、新しいファイルが最初から作成されます。
* 同じ検索が繰り返されると、主要な検索結果が異なっていた問題を修正しました。
* 検索結果ごとに多くのフィールドが出力される場合のテンプレート処理のパフォーマンスが向上しました。
* **[!UICONTROL Business Rule History]**&#x200B;にメモを追加しました。
* インデックス作成処理時に、結果ベースのトリガーおよびアクションのプレビューインデックス再生成フェーズのパフォーマンスが時間の経過と共に着実に低下する問題を修正しました。
* **[!UICONTROL Reset SPIN cache]**&#x200B;オプションをboolean no/next-runから3つの状態に変更しました。no/always/next-run
