---
description: 検索クエリの結果の拡張を上書きできます。
solution: Target
title: クエリ拡張の上書きについて
topic-legacy: Linguistics,Site search and merchandising
uuid: dfe18004-b8fd-4889-b01c-72a3b0c82b9c
exl-id: 6157ffcb-e696-419a-acb5-2076c12a6763
translation-type: tm+mt
source-git-commit: 7559f5f7437d46e3510d4659772308666425ec96
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# クエリ拡張の上書きについて{#about-query-expansion-overrides}

検索クエリの結果の拡張を上書きできます。

## クエリ拡張の上書きの使用{#concept_6895B469B0E044299E93361BFA06B554}

クエリ拡張の上書きを設定する場合は、「ルール」のセットを作成します。 各ルールは、基本的に「`<this>`を検索時に`<that>`に拡張しないでください」と言います。`<this>`は単純なテキストの単語またはフレーズで、`<that>`はテキストの単語またはフレーズまたは分類です。

>[!NOTE]
>
>この機能は、Search&amp;Promoteではデフォルトで無効になっています。 お使いの機能をアクティブにするには、テクニカルサポートにお問い合わせください。 クエリ拡張の上書き機能を有効にした後は、ユーザインターフェイスでオンにする必要があります。

**クエリ拡張の上書きの動作**

クエリの拡張の上書きページでテキストと用語の値が指定されている場合、コードは特定のペアに追加基づいて動作します。 辞書や代替ワードFormsなど、分類タイプをキーワードとして指定した場合、「展開しない」の値は、指定した分類で作成された形式に変換されません。

例えば、次の定義があるとします。

`Do Not Expand = "dog"`

`Type = Text`

`Term = "dogs"`

「犬」の検索クエリは、「犬」を含み、「犬」と「犬」は、代替語「Forms」を介して含みません。

ただし、定義が次の場合は、

`Do Not Expand = "dog"`

`Type = Alternate Word Forms`

このクエリには、「dog&#39;s」または「dogs」(「dog」に対して使用可能な代替単語「Forms」)は含まれません。

複数のキーワード、複数の分類またはその両方を指定できます。 ただし、「種類」で「すべて」を選択した場合、複数の用語を含むリストは、単一の「すべて」のエントリに折りたたまれます。

テキストと分類のエントリがルール内で混在する場合、最初にテキスト値が表示されるように、ユーザーインターフェイス内で再編成されます。 ただし、検索時の評価の順序を示すものや影響を与えるものではありません。

テキスト用語は検証され、無意味な参照が削除されます。 つまり、キーワードと「展開しない」の値を比較し、一致が見つかった場合にそのキーワードを削除します。 また、重複用語の値（テキストまたは分類）は削除されます。

以前の定義と同じ「展開しない」の値を持つ新しいルールを追加した場合、新しい定義の用語は元の定義に追加されます。

## クエリ拡張の上書きの設定{#task_A087354A509D4997BA275186C224160E}

Search&amp;Promoteでのクエリ拡張の上書きの定義と追加を参照してください。

<!-- 

t_configuring_query_expansion_overrides.xml

 -->

>[!NOTE]
この機能は、Search&amp;Promoteではデフォルトで無効になっています。 お使いの機能をアクティブにするには、テクニカルサポートにお問い合わせください。 クエリ拡張の上書き機能を有効にした後は、ユーザインターフェイスでオンにする必要があります。 以下の最初の手順で、その方法を説明します。

**クエリ拡張の優先を設定するには**

1. Search&amp;Promoteで、**設定**/**ユーザー**/**表示の役割**&#x200B;をクリックします。
1. 表示の役割ページの表の「アクション」列で、言語の上書きに対するアクセス権を付与する役割の右側の&#x200B;**編集**&#x200B;をクリックします。
1. 「ロールを編集」ページで、言語ツリーを展開します。
1. **クエリ拡張の上書き**&#x200B;をチェックし、**変更の保存**&#x200B;をクリックします。
1. **言語学** > **クエリ拡張の上書き**&#x200B;をクリックします。
1. **追加クエリ拡張の上書き**&#x200B;をクリックします。
1. [クエリの拡張の優先]追加ページで、必要なオプションを設定します。

   <!-- 
   
   r_query_expansion_override_definitions.xml
   
   -->

   <table> 
    <thead> 
      <tr> 
      <th colname="col1" class="entry"> <p>オプション </p> </th> 
      <th colname="col2" class="entry"> <p>説明 </p> </th> 
      </tr> 
    </thead>
    <tbody> 
      <tr> 
      <td colname="col1"> <p>展開しない </p> </td> 
      <td colname="col2"> <p>拡大しない単語またはフレーズを指定します。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>タイプ </p> </td> 
      <td colname="col2"> <p>「<b>テキスト</b>」を選択して、特定の単語またはフレーズのペアを指定します。 または、分類を選択して、「単語またはフレーズを展開しない」を選択した分類を使用して変換しないようにします。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>用語 </p> </td> 
      <td colname="col2"> <p>「種類」で「<b>テキスト</b>」を選択した場合にのみ使用できます。 検索範囲から除外する単語またはフレーズを指定します。 </p> </td> 
      </tr> 
      <tr> 
      <td colname="col1"> <p>アクション </p> </td> 
      <td colname="col2"> <p> 定義にキーワードを追加または削除するには、<b>+</b>または<b>-</b>をクリックします。 </p> </td> 
      </tr> 
    </tbody> 
    </table>

1. 終了したら、**追加**&#x200B;をクリックします。

   [クエリ拡張の上書きの定義]ページで、追加した定義を編集または削除できます。
1. 追加の結果をプレビューするには、青いボックスの&#x200B;**ステージ済みサイトインデックス**&#x200B;を再生成して、ステージ済みWebサイトインデックスをすばやく再構築します。
1. （オプション）次のいずれかの操作を行います。

   * 「**ライブ**」をクリックします。

      [ライブ設定の表示](../c-about-staging.md#task_401A0EBDB5DB4D4CA933CBA7BECDC10F)を参照

   * 「**ライブをプッシュ**」をクリックします。

      [ステージ設定をライブにプッシュする](../c-about-staging.md#task_44306783B4C0408AAA58B471DAF2D9A4)を参照
